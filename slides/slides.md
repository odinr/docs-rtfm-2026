---
layout: cover
---

<style>
.cover-title {
  margin-left: auto;
  margin-right: auto;
  width: fit-content;
  text-align: left;
}
.cover-title__word {
  display: block;
  font-size: 5rem;
  line-height: 1.2em;
}
.cover-title__word::first-letter {
  font-weight: bold;
}
</style>
Adaptive
<h1 class="cover-title">
  <span class="cover-title__word"><Keyword>Intent</Keyword></span>
  <span class="cover-title__word">Driven</span>
  <span class="cover-title__word">Development</span>
</h1>

<!--
Oh great! 
Yet another 3 letter abrivation....
But we are only going to focus on the word; Intent.
Ever pounded on why developers still are around?
Why do we need developers when the internet holds all the knowledge in the world?
Why do we need developers when agents can generate code out the wazoo?

First we need to clarify some definitions.
-->

---
layout: statement
---

# Develop

## Creating __solutions__ by applying __knowledge__

<Quote author="dictionary.com">
Bring out the capabilities or possibilities<br/>
to a more advanced or effective state.
</Quote>

<!--
A developers job is to create solutions by applying knowledge.
Solutions are created by knowing how to to apply that knowledge
-->

---
layout: statement
---

# Intent

## __Goal__ of applying knowledge

<Quote author="dictionary.com">
Something that someone is <b>intending</b> or meaning<br/>
to achieve purpose or objective.
</Quote>

---
layout: fact
---

Knowing that 25 laps indoor is 5km run is useful....

<div v-click>

but applying <Keyword><b>knowledge</b></Keyword> to solve a problem is <b><u>priceless</u></b>

```ts {2,14}
/**
 * Calculate the number of laps required to cover a given distance.
 *
 * @param total_length – distance to cover (e.g. metres)
 * @param lap_length – length of one lap (e.g. 200m indoor, 400m outdoor)
 * @returns number of laps required
 *
 * @example
 * const goal = 5000;
 * calculateNumberOfLaps(goal, 200); // 25 — indoor
 * calculateNumberOfLaps(goal, 400); // 12.5 — outdoor
 */
calculateNumberOfLaps(total_length, lap_length) {
  // Divide the total distance we want to cover by the length of one lap
  const laps = total_length / lap_length;
  return laps;
}
```

</div>

---
layout: statement
---

# If the <Keyword>intent</Keyword> is clear<br/> 
## wrong implementation is a temporary problem.
---

# <Keyword><b>Intent</b></Keyword> <u>persists</u>
## Implementation evolves

<style>
.intent-boxes {
  position: relative;
  min-height: 20rem;
}
.intent-box {
  position: absolute;
  inset: 0;
  margin: 0;
}
</style>



<div class="stacked-clicks intent-boxes">

<div class="stacked-click intent-box" v-click v-click.hide="1">

```ts {1,3}
/** explain the intended way to use the implementation */
function fn(...args: number[]): number {
    // explain the intended implementation
}
```
</div>

<div class="stacked-click intent-box" v-click="1" v-click.hide="2">

```ts {2-7,10} 
/**
 * Multiplies all provided numbers.
 *
 * @example
 * const result = product(1, 2, 3); // 6
 *
 * @returns the product of all provided numbers
 */
function product(...args: number[]): number {
    // iterate through all provided args and multiply with each other
}
```

</div>

<div class="stacked-click intent-box" v-click="2" v-click.hide="3">
```ts {11-14}
/**
 * Multiplies all provided numbers.
 *
 * @example
 * const result = product(1, 2, 3); // 6
 *
 * @returns the product of all provided numbers
 */
function product(...args: number[]): number {
    // iterate through all provided args and multiply with each other
    let result = 1;
    for (const value of args) {
        result *= value;
    }
    return result;
}
```
</div>

<div class="stacked-click intent-box" v-click="3" v-click.hide="4">
```ts {11} 
/**
 * Multiplies all provided numbers.
 *
 * @example
 * const result = product(1, 2, 3); // 6
 *
 * @returns the product of all provided numbers
 */
function product(...args: number[]): number {
    // iterate through all provided args and multiply with each other
    const result = args.reduce((cur, next) => cur * next, 1);
    return reuslt
}
```
</div>

<div class="stacked-click intent-box" v-click="4">
```ts {11-12}
/**
 * Multiplies all provided numbers.
 *
 * @example
 * const result = product(1, 2, 3); // 6
 *
 * @returns the product of all provided numbers
 */
function product(...args: number[]): number {
    // iterate through all provided args and multiply with each other
    const [head, ...tail] = args;
    const result = head * product(...tail);
    return result;
}
```
</div>

</div>

---
layout: statement
---

# The collective <Keyword>intent</Keyword> 
## is the culture of __solution__

---
layout: full
---

<SlidevVideo autoplay autoreset="slide" playsinline muted id="intent-video">
  <source src="./media/capture-intent.mp4" type="video/mp4" />
</SlidevVideo>

<style>
  #intent-video {
    margin: 0 auto;
    height: 100%;
  }
</style>
---

# Conventions

Rules for the <Keyword>intended</Keyword> way of implementing

```md
## Functional style
Prefer functions and composition; avoid classes and imperative mutation.

## Immutability
Never mutate in place; return new data instead.

## map/reduce vs for loops
Prefer `map`, `reduce`, and other array methods over imperative `for` loops.

## TSDoc
Every exported function, type, and module has accurate `@param`, `@returns`, and `@example` where useful.

## Intent comments
Use short internal comments for maintainers that explain *why*, not what the code literally does.
```

---

# Contribute

Guide for <Keyword>intended</Keyword> contributions

```md
## How we intend you to make a PR

### 1. Open an issue first
For non-trivial changes — align on scope and approach before coding.

### 2. Branch from main
One logical change per PR; keep it reviewable.

### 3. Follow project style
Match existing patterns, formatting, and structure.

### 4. Describe intent
Clear title and description: what changed and why.

### 5. Respond to review
Address feedback or discuss; don't leave threads hanging.

### 6. Squash when we ask
Keep history clean; we'll say when to squash.
```

---

# Documentation

Description of the <Keyword>intended</Keyword> solution

```md
# my-app

React app with components and route-based views.

## Get started
`bun install`
`bun run dev`

## Project structure
my-app/
├── src/
│   ├── components/
│   ├── routes/
│   └── App.tsx
├── public/
└── package.json
```

---

# Changeset

Clear <Keyword>intentions</Keyword> of changes

Changeset
```md
---
my-app: patch
---

Fixed redirect loop when session expires on protected routes.
```

Changelog
```md
## 1.2.0 (2026-01-15)
- **fix:** #666 - Fixed redirect loop when session expires on protected routes.
```

---

# Architecture Decision Records

Record of <Keyword>intended</Keyword> decisions

```md
# 001: Use React for the frontend

## Status
Accepted

## Context
We need a UI framework that supports components and fast iteration.

## Decision
We will use React with TypeScript.

## Consequences
- Strong ecosystem and hiring pool
- Need to manage state (e.g. Zustand)
```

---

# Artifacts

Documentation of the lifecycle — not just issues on a board.

<VClick>

## Feature
__Why__ is a solution needed and __what__ is the <Keyword>intended</Keyword> value

</VClick>
<VClick>

## Use Case
__Who__ are the <Keyword>intended</Keyword> actors

</VClick>
<VClick>

## Task
__How__ to execute <Keyword>intended</Keyword> work

</VClick>

---

# Instructions

Rules the agent follows on (almost) every request — *how* to write and which conventions to apply.

```md
When writing or editing TypeScript in this repo:

## Conventions
Read and apply the conventions in `./contribute/typescript.md` before suggesting or generating code.

## Match existing code
Same style and patterns as the file you're editing.

## Don't violate conventions
Don't suggest code that breaks the conventions (e.g. no mutable in-place updates if immutability is required).

## TSDoc
Add TSDoc for any new exported function or type; include `@param`, `@returns`, and `@example` where useful.

## Intent comments
Prefer short comments that explain *why*, not what the code does.
```

---

# Skills

Documented procedures that tell an agent *when* to run and *what* to do.

```md
---
name: create-pr
description: Use when the user asks to create or open a pull request.
---

1. Validate state
   - Check we're on a branch.
   - Check all changes are staged.
   - Ask the user if unstaged changes should be included.
2. Commit
   - Diff changes to `main`.
   - Generate a proper commit message.
3. Quality
   - Follow project style.
   - Run linter and tests.
4. Draft PR
   - Use the PR template `.github/PULL_REQUEST_TEMPLATE.md`.
   - Generate a proposed markdown PR description.
5. Create PR
   - Use `gh pr create --base main --fill` (or `--title` / `--body-file` for template).
```

---

# Agent

An AI that acts on your behalf — uses instructions (how to behave) and skills.

```md
You are an agent that helps generate TypeScript code in this repository.
You adhere to the project's contribute docs (conventions, style, PR flow).
You help create PRs by following the create-pr skill when the user asks.

## Tone
- Be concise and direct.
- Use clear, professional language.
- Explain *why* when suggesting changes, not just *what*.

## Instructions
- Read and apply `.github/copilot-instructions.md` on every request.
- For TypeScript, follow conventions in `./contribute/typescript.md`.

## Scope
- Stay in this repo; only touch files outside the workspace if the user explicitly asks.
```
