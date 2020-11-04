## Planning in Agile

Takes a signigicantly different flavour from traditional approaches.

Detailed planning is deferred until the start of the iteration.

- Designed to handle change
- An iteration includes all phases (requirements, design and test)

Planning is based on light weight lists

- Gannt and PERT charts are considered less useful

### Planning in SCRUM

|   Level   |       Horizon        |               Who               |                Focus                |                      Deliverables                       |
| :-------: | :------------------: | :-----------------------------: | :---------------------------------: | :-----------------------------------------------------: |
| Portfolio |     Year or more     |   Stakholders, product owners   |    Manaing portfolio of projects    | Portfolio backlog and collection of in-process products |
|  Product  |        Months        |   Product owner, stakeholders   |    Visions and product evolution    |      Product vision, high level features, roadmap       |
|  Release  | Three to Nine months |    SCRUM team, Stakeholders     | balance customer value, constraints |                      Release PLan                       |
|  Sprint   |    Week to Month     |           SCRUM team            |     What to deliver next sprint     |                  Sprint goals backlog                   |
|   Daily   |        Daily         | SCRUM Master, developement team |  How to complete commited features  |             Inspection of current progress              |

### Fixed Date Release Planning

1. Determine the number of sprints N by `N := allocated_time/sprint_length`
2. Groom the product backlog by estimating and prioritizing stories
3. Measure team velocity range, V_min, V_max
4. Compute minimum and maximum story points based on velocity. `SP_min := V_min * N`, `SP_max := V_max * N`
5. Draw lines through product backlog to show above

### Fixed Scope Release Planning

1. Groom the product backlog by creating, estimating and prioritizing and identify must-have stories.
2. Determine total number of must have story points, `SP_total`.
3. Measure team velocity, `V_min`, `V_max`.
4. Compute minimum and maximum number of sprints, `S_min := SP_total/V_max`, `S_max := SP_total/V_min`
5. Show burndown chart
