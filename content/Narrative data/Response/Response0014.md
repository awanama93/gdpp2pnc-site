---
publish: true
created: 2026-07-04T15:03:01.199+07:00
modified: 2026-07-07T15:21:54.117+07:00
published: 2026-07-07T15:21:54.117+07:00
tags:
  - response
Response_ID: "[[Response0014]]"
Narrative_ID: "[[Narrative0009]]"
Response_text: Interact to Guest B to lose condition dice
Player_action_description: Observing Guest B
Opponent_action_description: Ready to take your condition away
Skill_check_text: Whatever happens, after this you will lose condition...
Response_prerequisite_type: Outcome received
Prerequisite_quest_ID: none
Prerequisite_item_ID: none
Skill_check?: yes
Skill_type: observation
Multiple_skill_check_attempt?: no
Item_check?: none
Item_Id: none
Succeed_outcome: "[[Outcome0020]]"
Failed_outcome: "[[Outcome0020]]"
Neutral_outcome: "[[Outcome0020]]"
Outcome_ID_prerequisite: "[[Outcome0019]]"
dg-publish: true
Response_completion_status:
Quest_ID_prerequisite_relation: none
Item_ID_prerequisite_relation: none
Outcome_ID_prerequisite_relation: is
---

```datacorejsx
return function TitleHeader() { 
const file = dc.useCurrentFile(); 
if (!file) return null; 
// file.$name contains the clean string of the note title 
return <h1>{file.$name}</h1>; }

```

- response\_id: [[Narrative data/Response/Response0014|Response0014]]

- narrative\_id: [[Narrative data/Narrative/Narrative0009|Narrative0009]]

- response\_text: Interact to Guest B to lose condition dice

- player\_action\_description: Observing Guest B

- opponent\_action\_description: Ready to take your condition away

- skill\_check\_text: Whatever happens, after this you will lose condition...

- response\_prerequisite\_type: Outcome received

- prerequisite\_quest\_id: none

- prerequisite\_item\_id: none

- skill\_check?: yes

- skill\_type: observation

- multiple\_skill\_check\_attempt?: no

- item\_check?: none

- item\_id: none

- succeed\_outcome: [[Narrative data/Outcome/Outcome0020|Outcome0020]]

- failed\_outcome: [[Narrative data/Outcome/Outcome0020|Outcome0020]]

- neutral\_outcome: [[Narrative data/Outcome/Outcome0020|Outcome0020]]

- tags: response

- outcome\_id\_prerequisite: [[Narrative data/Outcome/Outcome0019|Outcome0019]]

- response\_completion\_status: null

- quest\_id\_prerequisite\_relation: none

- item\_id\_prerequisite\_relation: none

- outcome\_id\_prerequisite\_relation: is
