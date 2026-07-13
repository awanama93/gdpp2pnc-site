---
publish: true
created: 2026-07-04T17:25:27.370+07:00
modified: 2026-07-11T20:25:05.439+07:00
published: 2026-07-11T20:25:05.439+07:00
tags:
  - quest
Quest_ID: "[[Quest0013]]"
Quest_name: Learn about special dice
Quest_type: main quest
Status:
Quest_description: Other than skill and condition dice, along the way you will have special dice. Learn about that
Hints:
  - "[[Hint0017]]"
  - "[[Hint0018]]"
  - "[[Hint0019]]"
Starter_prerequisite_type: Quest completion
Starter_item_ID: none
Starter_quest_ID: "[[Quest0012]]"
Starter_response_ID: none
Completion_prerequisite_type: Skill check result
Completion_quest_ID: none
Completion_item_ID: none
Skill_check_result: Any
Completion_response_ID:
  - "[[Response0018]]"
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[Quest0014]]"
  - "[[LC0006]]"
dg-publish: true
Completion_quest_ID_relation: none
Completion_item_ID_relation: none
Completion_response_ID_relation: is
Completion_outcome_ID_relation: none
Completion_outcome_ID: none
Narrative_ID:
  - none
Narrative_ID_relation: none
Starter_Narrative_ID: none
---

Quest0013

```datacorejsx
return function View() {
const file = dc.useCurrentFile();
const hiddenKeys = ["dg-publish", "publish"];

if(!file) return <p>loading</p>;

const KUMPULAN = file.$frontmatter;

const items = Object.entries(KUMPULAN)
	.filter(([key]) => !key.startsWith("__") && !hiddenKeys.includes(key))
	.map(([key, field]) => {return `${key}: ${field?.value}`;}
);
	return <dc.List rows={items} />;
}

```
