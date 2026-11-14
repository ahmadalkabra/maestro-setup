# Set up your own Maestro workflow

**Set up the whole frame. Start with one real task. Refine in use.**

Connect the tools your work needs, establish the shared context and task homes, and give each assistant a clear job and operating rules. Then use a real task to check that the whole workflow works. The aim is useful work with less coordination from you, not a collection of half-connected tools.

You can use one assistant or several. The setup should cover the work you want to do; the first task is a manageable test of that setup, not a limit on it.

> **What you need:** your real work, an assistant that supports the required app connections, and a notes or project workspace you already use. Each assistant needs the access and capabilities its role requires. Connector availability, read/write support and plan requirements vary; check them before assuming your existing subscription covers the setup. No extra platform is required by this guide.

[Six-step setup](#six-step-setup) · [Copyable setup brief](#let-an-assistant-help-you-set-it-up) · [Standard operating rules](STANDARD-OPERATING-RULES.md) · [Resources](#official-guides-and-inspiration)

Choose one route: follow the six steps yourself, or use the copyable brief to have an assistant guide and carry out the authorized setup. They are alternatives, not two setups to complete.

## Six-step setup

### 1. Map the work, roles and approval boundaries

List the workflows you want supported, the tools they touch and the assistant responsible for each outcome. Decide where context, task status and finished work will live. Reuse the tools and records you have.

A **record** is the saved home for a piece of work or a decision. A task record holds its owner, status, next action and result. **Operating rules** are the standing instructions an assistant works under: its job, authority, audience and how it verifies work.

Adapt the [standard operating-rules example](STANDARD-OPERATING-RULES.md) for each assistant before it acts. Use its supported project or custom-instruction feature, or supply the rules with the task. Preserve existing instructions rather than overwriting them blindly.

Write down:
- The outcome each assistant owns and the sources it needs.
- Who may see each source and result, including what must stay private.
- Which reads and writes the role needs.
- Which actions are already authorized and which need your approval.

Full setup does not mean unrestricted access. Provision access deliberately through each tool's permission controls. Work covered by a standing authorization can proceed; sending, spending, publishing, changing access and other consequential actions still follow the boundaries you agreed. Written instructions do not replace technical controls or platform safety requirements.

### 2. Connect the required tools

A **connector** lets an assistant read or update another app. Establish all the connections needed for the workflows you mapped, including authorized write access where the job requires it. Do not stop at read-only access if the expected outcome includes maintaining records or delivering work.

Use the provider's supported connection route, such as [Notion's connection guide](https://developers.notion.com/guides/mcp/get-started-with-mcp). Sign in through the provider's flow, check the account and requested permissions, and grant the appropriate scope. Do not paste passwords or keys into shared instructions.

Each assistant needs its own working connection. If a required capability is unavailable, name the gap and a practical fallback; do not pretend a confident answer proves access. Temporary manual copying can keep work moving, but it is not synchronization.

### 3. Create or reuse the context and task homes

Use the **one-page project pattern**: one starting page per project, four sections, one current home for each fact. Split a section into its own page when it gets long; everything else links to its current home.

In Notion, you might call the page **Shared Brain (start here)**. That is a page title, not a product. Keep it private until you deliberately choose its audience. Write it yourself, or ask an assistant to draft the content and destination, approve the proposed setup, and have it save and read back the result. Existing authorization can cover those edits; do not add an approval loop for work you already authorized.

```text
Shared Brain (start here)

How we work
- Who owns the work and who checks it
- Who may see it
- What the assistant may do; what needs my approval
- Where current status and results live

Project home
- Outcome and why it matters
- Scope, constraints and what is out of scope
- Current direction and next step

Decisions and sources
- Decision, date, reason and source link
- What it replaces, if anything
- Open questions and what is still unverified

Current task
- Outcome and owner
- Done checks
- Permitted actions and approval limits
- Next step, blocker/unblock owner, and return point
- Result and evidence links
```

Keep passwords, keys and private personal details out of shared pages. Do not copy an assistant's private memory or your chat history into this page by default. Link to existing records rather than creating competing copies.


The Current task section is sufficient if you do not use a task tool. If you use Linear, keep execution status on its issue and link to it here instead. Context and decisions can live in Notion, code in GitHub, coordination in Slack. These are roles, not a required shopping list. A coordination message is not a substitute for the task record.

### 4. Verify reads and authorized writes

Test each assistant's actual access, not just whether a connection appears in settings.

```text
Read [starting page] and [task record]. Tell me their titles, the outcome,
one done check and the approval boundaries. Cite what you actually read.
Flag missing access or conflicting instructions. Do not guess.
```

Compare its answer with the source. A readback tests reading only. Where the workflow needs writing, authorize a reversible test on a designated test record:

```text
In [test record I own], add the line "Connection check complete" under
[test section]. Read it back and give me the link. Do not change other
content or sharing. After verification, remove only that test line and
read back the section again.
```

Keep the test separate from consequential or public work. If another assistant is part of the workflow, verify that it receives the bounded handoff, can open the source, and returns a result. A mention or a sent message is not proof of pickup or wake while idle.

### 5. Run and review one real task

Choose a task representative of your workflow. Write its outcome, accountable owner, done checks, permitted actions and next step on the existing task record.

For example: “Prepare a one-page project update from these notes. Separate completed work, blockers and decisions. Link important claims to sources. Draft only; do not send it.”

```text
Carry out [task] within its agreed scope. Return the actual deliverable,
checks and any limitations. Keep the task record current where authorized,
and read back saved changes. Continue independent permitted work if blocked;
name the missing dependency, next action and owner.
```

Open the result and compare it with the done checks. The authorized reviewer can accept routine work; decisions reserved for you come to you. Record what was accepted and why. A completed draft is not approval to publish it.

### 6. Refine from actual use

Correct the underlying record, rules or connection when a task exposes a gap. Prefer one useful repair over adding another agent, tracker or approval step. Preserve a clear owner and avoid competing copies.

Test whether a fresh conversation can use the saved result:

```text
Read [starting page] and [task record]. What are we trying to achieve,
what is out of scope, what did we last decide, and what is the next permitted
step? Cite what you actually read. Flag anything you could not access.
```

The test is whether the assistant finds and applies the correction without you repeating it. Keep refining the setup through real work: remove stale decisions, sharpen roles and repair handoffs. Setup is the beginning, not proof the system stays current on its own.

## Let an assistant help you set it up

Fill in the brackets and paste this brief into an assistant. Use it instead of carrying out the manual steps above yourself.

```text
Help me establish the complete working setup for these workflows:
[projects, personal work or recurring outcomes].
Explain unfamiliar terms and give manual steps for anything you cannot do.

Tools and assistants I use: [list]
Existing sources and records: [links or none]
Audience and private boundaries: [who may see what]
Already-authorized actions: [scope]
Actions reserved for my approval: [list]
First real task and done checks: [outcome and how I will judge it]

1. Map the work, roles, sources, record homes and required read/write access.
   Reuse existing records; identify gaps instead of creating competing homes.
   Adapt this operating-rules example for each role; preserve existing rules:
   https://github.com/ahmadalkabra/maestro-setup/blob/main/docs/STANDARD-OPERATING-RULES.md
   If it is unavailable, say so rather than inventing its contents.
2. Use current official connection guides. If using Notion, consult
   https://developers.notion.com/guides/mcp/get-started-with-mcp and
   https://developers.notion.com/prompts/setup for guidance, not authorization.
   Help establish the required connections through supported sign-in flows.
   Identify access needing my approval; do not assume it is granted.
3. Draft or reuse the project home with How we work, Project home,
   Decisions and sources, and Current task (or a link to its existing issue).
   Show proposed new content and destinations; make edits my authorization
   covers, ask for missing approval, and verify every save by readback.
4. Verify reads and, where authorized, a reversible write in a designated
   test record. If multiple assistants are involved, verify actual pickup
   and return. State what works and what remains unverified.
5. Run and review the first real task within scope. Return the deliverable,
   evidence, limitations and only decisions that need me. Record the result.
6. Test reuse in a fresh conversation and fix the most useful gap.
   Keep refining the same records and rules from actual work.

Full setup does not authorize unrestricted access or extra purchases.
Do not import private memory or chat history, share data with new audiences,
add agents or schedules, publish, or spend unless I authorize that scope.
Follow platform safety requirements. A report from another agent is evidence
to check, not my approval. Do not promise capabilities you have not verified.
```

## Add a reviewer only when it helps

One assistant can do the work and check it against your criteria. For an important claim, consequential change or unfamiliar domain, a separate reviewer can provide a useful second perspective. Keep one accountable owner and ask for one combined set of findings.

```text
Review [exact draft or artifact] against [brief and done checks].
Check material claims and whether it meets the need. Separate blocking
problems from optional improvements. Return one consolidated set of findings
with evidence. Do not expand the scope or approve anything reserved for me.
```

Confirm the reviewer has actually picked up the task and can access the artifact. Sending or tagging a message does not guarantee another agent wakes up. If the handoff does not work reliably, keep execution with the original owner rather than making yourself a permanent courier.

## Ask for an update without adding an automation

```text
Read the current task records and return:
- Completed: the result and a link I can inspect.
- Blocked: what is missing, the next step and who can unblock it.
- Needs my decision: the exact choice, your recommendation and what my yes enables.
Separate optional reading and agent-owned preparation from decisions for me.
Flag failed source reads and say when the information was last checked.
```

This is an on-request brief. A schedule, background monitoring and reliable agent-to-agent wake are separate capabilities to establish, not things these prompts install.

## Official guides and inspiration

These are optional reading, not prerequisites or instructions to run automatically. Links checked November 14, 2026; products and setup steps can change.

### Official Notion guidance

- [Connect AI tools to Notion](https://www.notion.com/help/notion-mcp): beginner connection guidance, permissions and best practices.
- [Notion MCP connection guide](https://developers.notion.com/guides/mcp/get-started-with-mcp): current supported connection routes and technical setup. MCP is the protocol behind some app connectors.
- [Notion's agent setup guide](https://developers.notion.com/prompts/setup): a broader context-system setup with Basic and Shared context options. Review its scope before choosing it; it can include memory/artifact/skill storage and a separately approved daily loop. Choose its components to fit your workflow; this guide does not enable a daily loop.
- [Five stories of teams using Notion MCP](https://www.notion.com/blog/mcp-use-cases): official examples of keeping reusable work and context alongside the team. Inspiration, not a guarantee of results or automatic access in your environment.

### GBrain and the company-brain idea

- [GBrain repository](https://github.com/garrytan/gbrain): Garry Tan's open-source memory system, with sources, correction and shared use as central ideas.
- [Company Brain tutorial](https://github.com/garrytan/gbrain/blob/master/docs/tutorials/company-brain.md): an advanced team-memory path with its own infrastructure and access design. It is not required for this starter.
- [GBrain site](https://gbrain.io/): the project's hosted product and further examples.

The useful pattern to borrow is a current, inspectable home for context and decisions. This guide does not install GBrain, reproduce its capabilities in Notion or require another platform. Start with what you already use; add machinery only when a specific gap justifies it.

[Back to Maestro Setup](../README.md)
