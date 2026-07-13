---
publish: true
created: 2026-07-03T18:13:00.639+07:00
modified: 2026-07-07T15:21:51.773+07:00
published: 2026-07-07T15:21:51.773+07:00
tags:
  - response
Response_ID: "[[Response0013]]"
Narrative_ID: "[[Narrative0008]]"
Response_text: Interact to Guest A to get condition dice
Player_action_description: Observing Guest A
Opponent_action_description: Ready to give you condition
Skill_check_text: Whatever happens, after this you will get condition...
Response_prerequisite_type: Quest ongoing
Prerequisite_quest_ID: "[[Quest0011]]"
Prerequisite_item_ID: none
Skill_check?: yes
Skill_type: observation
Multiple_skill_check_attempt?: no
Item_check?: none
Item_Id: none
Succeed_outcome: "[[Outcome0019]]"
Failed_outcome: "[[Outcome0019]]"
Neutral_outcome: "[[Outcome0019]]"
Outcome_ID_prerequisite: none
dg-publish: true
Response_completion_status:
Quest_ID_prerequisite_relation: is
Item_ID_prerequisite_relation: none
Outcome_ID_prerequisite_relation: none
---

```datacorejsx
return function TitleHeader() { 
const file = dc.useCurrentFile(); 
if (!file) return null; 
// file.$name contains the clean string of the note title 
return <h1>{file.$name}</h1>; }

```

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
