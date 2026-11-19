# Maestro Setup

This repository is a practical guide to organizing AI-assisted work, with diagrams, setup prompts and an operating-rules example. It describes a working practice, not an app to install.

I want more useful work from AI agents, with less of my effort. The useful part is deciding who owns the outcome, what context they need, and how I will check the result.

You can use the pattern with one assistant, several agents inside one tool, or assistants from different providers. The roles and records matter more than the brands.

It can also fit a team where each person has an agent: one accountable owner per task, shared project context within the team's access rules, and decisions recorded where the next authorized person or agent can find them.

I use several tools to learn their strengths side by side and avoid relying on a single provider. Shared records make it easier to move work when one is unavailable, but that is not automatic failover. If one tool covers the work and the connections you need, one tool is enough.

## Setup, Brain, Spine

**Setup** is the whole arrangement of me, agents and tools.

**Brain** is the shared project context and knowledge: purpose, current decisions, constraints and useful sources. Each agent keeps its own memory.

**Spine** is the path a request follows: it gets an owner, moves through delivery and review, and ends with a decision or recorded result.

![Diagram titled "Maestro Setup", in three parts. SETUP: three tiles aligned over the steps below them: Accountable agents, Reviewers, and Me (human) (judgment and acceptance). SPINE: five steps left to right: Request, Accountable agent, Delivery, Reviewers + human decision, Recorded result (in the task record). A dashed coral arc labelled "Not yet" loops from the decision back to Delivery. "Accepted" sits over the arrow into Recorded result. BRAIN: a solid green layer across the full width, "Shared context: purpose, constraints, sources". Three arrows labelled "reads" rise from it into Accountable agent, Delivery, and Reviewers + human decision.](images/maestro-readme-light-v7.1.png#gh-light-mode-only)
![Diagram titled "Maestro Setup", in three parts. SETUP: three tiles aligned over the steps below them: Accountable agents, Reviewers, and Me (human) (judgment and acceptance). SPINE: five steps left to right: Request, Accountable agent, Delivery, Reviewers + human decision, Recorded result (in the task record). A dashed coral arc labelled "Not yet" loops from the decision back to Delivery. "Accepted" sits over the arrow into Recorded result. BRAIN: a solid green layer across the full width, "Shared context: purpose, constraints, sources". Three arrows labelled "reads" rise from it into Accountable agent, Delivery, and Reviewers + human decision.](images/maestro-readme-dark-v7.1.png#gh-dark-mode-only)

> **In my case:** Dot (ChatGPT) handles projects and portfolio; Muse handles personal work; Claude handles delivery; Grok Bots provide specialist help. Notion holds the Brain, Linear the tasks, and Slack the conversations. The tool names are real; the roles describe how I use them.

## The Spine

```mermaid
flowchart TD
    A["Request"] --> B["Owner"]
    B --> C["Delivery"]
    C --> D{"Review and<br/>decision"}
    D -- "Not yet" --> C
    D -- "Accepted" --> E["Recorded result"]
```

> In words: a request names an outcome you can check. It gets one owner with sources, limits and done checks. The owner returns the result, the checks they ran, and any remaining gaps. Review decides: if it isn't there yet, it goes back to delivery; if it's accepted, the result is recorded on the task record.

### One real workflow: launching the Lunar Wave website

1. **Request.** I asked for a website for Lunar Wave, my independent product and AI practice, and set the direction: a company voice, capabilities and real work, and a simple way to get in touch.
2. **Owner.** One agent was accountable for the outcome and a second built the site. The work had written done checks.
3. **Delivery.** The site went through private previews, then a public review build marked noindex.
4. **Review and decision.** The accountable agent checked the final launch package against the reviewed version (no visible change), tested navigation, links and the contact path, and confirmed that mail to the new address was received and could be answered. Agents could prepare everything, but only I could approve the launch. I approved one exact action: attach the domain, set two named web records and publish. Mail settings and nameservers were out of scope.
5. **Recorded result.** After launch, the accountable agent checked the live site over HTTPS, the redirect, the canonical address, that the live pages were indexable, the sitemap and the contact link, and confirmed that mail and nameservers were untouched. The result is recorded on the task.

**When a tool does not behave as expected.** In another project, one agent found that searches of the shared project records ignored a saved view's filters unless the filters were written into the search itself. It recorded the fix once in the shared task method. A second agent, on a different platform, later read that method and searched correctly. The knowledge moved through the shared records instead of through me.

**When something is not right.** A rollback path was defined before launch. Copy changes reported through agents still had to match my own approval. Sending and replying from the public contact address were tested before launch. Custom email authentication was not part of the launch; it stays open on the task instead of being reported as done.

## The Brain

It gives a fresh session a starting point. It is not shared memory. Each agent keeps its own memory, and access to a page is not proof that anyone read it.

- **Project reference**
  - **Holds:** Purpose, audience, current decisions and why, constraints, sources
  - **Links to:** each open task record
- **Task record**
  - **Holds:** Owner, done checks, the result, the review, the recorded decision
  - **Links to:** the project reference, and the work itself
- **The work**
  - **Holds:** The draft, the code, the tests
  - **Links to:** its task record
- **Coordination message**
  - **Holds:** A short ask, plus a link to the task record
  - **Links to:** the task record

One current home for each fact; everything else links to it. Keep passwords, keys and private personal details off these pages.

This is a setup I use in my own work, not software you can install. Each task's owner, done checks and review come from written rules the agents are asked to follow. Written rules are not technical controls. Routine work can be accepted within delegated authority; decisions I reserve still come to me. The diagram's human-decision step represents those reserved decisions, not a new approval gate for every task.

In practice, cross-agent handoffs still need checking. Sending a message does not prove another agent picked it up. I now prefer one agent to carry a project through, adding a second reviewer where it helps.

In day-to-day use, I get one consolidated brief with completed work, blockers and decisions that need me. I answer its numbered decisions, and the answers are recorded against the corresponding source items.

## Set it up yourself

Set up the whole frame, start with one real task, then refine in use. The [starter guide](docs/START-HERE.md) walks through roles, required connections, shared context, verification and real work, with copyable prompts and official resources. Adapt the separate [standard operating-rules example](docs/STANDARD-OPERATING-RULES.md) to each assistant's job and boundaries.

Use the assistants and workspace tools you already have where they support the required connections and access. You do not need a particular team of agents; plan eligibility and connector capabilities vary.

## Related work

[Maestro Spine](https://github.com/ahmadalkabra/maestro-spine) is my earlier project: rules, templates and scripts for AI-assisted work, adapted from Garry Tan's MIT-licensed gstack and gbrain. Maestro Setup doesn't build on its code.

## About

Ahmad Alkabra. Licensed under MIT. Copyright (c) 2026 Ahmad Alkabra.

[LinkedIn](https://www.linkedin.com/in/aalkabra) · X: [@ahmadalkabra](https://x.com/ahmadalkabra)

