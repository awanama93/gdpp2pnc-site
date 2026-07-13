---
publish: true
created: 2026-07-02T22:27:23.152+07:00
modified: 2026-07-11T20:25:05.214+07:00
published: 2026-07-11T20:25:05.214+07:00
tags:
  - quest
Quest_ID: "[[Quest0008]]"
Quest_name: Learn skill check with Guest B
Quest_type: main quest
Status:
Quest_description: To resolve certain situation you have to do skill check using dice
Starter_prerequisite_type: Quest completion
Hints:
  - "[[Hint0007]]"
  - "[[Hint0008]]"
  - "[[Hint0009]]"
Starter_item_ID: none
Starter_quest_ID: "[[Quest0007]]"
Starter_response_ID: none
Completion_prerequisite_type: Skill check result
Completion_quest_ID: none
Completion_item_ID: none
Completion_response_ID: "[[Response0008]]"
Skill_check_result: Succeed
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[Quest0009]]"
  - "[[LC0003]]"
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

Quest0008

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
