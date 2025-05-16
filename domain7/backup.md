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

# RAID Concpets

# 🧠 RAID Levels Explained

RAID (Redundant Array of Independent Disks) is a data storage technique that uses multiple disks to improve performance, fault tolerance, and/or capacity.

---

## 🔑 Key Concepts

| Concept     | Description                                                |
|-------------|------------------------------------------------------------|
| Striping    | Data is split across multiple disks (increases speed)      |
| Mirroring   | Data is duplicated on two or more disks (adds redundancy)  |
| Parity      | Error detection info that allows data recovery             |
| Hot Spare   | Idle disk that auto-replaces a failed disk                 |

---

## 🔢 RAID Level Summary

| RAID Level | Min Disks | Redundancy      | Performance     | Storage Efficiency | Use Case                           |
|------------|-----------|------------------|------------------|---------------------|------------------------------------|
| **RAID 0** | 2         | ❌ None           | 🚀 Very High (R/W) | 100%                | Non-critical temp data, scratch disk |
| **RAID 1** | 2         | ✅ Mirroring       | ⚡ High (read)      | 50%                 | Boot drives, critical small systems |
| **RAID 5** | 3         | ✅ Single parity   | ⚡ Balanced         | ~67–80%             | File servers, mail servers         |
| **RAID 6** | 4         | ✅ Dual parity     | ⏳ Slower writes    | ~50–75%             | Archive, backup storage            |
| **RAID 10**| 4 (2x2)   | ✅ Mirror + Stripe | 🚀 Very High        | 50%                 | Databases, high I/O apps           |
| **RAID 50**| 6         | ✅ Stripe of RAID 5| ⚡ High              | ~67–80%             | Large storage with some redundancy |
| **RAID 60**| 8         | ✅ Stripe of RAID 6| ⏳ Moderate          | ~50–75%             | Mission-critical, fault-tolerant   |
| **JBOD**   | 1+        | ❌ None           | 🚶 Very slow         | 100%                | Non-critical or home use           |

---

## 🔧 Notes

- **RAID 0**: No fault tolerance; failure of one disk = data loss.
- **RAID 1**: Excellent read performance, full redundancy.
- **RAID 5/6**: Use parity to recover from disk failure(s); RAID 6 survives 2 failures.
- **RAID 10**: Combines speed of RAID 0 with redundancy of RAID 1.
- **RAID 50/60**: Nested RAID; best for enterprise environments.
- **JBOD**: "Just a Bunch of Disks"; not technically RAID; no redundancy.

---

## 🎓 CISSP Domain Relevance

- **Domain 7: Security Operations** – Availability & fault tolerance
- **Domain 5: IAM** – Protecting stored identity data
- **BCP/DRP** – RAID supports **RTO/RPO** goals for recovery

---