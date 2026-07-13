---
publish: true
created: 2026-07-03T17:16:37.124+07:00
modified: 2026-07-07T15:21:50.176+07:00
published: 2026-07-07T15:21:50.176+07:00
tags:
  - response
Response_ID: "[[Response0011]]"
Narrative_ID: "[[Narrative0007]]"
Response_text: Try to beat Guest D with your artistry skill
Player_action_description: Your artistry skill
Opponent_action_description: Ready to check your artistry
Skill_check_text: Can you beat Guest D with your artistry?
Response_prerequisite_type: Quest ongoing
Prerequisite_quest_ID: "[[Quest0010]]"
Prerequisite_item_ID: none
Skill_check?: yes
Skill_type: artistry
Multiple_skill_check_attempt?: yes
Item_check?: none
Item_Id: none
Succeed_outcome: "[[Outcome0016]]"
Failed_outcome: "[[Outcome0017]]"
Neutral_outcome: "[[Outcome0018]]"
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
