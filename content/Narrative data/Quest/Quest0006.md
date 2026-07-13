---
publish: true
created: 2026-07-02T18:38:52.302+07:00
modified: 2026-07-11T20:25:05.154+07:00
published: 2026-07-11T20:25:05.154+07:00
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
  - "[[DT0002]]"
  - "[[DT0001]]"
Completion_quest_ID_relation: is
Completion_item_ID_relation: none
Completion_response_ID_relation: none
Completion_outcome_ID_relation: none
Completion_outcome_ID: none
Narrative_ID:
  - none
Narrative_ID_relation: none
Starter_Narrative_ID: none
---

Quest0006

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
