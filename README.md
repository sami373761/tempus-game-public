<div align="center">

  <a href="https://tempusplay.com" target="_blank" rel="noopener noreferrer">
    <img src="icon.svg" alt="Tempus Logo" width="96" height="96" />
  </a>

  # TEMPUS

  **Explore world history across a 4.54-billion-year timeline.**  
  *Pinpoint dates, compare eras, and compete in real-time head-to-head chronological duels.*

  <br />

  <!-- PRIMARY CTA BUTTON -->
  <a href="https://tempusplay.com" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/▶_PLAY_TEMPUS_NOW-tempusplay.com-f5a623?style=for-the-badge&labelColor=111111&logoColor=white" alt="Play Tempus Now at tempusplay.com" height="46" />
  </a>

  <p align="center">
    <a href="https://tempusplay.com/guess" target="_blank" rel="noopener noreferrer"><b>🎯 Play /guess</b></a> &nbsp;•&nbsp;
    <a href="https://tempusplay.com/compare" target="_blank" rel="noopener noreferrer"><b>⚖️ Play /compare</b></a> &nbsp;•&nbsp;
    <a href="https://tempusplay.com/versus" target="_blank" rel="noopener noreferrer"><b>⚔️ Play /versus</b></a>
  </p>

  <br />

  <!-- TECH STACK BADGES -->
  <p align="center">
    <img src="https://img.shields.io/badge/Next.js-App_Router-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js" />
    <img src="https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
    <img src="https://img.shields.io/badge/PostgreSQL-Supabase-3ECF8E?style=flat-square&logo=postgresql&logoColor=black" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Cloudflare-Edge_CDN-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare" />
  </p>

</div>

---

## 🎮 Game Modes & Features

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🎯 Solo Modes & Daily Challenges</h3>
      <ul>
        <li><b>Date Guessing (<a href="https://tempusplay.com/guess" target="_blank" rel="noopener noreferrer"><code>/guess</code></a>):</b> Place historical events on a zero-scroll (<code>100dvh</code>) timeline stage. Graded dynamically by relative error against the event's age.</li>
        <li><b>Comparison (<a href="https://tempusplay.com/compare" target="_blank" rel="noopener noreferrer"><code>/compare</code></a>):</b> High-tempo chronological ordering between paired historical events.</li>
        <li><b>Daily & Thematic Categories:</b> Curated subject categories with tailored difficulty bands and daily challenges.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>⚔️ Head-to-Head (<a href="https://tempusplay.com/versus" target="_blank" rel="noopener noreferrer"><code>/versus</code></a>)</h3>
      <ul>
        <li><b>Online Matchmaking:</b> Ranked public duels staking <b>Chrono Rating (KP)</b>.</li>
        <li><b>Friend Rooms:</b> Instant private lobbies shareable via invite links or QR codes, open to both registered players and guests.</li>
        <li><b>Real-Time Sync:</b> Low-latency round synchronization for live competitive play.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🏆 Progression & Economy</h3>
      <ul>
        <li><b>Tempus Points (TP):</b> Earned across solo sets based on chronological accuracy and streaks.</li>
        <li><b>Chrono Rating (KP):</b> Competitive ELO-style rating system for ranked head-to-head matches.</li>
        <li><b>Metal Badge Ladder:</b> 6-tier progression unlocked automatically through gameplay milestones.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🌍 Multilingual By Design</h3>
      <ul>
        <li><b>5 Native Locales:</b> Full support for <b>English, Turkish, German, French, and Spanish</b> (<code>en</code>, <code>tr</code>, <code>de</code>, <code>fr</code>, <code>es</code>).</li>
        <li><b>Localized Content Engine:</b> Seamless language switching across historical event titles, descriptions, and UI.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🏗️ System Overview

Tempus uses a server-authoritative architecture where game state, grading, and competitive matchmaking are validated entirely on the backend before results reach the client.

```mermaid
graph LR
    Client["Web Client\n(Next.js / React)"]
    Edge["Edge CDN\n(Media Delivery)"]
    App["Application Layer\n(Game Engine & Auth)"]
    DB[("Database\n(State & Chronology)")]

    Client <-->|Interactive UI| App
    Client -->|Optimized Media| Edge
    App <-->|Authoritative State| DB

