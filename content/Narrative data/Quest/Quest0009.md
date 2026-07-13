---
publish: true
created: 2026-07-03T10:38:36.096+07:00
modified: 2026-07-11T20:25:05.243+07:00
published: 2026-07-11T20:25:05.243+07:00
tags:
  - quest
Quest_ID: "[[Quest0009]]"
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

Quest0009

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
