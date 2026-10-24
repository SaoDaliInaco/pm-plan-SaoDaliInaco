# Project charter: Realtime Quiz platform

| Field   | Value                            |
| ------- | -------------------------------- |
| Version | 1.0 (draft for sponsor approval) |
| Date    | 2026-09-29                       |
| Sponsor | Head of the IT department        |
| PM      | Supervising Lecturer             |

## 1. Purpose and justification

Lecturers currently spend extensive manual hours grading assessments without receiving immediate student comprehension data during lectures. The Realtime Quiz platform will provide a web-based, real-time multiple-choice assessment tool featuring instant scoring, WebSocket updates, and live leaderboards to increase classroom engagement and eliminate manual grading overhead. Completing this project will establish an in-house digital assessment capability hosted at gicitc.com while delivering key capstone learning outcomes for student developers. For detailed financial and strategic justification, see `business-case.md`.

## 2. Objectives and success criteria

| #   | Objective (what will be true)                                                 | Success criterion (number + week)                                                                                            |
| --- | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| O1  | Deploy a functional MVP with all core quiz creation and live session features | 100% of Must features passing acceptance tests by week 7                                                                     |
| O2  | Conduct a live pilot session under real classroom conditions                  | 50 concurrent student participants with 0 blocking defects in week 14                                                        |
| O3  | Maintain low-latency broadcast performance during live sessions               | Broadcast latency <= 500 ms at the 95th percentile, measured in week 14                                                      |
| O4  | Ensure authoritative server performance under expected full load              | 1 server instance serving 20 concurrent sessions of 100 participants (2 vCPU, 2 GB RAM) with timer drift < 200 ms in week 13 |
| O5  | Maintain software quality and test coverage through continuous integration    | Line coverage >= 80% with green CI pipeline on all merges through week 14                                                    |

## 3. High-level scope

In scope:

- Quiz authoring module for multiple-choice questions
- Real-time live session participation via 6-character access codes
- WebSocket-based real-time scoring, timers, and instant leaderboard updates
- Authentication and role-based access control (Instructor, Student, Guest, Admin)
- Export of quiz session results and analytics to CSV and PDF formats

Out of scope:

- Native mobile applications (iOS / Android)
- Non-multiple-choice question formats (free text, open essay)
- Video conferencing integration
- Learning Management System (LMS) integration
- Multi-node distributed scaling (architecture limited to single server instance)

## 4. Milestones

| Week | Milestone                           | Ends process group         |
| ---- | ----------------------------------- | -------------------------- |
| 1    | Charter approved, team formed       | Initiating                 |
| 3    | Architecture & PM Plan finalized    | Planning                   |
| 7    | MVP demo                            | Executing                  |
| 11   | Should/Could features complete      | Executing                  |
| 12   | Load testing & system hardening     | Executing                  |
| 13   | Pilot readiness & operation handoff | Monitoring and Controlling |
| 14   | Pilot with 50 students, closure     | Closing                    |

## 5. Budget summary

Effort: students 4 x 14 x 8 h = 448 h; PM 14 x 3 h = 42 h; total 490 h
Cash: hosting 4 x 25 USD = 100 USD; domain = 15 USD; tools = 60 USD; reserve = 25 USD (14 %)
total 200 USD

## 6. Assumptions

- Student team members contribute an average of 8 hours per week throughout the 14-week timeline.
- The IT department provides hosting infrastructure (Linode VPS) at gicitc.com.
- The campus Wi-Fi network and proxy allow persistent WebSocket/STOMP connections or SockJS fallbacks without blocking traffic.

## 7. Constraints

- Strict project completion timeline of 14 weeks starting 2026-09-29.
- Maximum total cash expenditure cap of 200 USD.
- Platform deployment bounded by single-instance hardware limits (2 vCPU, 2 GB RAM).

## 8. High-level risks

- Campus proxy blocking native WebSockets, requiring SockJS fallback testing early in development.
- Clock drift between client browsers and the central server affecting timer accuracy.
- Khmer name rendering failures during PDF export generation.

## 9. Project manager authority

The Project Manager has full authority to reallocate effort across team roles and manage the 200 USD budget up to the allocated reserve limit without higher approval. Any requests for scope changes, moving the week 14 pilot date, or exceeding the 200 USD cash cap require formal written approval from the Sponsor within 5 working days.

## 10. Approval

Sponsor: ********\_\_\_\_******** Date: **\_\_\_\_**
PM: ********\_\_\_\_******** Date: **\_\_\_\_**
