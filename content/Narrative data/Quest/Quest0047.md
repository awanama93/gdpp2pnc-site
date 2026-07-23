---
publish: true
created: 2026-07-23T16:18:23.315+07:00
modified: 2026-07-24T04:12:16.571+07:00
published: 2026-07-24T04:12:16.571+07:00
Quest_name: Get away by the backdoor at the Convention Area
Completion_prerequisite_type: Narrative completion
Completion_item_ID:
Completion_item_ID_relation:
Completion_outcome_ID:
Completion_outcome_ID_relation:
Completion_quest_ID:
Completion_quest_ID_relation:
Completion_response_ID:
Completion_response_ID_relation:
Narrative_ID:
  - "[[Narrative0101]]"
Narrative_ID_relation: is
Quest_ID: "[[Quest0047]]"
canvas:
  - "[[_General Plot.canvas]]"
_General Plot:
  - "[[PNCEndingA.jpg]]"
Starter_prerequisite_type: Quest completion
Starter_quest_ID: "[[Quest0046]]"
Quest_type: main quest
Quest_description: Get away by the backdoor at the Convention Area
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
