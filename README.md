<div align="center">

<h1>SlideWright: Multi-Agent Presentation Studio</h1>

<img src="https://readme-typing-svg.herokuapp.com?font=Inter&weight=800&size=22&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&width=800&lines=Decoupled+Multi-Agent+AI+Orchestration;Automated+Structural+Critique+%26+Review;Visual+Slide+Layout+Synthesis;Full-Stack+TypeScript+%2B+React+Interface" alt="Typing Header" />

<p><strong>Multi-Agent Artificial Intelligence Architecture for Autonomous Presentation Design</strong></p>

<p>
  <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=nodejs,react,ts,tailwind,github&theme=dark" alt="Skills" /></a>
</p>

<p>
  <a href="#overview">Overview</a> &bull;
  <a href="#purpose--problem-statement">Purpose</a> &bull;
  <a href="#real-world-industry-applications">Use Cases</a> &bull;
  <a href="#step-by-step-engineering-walkthrough">How It Was Built</a> &bull;
  <a href="#system-architecture">Architecture</a> &bull;
  <a href="#visual-showcase-gallery">Visual Gallery</a> &bull;
  <a href="#technology-stack-matrix">Tech Stack</a> &bull;
  <a href="#installation--setup">Installation</a> &bull;
  <a href="#author--contact-information">Author</a>
</p>

</div>

---
## Overview

SlideWright is a multi-agent framework designed for autonomous slide presentation generation. Operating through a decoupled multi-agent loop, a specialized Slide Critic Agent inspects and refines narrative outlines, while an independent Designer Agent synthesizes presentation slides. Automated validation schemas enforce visual clarity, preventing layout regressions.

---

## Purpose & Problem Statement

### The Problem
Single-prompt LLM presentation generators produce poor results: text is overcrowded, narrative pacing is disjointed, and visual formatting is inconsistent. Without a multi-agent separation of concerns (criticism vs design), generative models try to do everything at once, producing mediocre slide decks that require extensive manual reworking.

### The Engineering Purpose
To build a decoupled multi-agent architecture where distinct specialized agents collaborate through a strict review loop: a Critic Agent that analyzes argument flow and slide density, and a Designer Agent that translates structured critique into balanced presentation components with automated validation.

---

## Real-World Industry Applications

- **Corporate Strategy & Board Briefings**: Synthesizing quarterly financial and operational reports into crisp executive slide decks.
- **Technical Keynotes & Architecture Overviews**: Translating complex system design documents into clean visual diagrams and talking points.
- **Consulting Pitch Decks**: Rapidly producing structured client pitch presentations based on initial discovery interview transcripts.
- **Academic & Research Seminars**: Converting dense technical research papers into structured conference presentation slides.

---

## Step-by-Step Engineering Walkthrough (How It Was Built)

### Step 1: User Topic & Parameter Ingestion
The user provides a high-level topic, target audience profile, and desired slide count via the React frontend. The orchestrator initializes an agent session context.

### Step 2: Slide Critic Agent (Narrative Analysis)
The Critic Agent (`agents/critic/run.ts`) ingests the prompt and derives an outline. It analyzes the narrative arc:
- Does each slide convey a single core thesis?
- Is information density balanced?
- Is the pacing appropriate for the target audience?
The Critic outputs structured structural feedback and actionable revision instructions.

### Step 3: Designer Agent (Visual Layout Synthesis)
The Designer Agent (`agents/designer/run.ts`) consumes the Critic's approved outline. It maps abstract concepts into concrete slide components: hero headers, two-column metric comparisons, quote blocks, process flows, and key takeaways.

### Step 4: Schema Validation Subsystem
Before final compilation, slide components are passed through strict validation schemas using **Zod** (`agents/designer/validate.ts`). The validator checks word count limits, color contrast compliance, and grid layout integrity. If validation fails, the specifications are routed back to the Designer Agent for immediate self-correction.

### Step 5: Multi-Format Presentation Compilation
Approved slide objects are compiled into interactive React slide decks, printable PDF documents, or raw Marp-compatible Markdown bundles.

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

## Technology Stack Matrix

| Layer | Technologies | Version / Role | Engineering Purpose |
| :--- | :--- | :--- | :--- |
| Agent Orchestration | TypeScript Multi-Agent Engine | Node.js 20.x | Decoupled agent communication and state management |
| LLM Gateway | OpenRouter API Client | Latest | Multi-model routing between reasoning and creative LLMs |
| Schema Validation | Zod | 3.22+ | Type-safe JSON schema enforcement and layout validation |
| Frontend UI | React 18, Vite | 18.2 / 5.0+ | Reactive presentation canvas and agent message inspector |
| Styling | Tailwind CSS | 3.4+ | Modular typography, dark mode, and grid layouts |

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

<table width="100%">
  <tr>
    <td width="150" align="center" valign="middle">
      <img src="https://avatars.githubusercontent.com/u/231165170?v=4" width="120" style="border-radius: 50%;" alt="Sohail Ahmed"/>
    </td>
    <td>
      <h3>Sohail Ahmed</h3>
      <p><strong>Senior Software Engineer & AI Systems Architect</strong></p>
      <p>Specializing in Full-Stack AI Application Development, Computer Vision, Deep Learning Pipelines, and Scalable Automation Architectures.</p>
      <p>
        <a href="https://sohail.devsil.com"><strong>Portfolio Website</strong></a> | 
        <a href="https://github.com/sohailahmed-bsrh"><strong>GitHub Profile</strong></a> | 
        <a href="https://www.linkedin.com/in/sohail-ahmed-devsil/"><strong>LinkedIn</strong></a> | 
        <a href="https://www.kaggle.com/sohail2411126"><strong>Kaggle</strong></a> | 
        <a href="https://x.com/ahmed241126"><strong>Twitter/X</strong></a> | 
        <a href="mailto:se906403@gmail.com"><strong>Email Contact</strong></a>
      </p>
    </td>
  </tr>
</table>
