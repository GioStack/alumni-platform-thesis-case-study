# Alumni Platform – ECE, University of Western Macedonia

[![WordPress](https://img.shields.io/badge/WordPress-21759B?logo=wordpress&logoColor=white)](https://wordpress.org)
[![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)](https://www.php.net)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com)
[![BuddyPress](https://img.shields.io/badge/BuddyPress-D84800)](https://buddypress.org)

A small social network for the graduates of the Department of Electrical and Computer Engineering: profiles, groups, chat, events and a job board in one place.

**Live:** [alumni.ece.uowm.gr](https://alumni.ece.uowm.gr) · Diploma thesis, grade **10/10**

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

## Key features

- **Profiles** with graduation year, current job, skills, LinkedIn and GitHub
- **Member directory** with search, plus topic-based groups
- **Private chat** and an activity wall with posts and comments
- **Job board** where every graduate can post openings
- **Events** as a list or calendar, with "Add to Calendar"
- **Mobile-ready**, with dark mode, translation and accessibility tools

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

```mermaid
mindmap
  root((Alumni Platform))
    Frontend
      NewsBlogger theme
      Custom CSS and JavaScript
      Responsive design
    Backend
      WordPress and PHP
      BuddyPress
      Youzify profiles
      Better Messages chat
      The Events Calendar
      Submitted Posts jobs
    Database
      MySQL
    Security and privacy
      Wordfence
      Complianz GDPR
      UpdraftPlus backups
    Extras
      Google sign-in
      GTranslate
      UserWay accessibility
      Dark mode
      Newsletter
```

<details>
<summary><b>Performance</b>: loads in 1.92 s, DebugBear score 70% (click to expand)</summary>

<br>

| DebugBear | SiteSpeed.gr |
|---|---|
| ![DebugBear results](assets/performance-debugbear.jpg) | ![SiteSpeed.gr results](assets/performance-sitespeed.jpg) |

</details>

## About this repository

This repository documents the project and **does not contain source code**. The website runs on the university's servers, which I no longer have access to. No credentials, personal data or backups are included, and member pages are not shown to protect other people's data.

## Thesis details

**Georgios Georgiadis** · Diploma in Informatics and Telecommunications Engineering<br>
University of Western Macedonia, Department of Electrical and Computer Engineering · Supervisor: Prof. Pantelis Angelidis · October 2025 · Grade 10/10
