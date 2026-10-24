# Process Groups Mapping

| Process group              | Weeks active | Main activities                                                                     | Outputs                                                 | Lab that produces them  |
| -------------------------- | ------------ | ----------------------------------------------------------------------------------- | ------------------------------------------------------- | ----------------------- |
| Initiating                 | 1            | Define project charter, identify stakeholders, construct business case              | Project Charter, Stakeholder Register, Business Case    | Lab 01                  |
| Planning                   | 1-3, 7-8     | Develop project management plan, WBS, schedule, risk register, and re-plan post-MVP | WBS, Gantt Chart, Risk Matrix, Architecture Specs       | Labs 02, 03, 04, 07, 08 |
| Executing                  | 3-12         | Build software components, implement WebSocket, integrate features, perform CI/CD   | Source Code, Test Suites, Working Builds, MVP Demo      | Labs 05, 06, 09, 10     |
| Monitoring and controlling | 1-14         | Track progress, evaluate schedule/cost variances, review risks, manage changes      | Weekly Status Reports, Change Logs, Updated Baselines   | Labs 05, 06, 09, 11     |
| Closing                    | 13-14        | Conduct 50-student pilot, perform final acceptance, complete handoff, post-mortem   | Final Pilot Report, Operations Runbook, Lessons Learned | Lab 12                  |

## Process groups over the semester

```mermaid
gantt
  title Process groups over the 14-week semester (Realtime Quiz)
  dateFormat YYYY-MM-DD
  axisFormat %d %b
  section Initiating
  Charter, stakeholders, business case   :i1, 2026-09-29, 7d
  section Planning
  PM plan and subsidiary plans           :p1, 2026-09-29, 21d
  Re-planning after each status review   :p2, 2026-11-17, 14d
  section Executing
  Build to MVP (Must features)           :e1, 2026-10-13, 35d
  MVP demo                               :milestone, m1, 2026-11-13, 0d
  Should and Could features, hardening   :e2, 2026-11-17, 28d
  section Monitoring and controlling
  Weekly status, variance, change log    :m2, 2026-09-29, 98d
  section Closing
  Pilot with 50 students, lessons learned :c1, 2026-12-29, 7d
  Pilot Go-Live                          :milestone, m2, 2027-01-05, 0d
```
