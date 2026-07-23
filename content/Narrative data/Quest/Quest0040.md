---
publish: true
created: 2026-07-11T16:39:22.909+07:00
modified: 2026-07-23T18:50:28.216+07:00
published: 2026-07-23T18:50:28.216+07:00
tags:
  - quest
Quest_ID: "[[Quest0040]]"
Quest_name: Meet Security Organizer at Organizer Room
Quest_type: main quest
Status:
Quest_description: Now that you have list of suspects, go to organizer room to meet Security Organizer
Hints:
Starter_prerequisite_type: Quest completion
Starter_item_ID:
Starter_quest_ID: "[[Quest0039]]"
Starter_response_ID:
Completion_prerequisite_type: Response selection
Completion_quest_ID:
Completion_quest_ID_relation:
Completion_item_ID:
Completion_item_ID_relation:
Completion_outcome_ID:
Completion_outcome_ID_relation:
Completion_response_ID:
  - "[[Response0148]]"
Completion_response_ID_relation: is
Skill_check_result:
Narrative_ID:
Narrative_ID_relation:
Starter_Narrative_ID: none
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[DT0018]]"
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
