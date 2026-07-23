---
publish: true
created: 2026-07-23T21:45:12.531+07:00
modified: 2026-07-24T05:20:31.911+07:00
published: 2026-07-24T05:20:31.911+07:00
Outcome_ID:
Outcome_type: Succeed or neutral response
Response_ID:
  - "[[Response0184]]"
Outcome_name: Reveal in defeat
Outcome_response: Finally in defeat she tells you the reason Stage Host did that
EXP_gain: "5"
Add_item_ID:
Subtract_item_ID:
Condition_target_1: Player
Condition_dice_1_type_modification: addition
Condition_dice_1_ID: "[[DPBUnshakable]]"
Condition_dice_1_influenced_skill_type: deception
Condition_target_2: Opponent
Condition_dice_2_type_modification: addition
Condition_dice_2_ID: "[[DONStrained]]"
Condition_dice_2_influenced_skill_type: reflex
Condition_target_3: Opponent
Condition_dice_3_ID:
Condition_dice 3_type_modification: subtraction
Condition_dice_3_influenced_skill_type: any dice containing knowledge buff
Special_dice_face_1_addition:
Special_dice_face_2_addition:
Special_dice_face_3_addition:
tags:
Health_Modifier:
Sanity_Modifier:
---

```datacorejsx

return function TitleHeader() {

const file = dc.useCurrentFile();

if (!file) return null;

// file.$name contains the clean string of the note title

return <h1>{file.$name}</h1>; }

```
