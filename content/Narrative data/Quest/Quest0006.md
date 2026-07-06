---
publish: true
created: 2026-07-02T18:38:52.302+07:00
modified: 2026-07-06T10:11:07.319+07:00
published: 2026-07-06T10:11:07.319+07:00
tags:
  - quest
Quest_ID: "[[Quest0006]]"
Status:
Quest_type: main quest
Quest_name: How the world works
Quest_description: Learn how to interact with the game, then you're ready to play the game
Hints:
  - "[[Hint0022]]"
  - "[[Hint0023]]"
Starter_prerequisite_type: none
Starter_item_ID: none
Starter_quest_ID: none
Starter_response_ID: none
Completion_prerequisite_type: Quest completion
Completion_item_ID: none
Completion_quest_ID: "[[Quest0014]]"
Completion_response_ID:
  - none
Skill_check_result: none
canvas:
  - "[[_General Plot.canvas]]"
dg-publish: true
_General Plot:
  - "[[Quest0007]]"
---

### Properties

- Quest\_ID: `VIEW[{Quest_ID}][text(renderMarkdown)]`
- Status: `VIEW[{Status}][text(renderMarkdown)]`
- Quest\_type: `VIEW[{Quest_type}][text(renderMarkdown)]`
- Quest\_name: `VIEW[{Quest_name}][text(renderMarkdown)]`
- Quest\_description: `VIEW[{Quest_description}][text(renderMarkdown)]`
- Hints: `VIEW[{Hints}][text(renderMarkdown)]`
- Starter\_prerequisite\_type: `VIEW[{Starter_prerequisite_type}][text(renderMarkdown)]`
- Starter\_item\_ID: `VIEW[{Starter_item_ID}][text(renderMarkdown)]`
- Starter\_quest\_ID: `VIEW[{Starter_quest_ID}][text(renderMarkdown)]`
- Starter\_response\_ID: `VIEW[{Starter_response_ID}][text(renderMarkdown)]`
- Completion\_prerequisite\_type: `VIEW[{Completion_prerequisite_type}][text(renderMarkdown)]`
- Completion\_item\_ID: `VIEW[{Completion_item_ID}][text(renderMarkdown)]`
- Completion\_quest\_ID: `VIEW[{Completion_quest_ID}][text(renderMarkdown)]`
- Completion\_response\_ID: `VIEW[{Completion_response_ID}][text(renderMarkdown)]`
- Skill\_check\_result: `VIEW[{Skill_check_result}][text(renderMarkdown)]`

Dataview

```dataviewjs
// Grab the frontmatter object of the current file
let frontmatter = dv.current();

if (frontmatter) {
    let output = [];
    
    // Loop through every key in the metadata
    for (let key of Object.keys(frontmatter)) {
        // Filter out Dataview's internal system keys
        if (!["file", "id", "position"].includes(key)) {
            let value = frontmatter[key];
            
            // Format arrays (like lists of links) into comma-separated text
            if (Array.isArray(value)) {
                value = value.join(", ");
            }
            
            output.push(`- **${key}**: ${value}`);
        }
    }
    
    // Print the final list as plain markdown prose
    dv.paragraph(output.join("\n"));
}
```
