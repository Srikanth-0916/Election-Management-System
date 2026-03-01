# Election Management System
### Built on Zoho Creator

![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![Platform](https://img.shields.io/badge/Platform-Zoho%20Creator-orange)
![Status](https://img.shields.io/badge/Status-Active-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## Overview

The Election Management System (EMS) is a full-cycle election administration app built on Zoho Creator. It handles everything from voter registration and candidate nominations to live vote counting, result declaration, and grievance management — all in one place.

Whether you're running a government election, a university vote, or a corporate poll, this system is built to keep things transparent, secure, and organized.

---

## What It Does

- Voter registration with OTP verification and duplicate detection
- Candidate nomination workflow with document uploads and officer approval
- Polling booth assignment with GPS tracking and capacity management
- Live results dashboard that auto-refreshes every 2 minutes
- Mobile-friendly officer portal for field check-ins and vote count entry
- Automated notifications via Email and SMS at every key stage
- Complaint filing and tracking with auto-assignment and escalation
- Full audit logging for every action taken in the system
- Public pages for voter registration and result viewing — no login needed

---

## Modules

| Module | Description |
|--------|-------------|
| Election Configuration | Set up elections, define timelines, auto-lock forms by date |
| Constituency & Ward Management | Define zones, link voters, booths, and officers |
| Voter Registration | Register voters with OTP, auto-generate Voter ID on approval |
| Candidate Management | Nomination workflow with document uploads and approvals |
| Polling Booth Management | Assign booths, manage capacity, capture GPS coordinates |
| Election Officer Management | Duty assignment, check-in tracking, location capture |
| Ballot Configuration | Set candidate order, enable NOTA, lock ballot before voting |
| Vote Count Submission | Booth-wise entry with hourly turnout and auto-totals |
| Results & Winner Declaration | Auto-calculate winners, margins, and publish results |
| Complaint & Grievance System | File, assign, track, and resolve complaints |
| Document Management | Centralized document storage with bulk export and watermarking |

---

## User Roles

| Role | Access |
|------|--------|
| Super Admin | Full access — configure elections, approve records, declare results, view audit logs |
| Election Officer | Booth check-in, vote count entry, complaint handling |
| Candidate | View own profile, constituency results, submit withdrawal |
| Voter / Public | Submit registration form, check status, view assigned booth |
| Observer / Auditor | Read-only access to all modules and reports |
| Media / Public | Live results dashboard only, no login required |

---

## How the Key Workflows Work

**Voter Registration**
A voter fills out the public registration form, verifies their phone via OTP, and the system checks for duplicates using their National ID. Once an officer approves, a Voter ID is auto-generated and sent to them along with their assigned booth details.

**Candidate Nomination**
Candidates submit their nomination with all required documents. An election officer reviews and approves or rejects the application. Approved candidates are auto-assigned a Candidate ID and notified by email.

**Election Day**
Officers check in at their booth via the mobile app — the system captures their GPS location and timestamp. They submit vote counts at regular intervals, and the admin dashboard updates in real time. If a booth turnout drops below 20% by noon, the admin gets an automatic alert.

**Complaints**
Anyone can file a complaint through the public portal. It gets auto-assigned to the officer responsible for that constituency, who is notified immediately. If the complaint is not resolved within 24 hours, it escalates to the Super Admin.

---

## Notifications

The system sends automated Email and SMS notifications for:

- OTP during voter registration
- Voter approval or rejection with reason
- Candidate nomination approval or rejection
- Election day reminders to voters, candidates, and officers
- New complaint assignments to officers
- Low turnout alerts to admin
- Result declarations to candidates
- Unresolved complaint escalations after 24 hours

---

## Public Pages

These pages are accessible without any login:

- Voter registration form
- Voter status check (enter phone or National ID)
- Complaint tracking (enter Complaint ID)
- Live election results dashboard
- Candidate list by constituency

---

## Integrations

| Tool | Purpose |
|------|---------|
| Zoho Mail | All email notifications |
| Zoho SMS | OTP, reminders, alerts |
| Zoho Analytics | Advanced dashboards and heat maps |
| Zoho Sign | Digital signatures for candidate affidavits |
| Zoho Maps | Booth location display and GPS tracking |
| Zoho Flow + WhatsApp | Duty reminders and result alerts |

---

## Security

- OTP verification required for all voter registrations
- Duplicate voter detection using National ID / Aadhaar number
- Duplicate candidate check per constituency
- Full audit log capturing user, action, module, timestamp, and IP address
- Session auto-timeout after 15 minutes for all officers
- Only Super Admin can delete or modify approved records
- Forms auto-lock based on election dates and voting time windows
- All exported documents are watermarked

---

## Getting Started

**Prerequisites**
- Zoho Creator account (Professional or Enterprise plan recommended)
- Zoho Mail and SMS gateway configured
- Admin access to manage roles and permissions

**Setup Steps**

1. Log in to Zoho Creator, click "Create App" and use the Zia AI prompt to generate the base structure
2. Create your first election record and define the nomination dates, voting window, and result date
3. Add constituencies, wards, and polling booths
4. Set up user roles and assign permissions per module
5. Connect Zoho Mail, SMS, Analytics, and Flow integrations
6. Test the voter registration flow, officer check-in, and vote count submission
7. Publish the public registration page and go live

---

## Deployment Plan

| Phase | Focus | Timeline |
|-------|-------|----------|
| Phase 1 | Voter & Candidate Registration, Constituency Setup | Week 1 |
| Phase 2 | Booth Management, Officer Assignment | Week 2 |
| Phase 3 | Ballot Config, Voting Day Setup, Dashboard | Week 3 |
| Phase 4 | Complaints Module, Reports, Testing | Week 4 |
| Phase 5 | UAT, Bug Fixes, Go-Live | Week 5 |

---

## Auto-Generated ID Formats

| Record | Format |
|--------|--------|
| Voter | VTR-2024-00001 |
| Candidate | CND-2024-00001 |
| Polling Booth | BTH-2024-00001 |
| Election Officer | OFF-2024-00001 |
| Complaint | CMP-2024-00001 |

---

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Description of change'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## Support

For questions or issues, open a GitHub Issue or reach out at `your@email.com`.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
