# Committee Briefing

2 March 2026

**Purpose:** This briefing covers the core proposal and the first three decisions we need to land to start work on the Green AI Practitioner course. The briefing is all you need to get started. The companion documents are there when you're ready to go deeper.


## Why You're Reading This

To get us started on development of the Green AI Practitioner course, I'm sharing documents based on our discussions in regards to the course.

The full proposal lives across three companion documents — the Course Initiation, the Course Outline, and the Content Audit. This briefing is the short version. Read it first. Bring questions.


## The Problem We're Solving

AI has a significant and growing environmental impact. Practitioners building AI systems — developers, engineers, architects — make decisions every day that determine how large that impact is. Most of them don't know how to measure it, and they have nowhere to go to learn how in a way that is practical, role-specific, and grounded in something authoritative.

The SCI for AI specification was ratified in December 2025. It gives us the measurement framework. What we don't yet have is the course that translates it into actionable guidance for the people who actually build AI systems.

That's the gap this course closes.

# What We're Proposing

A course called the **Green AI Practitioner**. It has two layers:

<img width="1600" height="840" alt="course-layers" src="https://github.com/user-attachments/assets/f7e21855-9cb4-450f-b7ad-fbad57cd9df8" />

## Layer 1: Foundation module (mandatory, all learners)

What Green AI is (and is not); the AI lifecycle; the three-pillar measurement framework (carbon, energy, water); the consumer/provider lens; why carbon is the starting point; how the GSF spec family is designed to grow. Expands on the GSF position paper for a practitioner audience.   

## Layer 2: Persona modules (self-selected by role)

After the Foundation, learners choose the module for their role. We're initially proposing modules for: Application Developer, Infrastructure & Operations, ML/AI Engineer, and Architect/System Designer. This is the starting set — as the course matures and the community grows, we expect the range of persona modules to expand well beyond these. 

Each module goes deep on the decisions that specific role actually makes, grounded in the SCI for AI spec. Each module is made up of submodules — short, completable video units of 3–5 minutes, each with one learning objective and a quiz. Submodules are built from Knowledge Units: structured, citable content artifacts that are the source of truth for both the video scripts and the AI rulesets we publish alongside the course.

## Built For Humans And AI

This course is targeted at human learners today — but we're designing it with the near future in mind. AI coding assistants, agentic tools, and AI pair programmers are already embedded in how software gets built. Within the lifespan of this course, AI systems will be as important an audience as the humans we're building for now. We're structuring every piece of content as a Knowledge Unit first — a precise, citable record of one principle or decision. That Knowledge Unit gets rendered as a video script for human learners today, and as a structured ruleset that AI systems can consume directly tomorrow. One knowledge base. Multiple audiences. Built to last.

## The MVP

The MVP is deliberately small: the Foundation module and a first Application Developer module, with a small number of submodules — one or more, to be agreed by the committee as part of the authorship planning. Once the MVP is live, we ship the next submodule, then the next.

We're proposing Application Developer first because it's where the impact is most direct, the audience is largest, and the SCI for AI spec gives us everything we need to build it now. We don't need to wait for SEE for AI or SWE for AI to ship the first round of content.

The course is designed so that energy and water submodules slot into the existing structure once those specs are ratified — no rebuild required.

## How It Gets Built

This is a volunteer-led effort. The authorship model is designed around that reality.

* A content lead takes ownership of a submodule outline
* Volunteers author Knowledge Units — one at a time, each small enough to write in a lunch break
* An SME reviewer signs off on each Knowledge Unit before any rendering begins
* Claude is then used to derive the rendered outputs — the video script for human learners and the structured ruleset for AI systems — from the approved Knowledge Units
* GSF staff and the content lead review Claude's output, and GSF staff manage publication

**The critical gate:** no rendering begins until the Knowledge Units are SME-approved. Once they are, Claude converts them into the rendered outputs — the video script and the AI ruleset. Humans author the source of truth. AI does the conversion. When the spec evolves, we update the Knowledge Units and re-derive everything from there.

The full nine-phase authorship flow is in the Course Initiation document if you want the detail.

# The Three Decisions

These are the decisions that need to be taken first. Everything else — module scope, specific Knowledge Units, timeline — follows from these.

## 1: Course Structure

Do we approve the two-layer model (Foundation module plus persona modules) as the architecture for the Green AI Practitioner course?

## 2: Persona Prioritisation

Do we confirm Application Developer as the first persona module to build, ahead of Infrastructure & Operations, ML/AI Engineer, and Architect/System Designer?

## 3: Authorship Model

Do we approve the Knowledge Unit authorship model? Humans author and SME-approve each Knowledge Unit; Claude then derives the rendered outputs (video script and AI ruleset) from those approved artifacts.

# The Companion Documents

If you want to go deeper, three documents have the full detail:

* Course Initiation — the full proposal. Problem statement, course architecture, authorship flow, persona prioritisation rationale, Knowledge Unit schema, timeline, and all 14 decisions the committee will need to make over the life of this project.
* Course Outline — the one-page description of the course: title, audience, learning outcomes, structure, success measure. This will become the public-facing description once approved.
* Content Audit — the living document tracking what source material exists, what it covers, and where the gaps are that need SME input before we can write content.
