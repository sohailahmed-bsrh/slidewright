<div align="center">

<h1>SlideWright: Multi-Agent Presentation Studio</h1>

<img src="https://readme-typing-svg.herokuapp.com?font=Inter&weight=800&size=22&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&width=800&lines=Decoupled+Multi-Agent+AI+Orchestration;Automated+Structural+Critique+%26+Review;Visual+Slide+Layout+Synthesis;Full-Stack+TypeScript+%2B+React+Interface" alt="Typing Header" />

<p><strong>Multi-Agent Artificial Intelligence Architecture for Autonomous Presentation Design</strong></p>

<p>
  <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=nodejs,react,ts,tailwind,github&theme=dark" alt="Skills" /></a>
</p>

<p>
  <a href="#overview">Overview</a> &bull;
  <a href="#system-architecture">Architecture</a> &bull;
  <a href="#visual-showcase-gallery">Visual Gallery</a> &bull;
  <a href="#core-capabilities">Capabilities</a> &bull;
  <a href="#installation--setup">Installation</a> &bull;
  <a href="#author--contact-information">Author</a>
</p>

</div>

---
## Overview

SlideWright is a multi-agent framework designed for autonomous slide presentation generation. Operating through a decoupled multi-agent loop, a specialized Slide Critic Agent inspects and refines narrative outlines, while an independent Designer Agent synthesizes presentation slides. Automated validation schemas enforce visual clarity, preventing layout regressions.

---

## Visual Showcase Gallery

<table width="100%" align="center">
  <tr>
    <td width="50%" align="center"><b>SlideWright AI Presentation Studio</b><br><sub>Main dashboard for topic prompts and presentation settings.</sub></td>
    <td width="50%" align="center"><b>Critic Agent Structural Review</b><br><sub>Narrative density evaluation and pacing optimization.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/1.jpg" alt="Studio UI" width="460"/></td>
    <td align="center"><img src="screenshots/2.jpg" alt="Critic Review" width="460"/></td>
  </tr>
  <tr>
    <td width="50%" align="center"><b>Designer Agent Layout Synthesis</b><br><sub>Component placement, color hierarchy, and visual balance.</sub></td>
    <td width="50%" align="center"><b>Complete Presentation Deck Output</b><br><sub>Rendered presentation slides with export capabilities.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/3.jpg" alt="Designer Layout" width="460"/></td>
    <td align="center"><img src="screenshots/4.jpg" alt="Deck Output" width="460"/></td>
  </tr>
  <tr>
    <td width="50%" align="center"><b>Topic Taxonomy & Keyword Map</b><br><sub>Subject outline decomposition and conceptual clustering.</sub></td>
    <td width="50%" align="center"><b>Slide Typography & Styling Engine</b><br><sub>Font pairing, heading hierarchy, and contrast validation.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/5.jpg" alt="Taxonomy Map" width="460"/></td>
    <td align="center"><img src="screenshots/6.jpg" alt="Typography Engine" width="460"/></td>
  </tr>
  <tr>
    <td width="50%" align="center"><b>Multi-Agent Message Inspection Log</b><br><sub>Real-time communication log between Critic and Designer agents.</sub></td>
    <td width="50%" align="center"><b>Export & Slide Deck Delivery Hub</b><br><sub>PDF, HTML, and Markdown presentation bundle exports.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/7.jpg" alt="Agent Logs" width="460"/></td>
    <td align="center"><img src="screenshots/8.jpg" alt="Delivery Hub" width="460"/></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><b>SlideWright System Architecture Mockup</b><br><sub>High-level visual mock showing multi-agent interaction flow.</sub></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><img src="references/ui/slidewright_mockup.png" alt="System Mockup" width="650"/></td>
  </tr>
</table>

---

## System Architecture

```mermaid
flowchart TD
    A[User Presentation Prompt / Outline] --> B[Multi-Agent Orchestrator]
    B --> C[Slide Critic Agent: Structure & Logic Analysis]
    C -->|Evaluation & Structural Feedback| D[Designer Agent: Layout & Styling]
    D -->|Slide Specifications| E[Automated Schema & Quality Validator]
    E -->|Validation Passed| F[Rendered High-Definition Slide Deck]
    E -->|Validation Issues Detected| C
```

---

## Technology Stack

| Domain | Technologies |
| :--- | :--- |
| Frontend Interface | React, TypeScript, Tailwind CSS |
| Agent Orchestration | TypeScript Multi-Agent Architecture |
| Validation | Zod Schemas |
| Build Tooling | Vite, Node.js |

---

## Installation & Setup

```bash
# Clone the repository
git clone https://github.com/sohailahmed-bsrh/slidewright.git
cd slidewright

# Install dependencies and start
npm install
npm run dev
```
---

## Author & Contact Information

<table width="100%" align="center">
  <tr>
    <td align="center" style="padding: 20px;">
      <h3>Sohail Ahmed</h3>
      <p><strong>Full-Stack Artificial Intelligence & Computer Vision Engineer</strong></p>
      <p>
        <a href="https://sohail.devsil.com"><img src="https://img.shields.io/badge/Live_Portfolio-sohail.devsil.com-0052FF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio"/></a>
        <a href="https://github.com/sohailahmed-bsrh"><img src="https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
        <a href="https://linkedin.com/in/sohail-ahmed-dev"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
        <a href="mailto:sohail.bsrh@gmail.com"><img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
      </p>
      <p><em>Available for technical roles in Artificial Intelligence, Computer Vision, and Full-Stack Engineering.</em></p>
      <hr style="border: 0; height: 1px; background: #30363d; margin: 15px 0;">
      <small>Repository: <code>sohailahmed-bsrh/slidewright</code> &bull; Distributed under the MIT License.</small>
    </td>
  </tr>
</table>
