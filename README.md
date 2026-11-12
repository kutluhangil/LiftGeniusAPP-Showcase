<div align="center">

<img src="docs/media/hero.svg" alt="LiftGenius showcase — the trainer CRM on iOS and Android side by side" width="100%">

<p>
  <img alt="iOS" src="https://img.shields.io/badge/iOS%2026-SwiftUI-ff8a3d?style=for-the-badge&labelColor=08060a">
  <img alt="Android" src="https://img.shields.io/badge/Android-Jetpack%20Compose-ff4f9a?style=for-the-badge&labelColor=08060a">
  <img alt="Supabase" src="https://img.shields.io/badge/backend-Supabase-8ab4ff?style=for-the-badge&labelColor=08060a">
  <img alt="Languages" src="https://img.shields.io/badge/UI-TR%20%2F%20EN-ff8a3d?style=for-the-badge&labelColor=08060a">
</p>

<p><em>Clients, packages, sessions, AI plans and cash flow for personal trainers and studios.<br>
This repository is the public showcase; the source code is kept private.</em></p>

<table>
  <tr>
    <td width="33%"><img src="docs/screenshots/01_dashboard.png" alt="Dashboard"></td>
    <td width="33%"><img src="docs/screenshots/02_musteriler.png" alt="Clients"></td>
    <td width="33%"><img src="docs/screenshots/03_detay.png" alt="Client detail"></td>
  </tr>
  <tr>
    <td width="33%"><img src="docs/screenshots/04_takvim.png" alt="Calendar"></td>
    <td width="33%"><img src="docs/screenshots/05_profil.png" alt="Profile"></td>
    <td width="33%"><img src="docs/screenshots/06_upgrade.png" alt="Upgrade"></td>
  </tr>
</table>

</div>

<img src="docs/media/divider.svg" width="100%" alt="">

## What it is

LiftGenius is a mobile CRM for personal trainers and gym owners, designed in a dark-first *Obsidian Glass* language. It runs the whole business from one place: clients and packages, sessions with live timers, AI-generated workout and nutrition plans, and a clear view of what has been paid and what is still owed. Owners can run a multi-trainer salon from the same app.

Everything is bilingual (TR / EN), syncs through Supabase and keeps an on-device cache so the app stays fast between fetches.

<img src="docs/media/divider.svg" width="100%" alt="">

## Highlights

| | |
|---|---|
| **Live dashboard** | Revenue, active clients, today's sessions, expiring packages and overdue payments. |
| **Client CRM** | Goals, status, contact details, progress and personal records per client. |
| **Sessions** | A month calendar and a Dynamic Island / Live Activity session timer. |
| **AI plans** | Workout and nutrition plans tailored by Gemini, exportable as PDF. |
| **Finance** | Collected vs pending, payment methods and a six-month revenue chart. |
| **Reminders** | Pre-filled payment reminders via WhatsApp, SMS or a local notification. |
| **Widgets** | *Today's Sessions* and *Weekly Pulse* on the home screen. |
| **Team** | An owner role that manages several trainers and filters by trainer. |

<img src="docs/media/divider.svg" width="100%" alt="">

## Two native apps, one backend

| | iOS | Android |
|---|---|---|
| **UI** | SwiftUI with a Liquid Glass design system | Jetpack Compose · Material 3 |
| **Architecture** | Services over Supabase with an on-device cache | MVVM, repositories, Hilt, Coroutines + Flow |
| **Live session** | Live Activity in the Dynamic Island and on the Lock Screen | Ongoing notification |
| **Widgets** | *Today's Sessions* · *Weekly Pulse* | Home-screen widget |
| **Sign-in** | Email, Google, Apple | Email, Google (Credential Manager) |
| **Reports** | A4 PDF templates through the share sheet | Canvas-drawn PDF export |
| **AI plans** | Gemini | Gemini |
| **Languages** | Turkish and English | Turkish and English |

Both apps share one Supabase project with row-level security, and the same models, so a trainer can switch devices without exporting anything. Deleting an account removes the user's own data on both platforms through one database function.

<img src="docs/media/divider.svg" width="100%" alt="">

## The screens above

| Screen | Shows |
|---|---|
| Dashboard | Greeting, monthly revenue, active clients, today's sessions, expiring packages, overdue payments |
| Clients | The roster with status and package state |
| Client detail | Goals, measurements, progress and personal records |
| Calendar | The month grid and the day's sessions |
| Profile | The trainer, the salon and settings |
| Upgrade | What Pro adds |

<img src="docs/media/divider.svg" width="100%" alt="">

## Türkçe özet

**LiftGenius**, kişisel antrenörler ve spor salonu sahipleri için koyu, cam efektli bir tasarımla hazırlanmış mobil CRM uygulaması. Müşteriler, paketler, seanslar, yapay zekâ ile antrenman ve beslenme planları ve nakit akışı tek ekranda. Bu depo uygulamanın vitrinidir: ekran görüntüleri ve özellikler burada, kaynak kod gizli tutuluyor.

<div align="center">
<br>
<a href="https://github.com/kutluhangil"><img src="docs/media/signature.svg" width="100%" alt="Built by kutluhangil"></a>
<sub>Showcase only · native iOS (SwiftUI) and Android (Kotlin) apps on a shared Supabase backend · figures in the banner are examples.</sub>
</div>
