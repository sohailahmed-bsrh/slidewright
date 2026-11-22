<div align="center">

<h1>SlideWright: Multi-Agent Presentation Studio</h1>

<img src="https://readme-typing-svg.herokuapp.com?font=Inter&weight=800&size=22&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&width=800&lines=Decoupled+Multi-Agent+AI+Orchestration;Automated+Structural+Critique+%26+Review;Visual+Slide+Layout+Synthesis;Full-Stack+TypeScript+%2B+React+Interface" alt="Typing Header" />

<p><strong>Multi-Agent Artificial Intelligence Architecture for Autonomous Presentation Design</strong></p>

<p>
  <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=nodejs,react,ts,tailwind,github&theme=dark" alt="Skills" /></a>
</p>

</div>

---

## Executive Summary

SlideWright is a multi-agent framework designed for autonomous slide presentation generation. Operating through a decoupled multi-agent loop, a specialized Slide Critic Agent inspects and refines narrative outlines, while an independent Designer Agent synthesizes presentation slides. Automated validation schemas enforce visual clarity, preventing layout regressions.

---

## Application Interface & Presentation Deck Gallery

<table align="center">
  <tr>
    <td align="center"><b>SlideWright AI Presentation Studio</b><br><sub>Main dashboard for topic prompts and presentation settings.</sub></td>
    <td align="center"><b>Critic Agent Structural Review</b><br><sub>Narrative density evaluation and pacing optimization.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/1.jpg" alt="Studio UI" width="460"/></td>
    <td align="center"><img src="screenshots/2.jpg" alt="Critic Review" width="460"/></td>
  </tr>
  <tr>
    <td align="center"><b>Designer Agent Layout Synthesis</b><br><sub>Component placement, color hierarchy, and visual balance.</sub></td>
    <td align="center"><b>Complete Presentation Deck Output</b><br><sub>Rendered presentation slides with export capabilities.</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/3.jpg" alt="Designer Layout" width="460"/></td>
    <td align="center"><img src="screenshots/4.jpg" alt="Deck Output" width="460"/></td>
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

## Author & License

- **Author**: Sohail Ahmed ([Portfolio](https://sohail.devsil.com) | [GitHub](https://github.com/sohailahmed-bsrh))
- **License**: Distributed under the MIT License.
