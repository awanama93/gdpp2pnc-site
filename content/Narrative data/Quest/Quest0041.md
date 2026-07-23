---
publish: true
created: 2026-07-22T14:56:27.517+07:00
modified: 2026-07-23T18:50:26.468+07:00
published: 2026-07-23T18:50:26.468+07:00
tags:
  - quest
Quest_ID: "[[Quest0041]]"
Quest_name: Tell Security Organizer about your suspects
Quest_type: main quest
Status:
Quest_description: Tell him about your suspects, Stage Host and Musician
Hints:
Starter_prerequisite_type: Quest completion
Starter_item_ID:
Starter_quest_ID: "[[Quest0040]]"
Starter_response_ID:
Starter_Narrative_ID:
Completion_prerequisite_type: Narrative completion
Completion_quest_ID:
Completion_quest_ID_relation:
Completion_item_ID:
Completion_item_ID_relation:
Completion_outcome_ID:
Completion_outcome_ID_relation:
Completion_response_ID:
Completion_response_ID_relation:
Skill_check_result:
Narrative_ID:
Narrative_ID_relation:
canvas:
  - "[[_General Plot.canvas]]"
_General Plot: []
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
