---
Quest_ID: Quest0010
Quest_name: Beat Guest D in any skill check
Quest_type: main quest
Status:
Quest_description: Sometimes you have multiple ways to beat opponent on skill check. Learn how that works
Hints:
  - "[[Hint0011]]"
  - "[[Hint0012]]"
  - "[[Hint0013]]"
Starter_prerequisite_type: Quest completion
Starter_item_ID: none
Starter_quest_ID: "[[Quest0009]]"
Starter_response_ID: none
Completion_prerequisite_type: Skill check result
Completion_quest_ID: none
Completion_item_ID: none
Skill_check_result: Succeed
Completion_response_ID:
  - "[[Response0010]]"
  - "[[Response0011]]"
  - "[[Response0012]]"
tags:
  - quest
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[Quest0011]]"
  - "[[LC0005]]"
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