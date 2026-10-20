# Task 1: project, operation or programme?

| #   | Initiative                                                                                                 | Temporary? | Unique? | Coordinated? | Class     | Justification                                                         |
| --- | ---------------------------------------------------------------------------------------------------------- | ---------- | ------- | ------------ | --------- | --------------------------------------------------------------------- |
| 1   | Build the Realtime Quiz platform and pilot it with 50 students in week 14                                  | yes        | yes     | no           | Project   | Fixed end at the week-14 pilot, and the platform did not exist before |
| 2   | Run the nightly backup of the gicitc.com PostgreSQL database                                               | no         | no      | no           | Operation | Repeats nightly with the same output and no end date                  |
| 3   | Move the department's three web servers to a new Linode region before 15 December                          | yes        | yes     | no           | Project   | Deadline of 15 December, one-time move                                |
| 4   | Answer helpdesk tickets within the 4-hour service level                                                    | no         | no      | no           | Operation | Ongoing service level, repeated for every ticket                      |
| 5   | "Digital classroom": Realtime Quiz, LMS upgrade and lecture capture sharing one login and one grade export | yes        | yes     | yes          | Programme | Three related projects share one login and one grade export           |
| 6   | Apply the monthly security patches to the VPS                                                              | no         | no      | no           | Operation | Repeats monthly with the same procedure                               |
| 7   | Add multi-node scaling (RabbitMQ relay, Redis registry) to Realtime Quiz next semester                     | yes        | yes     | no           | Project   | New capability with its own end next semester                         |
| 8   | Operate the Realtime Quiz platform after go-live: password resets, restarts, monitoring                    | no         | no      | no           | Operation | Continuous running after go-live, no end date                         |
| 9   | Write and publish the department's annual IT report for the dean by 31 January                             | yes        | yes     | no           | Project   | Each report is unique with a 31 January deadline                      |
| 10  | Replace 40 wireless access points in two buildings during the summer break                                 | yes        | yes     | no           | Project   | Summer-break deadline, one-time replacement                           |

## Grey zones

TODO: two rows that could go either way and what would settle them.
Row 7: is it a maintenance release or a new project? It depends on whether the sponsor funds it separately with its own end date and budget.
Row 9: it is annual and repetitive, yet each report is unique with a deadline. It depends on whether “done” is defined per report and whether it has its own budget.

## What our project hands over

TODO: three sentences.
IT operations (VPS admin) run the platform after week 14, covering restarts, backups and monitoring. They need a runbook, docker-compose.prod.yml, the environment variable list and a backup/restore check. Lecturers and the helpdesk need a short user guide for password resets and live-session problems.
