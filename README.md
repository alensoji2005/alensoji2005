<!-- HERO SECTION -->
<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="art/header-dark.png">
    <img alt="Alen Soji Banner" src="art/header-light.png" width="100%">
  </picture>

  <br/><br/>

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=7AA2F7&center=true&vCenter=true&width=500&lines=Hi+there,+I'm+Alen+Soji!;Full-Stack+Developer;Building+scalable+web+apps." alt="Typing SVG" />

  <p>
    <a href="https://linkedin.com/in/alen-soji"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="mailto:alensoji2005@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
    <a href="https://github.com/alensoji2005?tab=repositories"><img src="https://img.shields.io/badge/Projects-181717?style=flat-square&logo=github&logoColor=white" alt="Repos" /></a>
  </p>

</div>

---

### 🚀 Featured Projects

<table width="100%" align="center">
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">
        <a href="https://github.com/alensoji2005/Saute-Bot">🍳 Saute-Bot</a>
      </h3>
      <p align="left">Automated bot service designed for streamlined workflow execution and tasks.</p>
      <p align="left">
        <img src="https://img.shields.io/github/stars/alensoji2005/Saute-Bot?style=flat-square&color=7aa2f7" alt="Stars" />
        <img src="https://img.shields.io/github/repo-size/alensoji2005/Saute-Bot?style=flat-square&color=bb9af7" alt="Repo Size" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">
        <a href="https://github.com/alensoji2005/tenderai">🤖 tenderai</a>
      </h3>
      <p align="left">AI-driven platform for parsing, analyzing, and managing tender opportunities.</p>
      <p align="left">
        <img src="https://img.shields.io/github/stars/alensoji2005/tenderai?style=flat-square&color=7aa2f7" alt="Stars" />
        <img src="https://img.shields.io/github/repo-size/alensoji2005/tenderai?style=flat-square&color=bb9af7" alt="Repo Size" />
      </p>
    </td>
  </tr>
</table>

<div align="center">
  <img src="https://play.pokemonshowdown.com/sprites/gen5ani/charizard-megax.gif" alt="Charizard Companion" width="60px" />
  <br/>
  <sub><b>Companion:</b> Charizard (Lvl. 51)</sub>
</div>
---

### 🛠️ Architecture & Tech Stack

```mermaid
flowchart LR
    subgraph Client["Frontend Layer"]
        direction TB
        UI[Next.js / React]
        Style[Tailwind CSS]
        UI --- Style
    end

    subgraph Core["Backend & Services"]
        direction TB
        Gateway[API Gateway / Node.js]
        Cache[(Redis Cache)]
        DB[(PostgreSQL / Supabase)]
        Gateway -->|Query / Mutate| DB
        Gateway -->|Cache Session| Cache
    end

    subgraph Ops["Deployment & CI/CD"]
        direction TB
        Docker[Docker Containers]
        Actions[GitHub Actions]
        Docker --- Actions
    end

    Client -->|REST / GraphQL| Core
    Core -->|Auto Deploy| Ops

    %% Visual Styling
    style Client fill:#1e1e2e,stroke:#89b4fa,stroke-width:2px,color:#cdd6f4
    style Core fill:#181825,stroke:#a6e3a1,stroke-width:2px,color:#cdd6f4
    style Ops fill:#11111b,stroke:#fab387,stroke-width:2px,color:#cdd6f4
