| Scheme                    | Media Needed | Backup Frequency            | Strengths                                  | Weaknesses                              |
|---------------------------|--------------|-----------------------------|--------------------------------------------|------------------------------------------|
| Grandfather-Father-Son    | High          | Daily, Weekly, Monthly      | Long retention, easy to manage             | High media cost, storage-intensive       |
| Tower of Hanoi            | Low–Moderate | Mathematically optimized    | Efficient use of media, good coverage      | Complex rotation logic                   |
| Six Cartridge Weekly      | Low           | Daily (Mon–Thu), Weekly (Fri) | Simple, low cost, recent data recovery    | Short retention window, no monthly copy  |

---

| Backup Type             | Description                                     | Pros                                 | Cons                                   | Best Use Case                          |
|-------------------------|-------------------------------------------------|--------------------------------------|----------------------------------------|----------------------------------------|
| Full                    | Complete copy of all data                       | Easiest to restore                   | Time & storage heavy                   | Periodic complete backups              |
| Incremental             | Changes since last backup                       | Fastest to backup, space-saving     | Slowest to restore                     | Daily backups with low impact          |
| Differential            | Changes since last full backup                  | Faster restore than incremental     | Grows larger over time                 | Balance between speed and storage      |
| Synthetic Full          | Virtual full backup built from previous backups | Offloads production systems         | Complexity in setup                    | Backup appliance environments          |
| Mirror                  | 1:1 replica of current state                    | Very fast restore                    | No versioning, deletions are copied    | Real-time duplication                  |
| Continuous Data Protection (CDP) | Real-time capture of all changes               | Near-zero data loss                 | High resource consumption              | Mission-critical systems               |
| Snapshot                | Point-in-time copy                              | Fast, low impact                    | Not a full backup solution alone       | VM & DB quick recovery                 |

---