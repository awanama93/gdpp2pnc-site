---
publish: true
created: 2026-07-23T21:45:12.531+07:00
modified: 2026-07-24T05:32:53.672+07:00
published: 2026-07-24T05:32:53.672+07:00
Outcome_ID:
Outcome_type: Failed response
Response_ID:
  - "[[Response0186]]"
Outcome_name: Reluctantly accept demand
Outcome_response: She accepts reluctantly the demand to do something about the Convention
EXP_gain: "2"
Add_item_ID:
Subtract_item_ID:
Condition_target_1: Player
Condition_dice_1_type_modification: addition
Condition_dice_1_ID: "[[DPNDrained]]"
Condition_dice_1_influenced_skill_type: strength
Condition_target_2: Opponent
Condition_dice_2_type_modification: addition
Condition_dice_2_ID: "[[DOBDiscrening]]"
Condition_dice_2_influenced_skill_type: knowledge
Condition_target_3: Player
Condition_dice_3_ID:
Condition_dice 3_type_modification: subtraction
Condition_dice_3_influenced_skill_type: any dice containing artistry buff
Special_dice_face_1_addition:
Special_dice_face_2_addition:
Special_dice_face_3_addition:
tags:
Health_Modifier: "-1"
Sanity_Modifier:
---

```datacorejsx

return function TitleHeader() {

const file = dc.useCurrentFile();

if (!file) return null;

// file.$name contains the clean string of the note title

return <h1>{file.$name}</h1>; }

```
