---
publish: true
created: 2026-07-04T17:08:23.066+07:00
modified: 2026-07-07T15:21:56.172+07:00
published: 2026-07-07T15:21:56.172+07:00
tags:
  - response
Response_ID: "[[Response0015]]"
Narrative_ID: "[[Narrative0010]]"
Response_text: Interact to see whether you lose your health or sanity
Player_action_description: Prepare to lose some health or sanity
Opponent_action_description: Ready to take your health or sanity away
Skill_check_text: Look at opponent condition dice, it has face that will subtract your health or sanity
Response_prerequisite_type: Quest ongoing
Prerequisite_quest_ID: "[[Quest0012]]"
Prerequisite_item_ID: none
Outcome_ID_prerequisite: none
Skill_check?: yes
Skill_type: deception
Multiple_skill_check_attempt?: no
Item_check?: none
Item_Id: none
Succeed_outcome: "[[Outcome0021]]"
Failed_outcome: "[[Outcome0021]]"
Neutral_outcome: "[[Outcome0021]]"
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

- response\_id: [[Narrative data/Response/Response0015|Response0015]]

- narrative\_id: [[Narrative data/Narrative/Narrative0010|Narrative0010]]

- response\_text: Interact to see whether you lose your health or sanity

- player\_action\_description: Prepare to lose some health or sanity

- opponent\_action\_description: Ready to take your health or sanity away

- skill\_check\_text: Look at opponent condition dice, it has face that will subtract your health or sanity

- response\_prerequisite\_type: Quest ongoing

- prerequisite\_quest\_id: [[Narrative data/Quest/Quest0012|Quest0012]]

- prerequisite\_item\_id: none

- outcome\_id\_prerequisite: none

- skill\_check?: yes

- skill\_type: deception

- multiple\_skill\_check\_attempt?: no

- item\_check?: none

- item\_id: none

- succeed\_outcome: [[Narrative data/Outcome/Outcome0021|Outcome0021]]

- failed\_outcome: [[Narrative data/Outcome/Outcome0021|Outcome0021]]

- neutral\_outcome: [[Narrative data/Outcome/Outcome0021|Outcome0021]]

- tags: response

- response\_completion\_status: null

- quest\_id\_prerequisite\_relation: is

- item\_id\_prerequisite\_relation: none

- outcome\_id\_prerequisite\_relation: none
