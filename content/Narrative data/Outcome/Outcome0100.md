---
publish: true
created: 2026-07-10T11:56:02.964+07:00
modified: 2026-07-11T21:12:17.621+07:00
published: 2026-07-11T21:12:17.621+07:00
Outcome_ID: "[[Outcome0100]]"
Response_ID:
  - "[[Response0070]]"
Outcome_name: He lets you prove yourself
Outcome_type: Any response
Outcome_response: He's not fully believed you but give you chance to prove your innocence
EXP_gain: "6"
Add_item_ID:
Subtract_item_ID:
Condition_target_1:
Condition_dice_1_type_modification:
Condition_dice_1_ID:
Condition_dice_1_influenced_skill_type:
Condition_target_2:
Condition_dice_2_type_modification:
Condition_dice_2_ID:
Condition_dice_2_influenced_skill_type:
Condition_target_3:
Condition_dice_3_ID:
Condition_dice 3_type_modification:
Condition_dice_3_influenced_skill_type:
Special_dice_face_1_addition:
Special_dice_face_2_addition:
Special_dice_face_3_addition:
tags:
---

Outcome0100

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
