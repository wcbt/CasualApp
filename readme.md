
# Casual app v1.0

---

## Overview / 項目概述

CasualApp is a job coordination and broadcasting platform designed to replace inefficient, fragmented messaging groups used for managing casual hotel and catering work.

Currently, coordinators manage 30–40 separate group chats to broadcast job availability, track capacity, and handle worker attendance. This approach is error-prone, slow, and lacks transparency.

CasualApp centralizes this workflow into a single platform that enables:

- Real-time job broadcasting
- Live capacity tracking
- Fair and transparent job assignment
- Worker performance and attendance records
- Reduced operational overhead for coordinators and hotels

The initial development focuses on **Android**, **Java-based backend**, and **relational databases**, with future expansion planned for web and iOS platforms.

---

CasualApp 是一個用於管理酒店及餐飲散工工作的協調與廣播平台，旨在取代目前效率低下、分散於多個通訊群組的工作安排方式。

目前協調員往往需要同時管理 30–40 個群組，以發布工作資訊、控制人數及處理出勤紀錄，這種方式不僅耗時，亦容易出錯，缺乏透明度。

CasualApp 將所有流程集中至單一平台，提供：

- 即時工作廣播
- 即時人數名額更新
- 公平的工作分配
- 工人表現與出勤紀錄
- 大幅減少人手管理成本

第一階段將專注於 **Android 平台**、**Java 後端** 及 **關聯式資料庫**，未來再擴展至 Web 及 iOS。

---

## Core Problems Addressed / 解決的核心問題

| Problem (EN) | 問題（中文） |
|--------------|-------------|
| Jobs are hard to discover quickly | 工作資訊分散，難以及時獲取 |
| Capacity is unclear or overfilled | 名額不透明，容易超額 |
| No formal performance records | 缺乏正式表現及紀錄 |
| High manual coordination cost | 人手協調成本極高 |

---

## Core Features (MVP) / 核心功能（最小可行版本）

| Feature (EN) | 功能（中文） |
|-------------|--------------|
| Centralized job posting | 集中式工作發布 |
| Real-time slot availability | 即時名額顯示 |
| One-tap job signup | 一鍵報名 |
| Attendance & performance tracking | 出勤及表現追蹤 |
| Optional reserved slots | 可預留名額 |

---

## User Roles / 使用者角色

| Role (EN) | 角色（中文） | Description |
|---------|--------------|-------------|
| Worker | 工人 | 查看及報名工作 |
| Coordinator | 協調員 / 帶隊 | 發布工作、管理名單、標記出勤 |
| Hotel Dispatcher (future) | 酒店方（未來） | 直接發布需求 |
| Admin | 管理員 | 系統管理 |

---

## Typical Workflow / 基本流程

1. Coordinator or hotel posts a job
2. Workers view jobs in a unified feed
3. Worker taps “Join” to reserve a slot
4. Capacity updates in real time
5. Attendance and outcomes recorded after the job

1. 協調員或酒店發布工作
2. 工人於統一平台查看工作列表
3. 工人點擊報名以鎖定名額
4. 名額即時更新
5. 工作後記錄出勤及表現

---

## Attendance & Penalty System / 出勤與懲罰機制

| Outcome (EN) | 結果（中文） | Effect |
|-------------|-------------|--------|
| Completed | 正常完成 | 無影響 |
| Bad Performance | 表現欠佳 | 累積警告 |
| No Show | 缺席 | 高風險記錄 |
| Approved Substitution | 獲批代替 | 無懲罰 |

Workers with better records may receive higher priority in future job broadcasts.

表現良好的工人將於未來工作廣播中獲得更高優先權。

---

## Technology Stack / 技術架構

| Layer | Technology |
|------|------------|
| Mobile App | Android (Java, Android Studio) |
| Backend | Java (Spring Boot) |
| Database | Relational DB (PostgreSQL / MySQL) |
| Realtime Updates | WebSocket or Polling |
| Notifications | Firebase Cloud Messaging |
| Version Control | Git & GitHub |

---

## Repository Structure / 專案結構

```text
CasualApp/
├── apps/
│   ├── android/
│   ├── ios/
│   └── web/
├── backend/
├── shared/
├── design/
├── docs/
├── infra/
└── tools/
