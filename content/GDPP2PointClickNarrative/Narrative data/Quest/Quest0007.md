---
Quest_ID: Quest0007
Quest_name: Click on Guest A
Quest_type: main quest
Status:
Quest_description: You can click on an object or character to interact with it
Starter_prerequisite_type:
Hints:
  - "[[Hint0006]]"
Starter_item_ID: none
Starter_quest_ID: "[[Quest0006]]"
Starter_response_ID: none
Completion_prerequisite_type: Response selection
Completion_quest_ID: none
Completion_item_ID: none
Completion_response_ID: "[[Response0007]]"
Skill_check_result: none
tags:
  - quest
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[Quest0008]]"
  - "[[LC0002]]"
dg-publish: true
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