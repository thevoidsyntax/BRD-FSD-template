# Functional Specification Document

| | |
|---|---|
| **Document ID** | FSD-[YYYY]-[NNN] |
| **Related BRD** | BRD-[YYYY]-[NNN] |
| **Project** | [Project name] |
| **Version** | 0.1 |
| **Status** | Draft / In Review / Approved |
| **Author** | [Name] |
| **Last Updated** | [YYYY-MM-DD] |

## Revision History

| Version | Date | Author | Change |
|---|---|---|---|

---

## 1. Purpose

One paragraph. What this document specifies and who it is for.

## 2. Requirements Traceability

| BRD Ref | FSD Ref | Covered |
|---|---|---|
| BR-01 | FR-01, FR-02 | Yes |
| BR-02 | FR-03 | Yes |

If a business requirement has no FSD reference, either it was dropped or the spec is incomplete. Both need explaining.

## 3. Functional Requirements

### FR-01: [Name]

| | |
|---|---|
| **Priority** | Must / Should / Could |
| **BRD Ref** | BR-01 |
| **Actor** | |

**Description**

What the system does.

**Trigger**

What starts it.

**Preconditions**

- [Condition]

**Main Flow**

1. [Actor] does [action]
2. System validates [what]
3. System [response]

**Alternate Flows**

| # | Condition | Behaviour |
|---|---|---|
| A1 | | |

**Exception Flows**

| # | Condition | Behaviour | Message |
|---|---|---|---|
| E1 | Validation fails | Reject, stay on form | "[Exact text shown to user]" |

**Postconditions**

- [State after success]

**Business Rules Applied**

- BR-R01

---

## 4. Business Rules

| ID | Rule | Applies to |
|---|---|---|
| BR-R01 | If amount exceeds [X], route to [role] | FR-01 |

Keep rules separate from flows. Rules change more often than flows, and separating them means one edit instead of six.

## 5. Data Requirements

### 5.1 Fields

| Field | Type | Length | Required | Validation | Default |
|---|---|---|---|---|---|
| | | | Y/N | | |

### 5.2 Data Model Changes

New tables, new columns, changed keys, indexes.

### 5.3 Data Migration

| Source | Target | Volume | Transformation | Cutover |
|---|---|---|---|---|

## 6. Interface Requirements

| ID | System | Direction | Method | Frequency | Payload |
|---|---|---|---|---|---|
| INT-01 | | In/Out | API/File/DB | | |

### Error Handling

| Scenario | Behaviour | Retry | Alert |
|---|---|---|---|
| Timeout | | | |
| Invalid payload | | | |

## 7. User Interface

Screen list with field-level detail. Attach wireframes.

| Screen | Purpose | Access |
|---|---|---|
| | | |

## 8. Roles and Permissions

| Action | Requester | Reviewer | Approver | Admin |
|---|---|---|---|---|
| Create | Y | N | N | Y |
| Approve | N | N | Y | Y |
| View all | N | Y | Y | Y |

## 9. Reports

| Report | Fields | Filters | Format | Frequency | Recipient |
|---|---|---|---|---|---|

Before adding a report, confirm someone will read it. Most reports outlive their readers.

## 10. Non-Functional Requirements

| ID | Category | Requirement |
|---|---|---|
| NFR-01 | Performance | Response under [X] seconds at [Y] concurrent users |
| NFR-02 | Availability | [X]% during business hours |
| NFR-03 | Audit | All approvals logged with user, timestamp, previous value |
| NFR-04 | Retention | Records kept [X] years |

## 11. Test Scenarios

| ID | FR Ref | Scenario | Expected | Type |
|---|---|---|---|---|
| TS-01 | FR-01 | | | Positive |
| TS-02 | FR-01 | | | Negative |
| TS-03 | FR-01 | | | Boundary |

Every FR needs at least one negative and one boundary case. Positive-only test coverage is how defects reach production.

## 12. Open Items

| # | Item | Owner | Needed by | Status |
|---|---|---|---|---|

## Appendix

- A. Wireframes
- B. Data dictionary
- C. Interface specifications
