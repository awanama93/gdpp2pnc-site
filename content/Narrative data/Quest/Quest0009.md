---
publish: true
created: 2026-07-03T10:38:36.096+07:00
modified: 2026-07-06T09:10:48.121+07:00
published: 2026-07-06T09:10:48.121+07:00
tags:
  - quest
Quest_ID: Quest0009
Quest_name: Succeed in skill check with Guest C
Quest_type: main quest
Status:
Quest_description: Sometimes you have to succeed in skill check. Learn how that works
Hints:
  - "[[Hint0010]]"
Starter_prerequisite_type: Quest completion
Starter_item_ID: none
Starter_quest_ID: "[[Quest0008]]"
Starter_response_ID: none
Completion_prerequisite_type: Skill check result
Completion_quest_ID: none
Completion_item_ID: none
Completion_response_ID: "[[Response0009]]"
Skill_check_result: Succeed
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[Quest0010]]"
  - "[[LC0004]]"
dg-publish: true
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
