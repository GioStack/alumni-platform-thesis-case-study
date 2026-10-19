# Alumni Platform – ECE, University of Western Macedonia

[![WordPress](https://img.shields.io/badge/WordPress-21759B?logo=wordpress&logoColor=white)](https://wordpress.org)
[![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)](https://www.php.net)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com)
[![BuddyPress](https://img.shields.io/badge/BuddyPress-D84800)](https://buddypress.org)

A small social network for the graduates of the Department of Electrical and Computer Engineering: profiles, groups, chat, events and a job board in one place.

**Live:** [alumni.ece.uowm.gr](https://alumni.ece.uowm.gr) · Diploma thesis, grade **10/10**

## Key features

- **Profiles** with graduation year, current job, skills, LinkedIn and GitHub
- **Member directory** with search, plus topic-based groups
- **Private chat** and an activity wall with posts and comments
- **Job board** where every graduate can post openings
- **Events** as a list or calendar, with "Add to Calendar"
- **Mobile-ready**, with dark mode, translation and accessibility tools

| Events | Job board |
|---|---|
| ![Events page](assets/events.jpg) | ![Job board](assets/job-board.jpg) |

## How it works

```mermaid
flowchart LR
    U["User<br/>computer or phone"] --> S["University server<br/>Apache"]
    S --> W["WordPress<br/>PHP"]
    W --> D[("MySQL<br/>database")]
    W --- T["NewsBlogger theme<br/>look and layout"]
    W --- P["Plugins<br/>BuddyPress, Youzify, etc."]
    W --- C["Custom code<br/>PHP/JS snippets, CSS"]
```

WordPress is the core. Each feature (profiles, chat, events, jobs) is a plugin, extended with custom PHP, JavaScript and CSS.

## User roles

```mermaid
flowchart LR
    V(["Visitor"]) -- "signs up<br/>email or Google" --> G(["Graduate"])
    A(["Administrator"]) -. "manages" .-> G

    V --> V1["Browse events,<br/>jobs and MSc news"]

    G --> G1["Profile and skills"]
    G --> G2["Groups and chat"]
    G --> G3["Post job openings"]
    G --> G4["Export or delete<br/>own data"]

    A --> A1["Content and members"]
    A --> A2["Security and privacy"]

    classDef visitor fill:#64748b,stroke:#475569,color:#fff
    classDef grad fill:#2563eb,stroke:#1d4ed8,color:#fff
    classDef admin fill:#d97706,stroke:#b45309,color:#fff
    class V visitor
    class G grad
    class A admin
```

## Technologies

| Layer | Tools |
|---|---|
| **Frontend** | ![NewsBlogger theme](https://img.shields.io/badge/NewsBlogger_theme-6F42C1) ![CSS](https://img.shields.io/badge/CSS-6F42C1) ![JavaScript](https://img.shields.io/badge/JavaScript-6F42C1?logo=javascript&logoColor=white) ![Responsive design](https://img.shields.io/badge/Responsive_design-6F42C1) |
| **Backend** | ![WordPress](https://img.shields.io/badge/WordPress-21759B?logo=wordpress&logoColor=white) ![PHP](https://img.shields.io/badge/PHP-21759B?logo=php&logoColor=white) ![BuddyPress](https://img.shields.io/badge/BuddyPress-21759B) ![Youzify](https://img.shields.io/badge/Youzify-21759B) ![Better Messages](https://img.shields.io/badge/Better_Messages-21759B) ![The Events Calendar](https://img.shields.io/badge/The_Events_Calendar-21759B) ![Submitted Posts](https://img.shields.io/badge/Submitted_Posts-21759B) ![WPCode Lite](https://img.shields.io/badge/WPCode_Lite-21759B) |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) |
| **Security & privacy** | ![Wordfence](https://img.shields.io/badge/Wordfence-2E7D32) ![Complianz GDPR](https://img.shields.io/badge/Complianz_GDPR-2E7D32) ![UpdraftPlus backups](https://img.shields.io/badge/UpdraftPlus_backups-2E7D32) |
| **Extras** | ![Google sign-in](https://img.shields.io/badge/Google_sign--in-6B7280?logo=google&logoColor=white) ![GTranslate](https://img.shields.io/badge/GTranslate-6B7280) ![UserWay](https://img.shields.io/badge/UserWay_accessibility-6B7280) ![Dark mode](https://img.shields.io/badge/Dark_mode-6B7280) ![Newsletter](https://img.shields.io/badge/Noptin_newsletter-6B7280) ![WP Mail SMTP](https://img.shields.io/badge/WP_Mail_SMTP-6B7280) |

## Performance

The live site loads in **1.92 s** (SiteSpeed.gr) and scores **70%** on DebugBear.

| DebugBear | SiteSpeed.gr |
|---|---|
| ![DebugBear results](assets/performance-debugbear.jpg) | ![SiteSpeed.gr results](assets/performance-sitespeed.jpg) |

## About this repository

This repository documents the project and **does not contain source code**. The website runs on the university's servers, which I no longer have access to. No credentials, personal data or backups are included, and member pages are not shown to protect other people's data.

## Thesis details

**Georgios Georgiadis** · Diploma in Informatics and Telecommunications Engineering<br>
University of Western Macedonia, Department of Electrical and Computer Engineering · Supervisor: Prof. Pantelis Angelidis · October 2025 · Grade 10/10
