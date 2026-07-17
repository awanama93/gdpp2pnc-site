---
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
- Quest_ID: `VIEW[{Quest_ID}][text(renderMarkdown)]`
- Status: `VIEW[{Status}][text(renderMarkdown)]`
- Quest_type: `VIEW[{Quest_type}][text(renderMarkdown)]`
- Quest_name: `VIEW[{Quest_name}][text(renderMarkdown)]`
- Quest_description: `VIEW[{Quest_description}][text(renderMarkdown)]`
- Hints: `VIEW[{Hints}][text(renderMarkdown)]`
- Starter_prerequisite_type: `VIEW[{Starter_prerequisite_type}][text(renderMarkdown)]`
- Starter_item_ID: `VIEW[{Starter_item_ID}][text(renderMarkdown)]`
- Starter_quest_ID: `VIEW[{Starter_quest_ID}][text(renderMarkdown)]`
- Starter_response_ID: `VIEW[{Starter_response_ID}][text(renderMarkdown)]`
- Completion_prerequisite_type: `VIEW[{Completion_prerequisite_type}][text(renderMarkdown)]`
- Completion_item_ID: `VIEW[{Completion_item_ID}][text(renderMarkdown)]`
- Completion_quest_ID: `VIEW[{Completion_quest_ID}][text(renderMarkdown)]`
- Completion_response_ID: `VIEW[{Completion_response_ID}][text(renderMarkdown)]`
- Skill_check_result: `VIEW[{Skill_check_result}][text(renderMarkdown)]`

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

