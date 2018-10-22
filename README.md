# RCA Knowledge Graphs

This repository contains the implementatioin and the information for the deployment of knowledge discovery and concept association graphs, using the visual tool proposed 
in HIVE Plots (https://bost.ocks.org/mike/hive/). For our project we will use a structure based on entities (people) and a number of attributes 
and organizational structures to give value to the represented data.

## Usage and deployment

Source code in the ``/docs`` directory of the repository. Changes are implemented directly in the project website in:  https://manuparra.github.io/knowledgegraphs/

## Database structure

### Version 0.5

JSON database, organized following the next (entity name, projects, expertise):

```
{
    "name": "person.ManuelParra",
    "projects": [
      "org.CERN.EP_NU.DUNE",
      "org.CERN.IdeaSquare",
      "org.CERN.EP_NU",
      "org.CERN"
    ],
    "expertise": [
      "programming.Python",
      "programming.JS"
    ]
}
```

### Version 1.0

JSON database, organized following the next (entity name, projects, institute, residence, contact, expertise):

```
{
    "name": ["ipt.CharlotteQin"],
    "projects": ["CERN.IdeaSquare"],
    "institutes": ["org.ImperialCollegeLondon","collab.RoyalCollegeofArt"],
    "residence": ["London,UK"],
    "contact": ["charlotte.qin@cern.ch"],
    "expertise": ["design, prototyping, graphics, programming in python and D3js"]
}
```