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
.cover-aside {
  width: fit-content;
  font-size: 1rem;
}
</style>
Adaptive
<h1 class="cover-title">
  <span class="cover-title__word"><Keyword>Intent</Keyword></span>
  <span class="cover-title__word">Driven</span>
  <span class="cover-title__word">Development</span>
</h1>
<p class="cover-aside">*Because software clearly needed another design doctrine.</p>

<!--
So... Adaptive Intent Driven Development.

Sounds like a __tech buzzword__ engineered to lure middle management into a workshop.
But this is not another methodology. We have enough of those.

> what still makes us unique at the dawn of the __AI__?

AI can execute, generate, optimize, and explain.
But it does not mean anything by it.

Intent is the __human part__.
It is the reason something should exist, the constraint that matters,
and the difference between code that runs and code that is right.

That is where our __role__ changes.
- We become __architects__ of intent: shaping what should exist and why.
- We become __witnesses__: observing what the system actually does, not what it said it did.
- We become the __jury__: deciding if the result matches the intent,
or just looks right.

If implementation gets cheaper, understanding gets more important.

That is the future I want to talk about.
-->

---
layout: statement
---

# AI can generate <Keyword>code</Keyword>
## But can it know what __right__ means?

<!--
This is the shift.
AI can write code. Annoyingly fast.

But __execution__ is not the same as __judgment__.

Something can look right, compile, and still mean the wrong thing.

Before, the bottleneck was implementation.

Someone had to write the code, wire the tests, fight the framework, and get the thing working.

Now the machine can produce a plausible implementation in minutes.

That does not remove the work. It just moves it.

So the __bottleneck__ moves from typing code to defining intent.
- __What__ should exist? 
- __Why__ should it exist? 
- __Which__ constraints exists?

That is where the __human__ role starts to matter.
-->

---
layout: fact
---

## The missing piece 
# <Keyword><b>Intent</b></Keyword>

<!--
Intent becomes more important when implementation gets cheaper.

AI can generate content quickly, then the hard question is not:
> can we produce something?

The hard question is:
> does this match what we meant?

Most teams already know this __feeling__.

> why did we do it like this?

We expect the tools to __understand our architecture__, our conventions, our trade-offs,
and all the cursed decisions that somehow became load-bearing.

But a model does not magically know the point.
It can generate something plausible and still miss the __reason the thing exists__.

So intent is not just nice __context__ around the work.

Intent is the reason behind the __solution__,
and it gives us something concrete to compare the generated __output__ against
when we decide whether it is __actually right__.
-->

---
layout: statement
---

# Development

## Applied <keyword>knowledge</keyword> turned into a solution

<Quote author="dictionary.com">

Bring out the <u>capabilities</u> or <u>possibilities</u> <br/>
to a more advanced or effective state.

</Quote>

<!--
Development

The dictionary version is nice.
Very official. Very dictionary.

Development is not __just knowing things__.
It is not collecting tools, patterns, and clever answers like __achievements__,
then hanging them on the wall as __diplomas__ for problems we have not solved yet.

> That is knowledge. Useful, but still just raw material.

Development starts when that knowledge has to work in reality.
When it has to solve a __real problem__, inside a __real system__,
with __real constraints__ and all the weird history that comes with it.

That is the move from __possibility to solution__.

And this is where AI changes the pressure a bit.
AI can give us a lot of possibilities very __quickly__.
Code, plans, docs, designs, explanations, summaries.

But development is not just producing more possibilities.
Development is __deciding__ which possibility should become the solution.

-->

---
layout: statement
---

# Intent

## The __goal__ that gives <Keyword>knowledge</Keyword> direction

<Quote author="dictionary.com">

Something that someone is <u>intending</u> or <u>meaning</u><br/>
to <u>achieve</u> purpose or objective.

</Quote>

<!--
So if development is __applied knowledge__,
intent is what tells us __where and how__ to apply it.

Intent is the goal behind the activity.
The reason this solution should __exist__.
The thing we are trying to make true.

Without that, knowledge has no __direction__.
It is just a pile of techniques looking for an excuse.

With intent, we can make __choices__.
We can say:
> - yes, this helps.
> - No, this is noise.
> - And sometimes: absolutely not, what problem are we actually solving here?

That is why intent matters.
It helps us build better, more __useful context__,
so we get __less noise__ and __better decisions__.
-->

---
layout: fact
---

## Knowing that 25 indoor laps is 5 km is useful.

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

<!--
Knowing that 25 laps indoor is 5 km is useful.
But applying knowledge to solve a problem is priceless.

And that is the key difference:
knowing the answer is not the same as knowing how to apply knowledge.

This example is intentionally simple.
The code is just division.
__No magic__.

What matters is the reasoning behind why the output is correct.

In other words, the value is not only the result.
The value is that we can __explain__ how it works and why it is right.
-->

---
layout: statement
---

# If the <Keyword>intent</Keyword> is clear<br/> 
## wrong implementation is a temporary problem

<!--
If the intent is clear, a wrong implementation is __annoying__, but __temporary__.

You still have a reference point.

You can point at the result and say: this does not match the goal, so fix it.

__That is survivable__.

If the intent is missing, the wrong implementation does not look wrong for long.

It slowly becomes normal.

Then it becomes "how we do things here," which is just technical debt with a company accent.

-->
---
layout: statement
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

<!--
The intent defines what the __function means__, while the implementation is allowed to __evolve__ underneath it.

We start by making behavior explicit.
Then we can swap in a loop, a reduce, recursion, or one beautifully broken version with a typo, because reality.

Some implementations are cleaner.
Some are faster.
Some are only acceptable if you enjoy incident postmortems.

But if __intent is clear__, change is safe.
We can replace the internals and still __verify__ that the __behavior__ stayed true.
-->

---
layout: statement
---

# Shared <Keyword>intent</Keyword>
## becomes engineering __culture__

<!--
> Intent in one person's head is a bottleneck with a salary. 

It can feel efficient for a while, especially if that person is fast and souped up on coffee, but it does not scale.

Shared intent becomes __engineering culture__. 
Not culture as in a poster saying "quality" while the build has been red since Tuesday. 
Real culture is repeated understanding: things people can read, test, question, and correct.

> If __humans and agents__ are going to co-exist,<br/>
> the intent has to live somewhere outside one person's brain.
-->

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

<!--
Intent is a weird word to land on, right?
- It is not a specification you can write down and hand off.
- It is not a diagram.
- It is not even code.

__But it is real__, and we feel its __absence__ constantly.

> how do we actually capture it?

Not the __idea__ of intent — that part is settled.
But the mechanics: 

> what form does intent take when it has to leave one person's head and live in shared space?

> How do you make it concrete enough to guide a system, but flexible enough to survive the mess of reality?

That is the question.
-->

---
layout: statement
---

# Specify

## <Keyword><b>What</b></Keyword> and <Keyword><b>why</b></Keyword>

<!--
First phase: specify.
> "write me some code."

__That is not a specification__.

Real specifying means saying:
- what should exist
- why it needs to exist
- what makes it *acceptable*.

Not perfect. Acceptable. 

This is where prompting stops being __vibes__ and starts being useful.
> You are not decorating a prompt with __emojis and hopium__.
> You are building __context__.
-->

---
layout: statement
---

# Plan

## Steps of <Keyword><b>how</b></Keyword>

<!--
Then comes the plan.

> And let me be clear: the plan is not sacred. Do not start a plan religion.

A plan starts with __research__: 
- what has been tried before? 
- What constraints actually exist?
- What does the landscape already look like? 

> A plan without research is just optimistic guessing.

A plan becomes the __artifact of intent__. 

It is what we meant to do, written down and actionable.

Changing a plan __is cheap__. Conversations and research cost coffee.

Refactoring code built on __misunderstanding__? 

That is when meetings multiply, and dreams die by consensus.
-->

---
layout: statement
---

# Implement

## Execution grounded in <Keyword><b>intent</b></Keyword>

<!--
Then we implement.
> This is where AI is genuinely useful.

It can move quickly, connect patterns, generate boilerplate, refactor, and never once complain about meetings.

> That is lovely.

But the implementation is not meant to be free-floating code confetti falling from the sky.
It should be __grounded in intent__ and __rooted in the plan__.
That is how speed becomes useful instead of just creating more surface area to __regret__ later.

> Speed without direction is just momentum in the wrong direction.
-->

---
layout: statement
---

# Evaluate

## Does the <b>output</b> match the <Keyword><b>intent</b></Keyword>?

<v-click>
<div class="intent-loop">
  <div class="intent-loop__step intent-loop__step--specify">
    <span>1</span>
    <h3>Specify</h3>
    <p>What and why</p>
  </div>
  <div class="intent-loop__step intent-loop__step--plan">
    <span>2</span>
    <h3>Plan</h3>
    <p>How to approach it</p>
  </div>
  <div class="intent-loop__step intent-loop__step--evaluate">
    <span>4</span>
    <h3>Evaluate</h3>
    <p>Compare with intent</p>
  </div>
  <div class="intent-loop__step intent-loop__step--implement">
    <span>3</span>
    <h3>Implement</h3>
    <p>Build from context</p>
  </div>
  <div class="intent-loop__center">
    <Keyword>Intent</Keyword>
  </div>
  <div class="intent-loop__arrow intent-loop__arrow--top">&rarr;</div>
  <div class="intent-loop__arrow intent-loop__arrow--right">&darr;</div>
  <div class="intent-loop__arrow intent-loop__arrow--bottom">&larr;</div>
  <div class="intent-loop__arrow intent-loop__arrow--left">&uarr;</div>
</div>
</v-click>

<style>
.intent-loop {
  position: relative;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 2.4rem 4rem;
  width: min(48rem, 100%);
  margin: 2.4rem auto 0;
}

.intent-loop__step {
  border: 1px solid rgba(93, 131, 146, 0.28);
  border-radius: 8px;
  padding: 1rem 1.15rem;
  min-height: 6.5rem;
  background: rgba(93, 131, 146, 0.07);
}

.intent-loop__step span {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 1.6rem;
  height: 1.6rem;
  border-radius: 999px;
  margin-bottom: 0.45rem;
  background: var(--slidev-theme-primary, #5d8392);
  color: white;
  font-size: 0.9rem;
  font-weight: 700;
}

.intent-loop__step h3 {
  margin: 0;
  font-size: 1.2rem;
  line-height: 1.15;
  font-weight:bold;
}

.intent-loop__step p {
  margin: 0.35rem 0 0;
  line-height: 1.25;
  color: rgba(255,255,255, 0.5)
}

.intent-loop__step--specify,
.intent-loop__step--evaluate {
  border-color: rgba(93, 131, 146, 0.45);
  background: rgba(93, 131, 146, 0.14);
}

.intent-loop__center {
  position: absolute;
  inset: 50% auto auto 50%;
  transform: translate(-50%, -50%);
  display: flex;
  align-items: center;
  justify-content: center;
  width: 8.2rem;
  height: 8.2rem;
  border: 1px solid rgba(93, 131, 146, 0.35);
  border-radius: 999px;
  background: white;
  font-size: 1.35rem;
  font-weight: 700;
  box-shadow: 0 0.7rem 2rem rgba(31, 41, 55, 0.08);
}

.intent-loop__arrow {
  position: absolute;
  color: var(--slidev-theme-primary, #5d8392);
  font-size: 2rem;
  font-weight: 700;
  line-height: 1;
}

.intent-loop__arrow--top {
  top: 2.25rem;
  left: 50%;
  transform: translateX(-50%);
}

.intent-loop__arrow--right {
  top: 50%;
  right: 1.45rem;
  transform: translateY(-50%);
}

.intent-loop__arrow--bottom {
  bottom: 2.25rem;
  left: 50%;
  transform: translateX(-50%);
}

.intent-loop__arrow--left {
  top: 50%;
  left: 1.45rem;
  transform: translateY(-50%);
}
</style>

<!--
Evaluation closes the loop. And this is where the real work lives.

The question is not just: 

> does the result look right?

Code can look right and still be wrong with excellent posture. Tests pass. It deploys. Nobody complains yet.

The better question is: 

> does the output match our intent?

If not, either the __implementation is wrong__, or __our understanding__ changed because we learned something in the building.

Either way, the __artifacts get better__.
The plan did its job: it made the mismatch visible early.
So the next round starts with less guessing and more __shared understanding__.
-->

---
layout: statement
---

# Project <Keyword>AI</Keyword> evolution
## Four phases toward autonomy

<!--
This is the transition point.
So far, this has been about how humans and AI collaborate on one task.

But the same pattern scales up.
Over time, a whole project evolves based on how much intent it can expose.

If we agree intent matters, then the next question is: 

> how does a project actually evolve with AI over time?

It is not 
> codebase in, press play on tape.

That fantasy usually ends in __expensive confidence__.

What we see instead is __phases__.

Each phase depends on how much intent the project can expose and preserve.
The more clearly a project explains itself, the more __useful__ AI becomes.

So think of this as an __evolution model, not a maturity poster__.

We are moving from ad-hoc assistance toward reliable autonomy, __one phase at a time__.
-->

---

# From __Bro__ to __Pro__

<div class="ai-lifecycle">
  <div class="ai-lifecycle__phase">
    <span class="ai-lifecycle__number">1</span>
    <h2>Bro-code</h2>
    <p>Knowledge stays tribal</p>
  </div>
  <div class="ai-lifecycle__arrow" v-click="1">&rarr;</div>
  <div class="ai-lifecycle__phase ai-lifecycle__phase--active" v-click="1">
    <span class="ai-lifecycle__number">2</span>
    <h2>Assisted</h2>
    <p><Keyword>Intent</Keyword> guides the prompt</p>
  </div>
  <div class="ai-lifecycle__arrow" v-click="2">&rarr;</div>
  <div class="ai-lifecycle__phase ai-lifecycle__phase--active" v-click="2">
    <span class="ai-lifecycle__number">3</span>
    <h2>Observing</h2>
    <p>AI turns usage into signals</p>
  </div>
  <div class="ai-lifecycle__arrow" v-click="3">&rarr;</div>
  <div class="ai-lifecycle__phase ai-lifecycle__phase--autonomous" v-click="3">
    <span class="ai-lifecycle__number">4</span>
    <h2>Autonomous</h2>
    <p>AI acts on signals</p>
  </div>
</div>

<style>
.ai-lifecycle {
  display: grid;
  grid-template-columns: 1fr auto 1fr auto 1fr auto 1fr;
  gap: 0.75rem;
  align-items: stretch;
  margin-top: 3rem;
}

.ai-lifecycle__phase {
  position: relative;
  box-sizing: border-box;
  overflow: hidden;
  border: 1px solid rgba(93, 131, 146, 0.35);
  border-radius: 8px;
  padding: 1rem;
  min-height: 9rem;
  background: rgba(93, 131, 146, 0.07);
}

.ai-lifecycle__phase--active {
  background: rgba(93, 131, 146, 0.16);
}

.ai-lifecycle__phase--autonomous {
  border: 2px solid rgba(75, 145, 98, 0.9);
  background:
    linear-gradient(135deg, rgba(75, 145, 98, 0.36), rgba(93, 131, 146, 0.16)),
    rgba(75, 145, 98, 0.16);
  box-shadow: inset 0 0 0 3px rgba(75, 145, 98, 0.16), 0 0 1.5rem rgba(75, 145, 98, 0.18);
  z-index: 1;
}

.ai-lifecycle__number {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 1.75rem;
  height: 1.75rem;
  border-radius: 999px;
  margin-bottom: 0.75rem;
  background: var(--slidev-theme-primary, #5d8392);
  color: white;
  font-weight: 700;
}

.ai-lifecycle h2 {
  margin: 0;
  font-size: 1.3rem;
  line-height: 1.2;
}

.ai-lifecycle__phase--autonomous .ai-lifecycle__number {
  background: rgb(75, 145, 98);
  box-shadow: 0 0 0 2px rgba(255, 255, 255, 0.14);
}

.ai-lifecycle__phase--autonomous h2 {
  color: white;
}

.ai-lifecycle__phase--autonomous p {
  color: rgba(255, 255, 255, 0.88);
  font-weight: 700;
}

.ai-lifecycle p {
  margin: 0.75rem 0 0;
  line-height: 1.35;
}

.ai-lifecycle__arrow {
  display: flex;
  align-items: center;
  color: var(--slidev-theme-primary, #5d8392);
  font-size: 2rem;
  font-weight: 700;
}
</style>

<!--
So this is the rough evolution.

First we have bro-code.
> Knowledge stays tribal. Intent lives in someone's head, or in Slack, or in that one __keyboard warrior__ who somehow remembers why the payment flow is allergic to Tuesdays.

It can look fast.
It can even look heroic.
But it is also a bus factor wearing sunglasses.

Then we move into assisted.
> The human still __drives__, but AI helps with execution.

Here, intent starts to matter because it guides the prompt, the plan, and the review.

Then observing.
> AI starts extracting intent and signals from sessions and artifacts: the traces we leave behind while pretending software is orderly.

And finally autonomous.
> AI can act on those __signals__.

But autonomy does not remove the need for intent. It raises the price of missing it.

-->

---
layout: statement
---

# The hard part is not <Keyword>watching</Keyword>
## It is knowing what the observation means

<!--
One thing I keep noticing is how big the documentation part has become.
Not just formal docs, but everything around the work: the plans, summaries, notes, reviews, logs, and reflections.

> The hard part is no longer __producing enough context__.

> The hard part is __surviving__ the amount of context we produce.

Suddenly there is a lot __more text__, and the annoying part is that much of it is __actually useful__.

Humans cannot consume all of it.

So the project starts to develop gray matter: messy, partial, connected memory spread across sessions and artifacts.

> That gray matter is valuable, but only if we can extract meaning from it.

__That is where intent becomes the filter__.

Intent helps __condense the noise into context__ without throwing away the knowledge underneath.

- The goal is not less knowledge.
- The goal is knowledge we can actually use.
-->

---
layout: statement
---

# From data to <Keyword>signals</Keyword>

<div class="signal-equation">
  <div class="signal-equation__panel">
    <h2>Data</h2>
    <div class="signal-equation__chips">
      <span>Telemetry</span>
      <span>Analytics</span>
      <span>Tickets</span>
      <span>Pull requests</span>
      <span>Documentation</span>
    </div>
  </div>
  <div class="signal-equation__operator">+</div>
  <div class="signal-equation__panel signal-equation__panel--intent">
    <h2><Keyword>Intent</Keyword></h2>
    <p>What should be true?</p>
  </div>
  <div class="signal-equation__operator">=</div>
  <div class="signal-equation__panel signal-equation__panel--signal">
    <h2>Signal</h2>
    <p>Something changed that matters</p>
  </div>
</div>

<style>
.signal-equation {
  display: grid;
  grid-template-columns: 2fr auto 1.25fr auto 1.5fr;
  gap: 1rem;
  align-items: stretch;
  margin-top: 3rem;
}

.signal-equation__panel {
  border: 1px solid rgba(93, 131, 146, 0.28);
  border-radius: 8px;
  padding: 1.25rem;
  background: rgba(93, 131, 146, 0.07);
}

.signal-equation__panel h2 {
  margin: 0 0 1rem;
  font-size: 1.45rem;
}

.signal-equation__panel p {
  margin: 0;
  line-height: 1.35;
}

.signal-equation__panel--intent {
  background: rgba(93, 131, 146, 0.12);
}

.signal-equation__panel--signal {
  border-color: rgba(75, 145, 98, 0.45);
  background: rgba(75, 145, 98, 0.16);
}

.signal-equation__chips {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.signal-equation__chips span {
  border-radius: 999px;
  padding: 0.25rem 0.6rem;
  background: rgba(93, 131, 146, 0.14);
  font-size: 0.9rem;
  line-height: 1.25;
}

.signal-equation__operator {
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--slidev-theme-primary, #5d8392);
  font-size: 2.5rem;
  font-weight: 700;
}
</style>

<!--
This is the equation for useful observation.

- Data tells us what happened.
- Intent tells us whether it matters.
- Together, they become signal.

And signal is the useful shape we extract from the project's __gray matter__.

- It tells us about __health__.
- It shows __evolving patterns__.
- It surfaces __relevant information__.
- It points to what needs __human focus__.
- It gives us a sense of __direction__.

Without intent, data just piles up.
-->

---
layout: statement
---

# Signals need <Keyword>intent</Keyword>
## Otherwise the AI can only guess

<!--
This is where signals connect to autonomy.

A bug signal tells the system that something is wrong.
Useful, yes.
But not enough to act.

If the system is going to create a change request, it needs to know the __intended behavior__.
- What should have happened?
- What constraint matters?
- What is the difference between a bug and a deliberate trade-off with terrible public relations?

> Without intent, the system can detect pain, but it cannot prescribe medicine.

> It can guess at a fix, but it cannot know whether the fix moves us toward the goal.

Autonomy starts when the system can connect those two without __hallucinating__ a product strategy in the middle.
-->

---
layout: statement
---

# Words <Keyword>matter</Keyword>
## That's why it is called a <u>__large language model__</u>

<!--
This is why words matter.
> It is called a large language model, not a large code model.

That sounds like a joke, but it is also the operating manual.
AI reads code, yes, but it also reads names, comments, issues, PRs, docs, examples, and all the tiny sentences where we accidentally __reveal what we meant__.

That __language is where intent survives__.
- Not as bureaucracy.
- Not as punishment for finishing the fun part.
- As memory.

Write down the why, the constraint, the trade-off, the edge case, the thing that looks wrong but was deliberate.

- If the words are vague, the model guesses.
- If the words are clear, the model has something to reason with.

-->

---

# Artifacts

<div class="intent-artifacts">
  <div class="intent-artifacts__center">
    <h2><Keyword>Intent</Keyword></h2>
    <p>The project memory layer</p>
  </div>
  <div class="intent-artifacts__grid">
    <div class="intent-artifacts__item">
      <h3>Conventions</h3>
      <p>How we work</p>
    </div>
    <div class="intent-artifacts__item">
      <h3>Documentation</h3>
      <p>What should be true</p>
    </div>
    <div class="intent-artifacts__item">
      <h3>ADRs</h3>
      <p>Capture decisions</p>
    </div>
    <div class="intent-artifacts__item">
      <h3>Tests</h3>
      <p>Validate behaviours</p>
    </div>
    <div class="intent-artifacts__item">
      <h3>Issues</h3>
      <p>Problems and desired outcomes</p>
    </div>
    <div class="intent-artifacts__item">
      <h3>Pull requests</h3>
      <p>What changed</p>
    </div>
  </div>
</div>

<style>
.intent-artifacts {
  display: grid;
  grid-template-columns: 1fr 2.2fr;
  gap: 1.5rem;
  align-items: stretch;
  margin-top: 2.5rem;
}

.intent-artifacts__center {
  display: flex;
  flex-direction: column;
  justify-content: center;
  border: 1px solid rgba(93, 131, 146, 0.35);
  border-radius: 8px;
  padding: 1.5rem;
  background: rgba(93, 131, 146, 0.12);
}

.intent-artifacts__center h2 {
  margin: 0;
  font-size: 2rem;
}

.intent-artifacts__center p {
  margin: 0.75rem 0 0;
  line-height: 1.35;
}

.intent-artifacts__grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.75rem;
}

.intent-artifacts__item {
  border: 1px solid rgba(93, 131, 146, 0.22);
  border-radius: 8px;
  padding: 0.95rem 1rem;
  background: rgba(93, 131, 146, 0.06);
}

.intent-artifacts__item h3 {
  margin: 0;
  font-size: 1.1rem;
  font-weight: bold;
}

.intent-artifacts__item p {
  margin: 0.4rem 0 0;
  line-height: 1.3;
}
</style>

<!--
This is why artifacts matter.
> They are not paperwork! They are the project memory layer.

Conventions, documentation, ADRs, tests, issues, pull requests.
Each one captures a small piece of intent.

Together, they become the project's __gray matter__.
Not a perfect archive. Not a holy book.
More like a messy brain: 
- partial memories 
- useful connections
- suspicious gaps.

That is enough.
The system does not need every artifact to be __perfect__.
It needs enough __connected context__ to triangulate what we meant.

As implementation gets cheaper, this layer gets more important.

> The code says what exists now.

> The artifacts explain why it exists, what should stay true, and what reality can be compared against.
-->

---
layout: statement
---

# No <Keyword>intent</Keyword>, no autonomy
## Signals without meaning are just noise

Observe → Reflect → Adapt → Evaluate.

<!--
Autonomy is not __"let the machine wander around and improve things"__.

> Claude worked on my project for 10 hours, spent 640M tokens. It was amazing, but nothing works anymore.

Real autonomy is a closed loop.

- Observe reality.
- Reflect against intent.
- Adapt the system.
- Evaluate the result.

The important part is that action is not the end of the story.
The system has to check whether the change actually moved us toward the goal.

So this is the same pattern we already talked about, just with more AI allowed to act inside the loop.

> Intent still decides what "better" means.
-->

---
layout: statement
---

## This is not only an <Keyword>AI</Keyword> problem

<!--
This sounds like an AI problem, but it is older than the tools. 

> AI just turns up the volume.

With clear intent, we can __rebuild__ an implementation and still know whether it is right.
Without it, even the original code becomes questionable, because nobody knows what is essential and what is just history wearing a name badge.
-->

---
layout: statement
---

# Implementation is <Keyword>cheap</Keyword>
## Misunderstanding is still <u>__expensive__</u> 💸

<!--
This is where the economics get spicy. 
- AI makes implementation cheaper. 
- It does not make misunderstanding cheaper.

Actually, it can scale __misunderstanding beautifully__. If the intent is wrong or missing,
the model can help us go very fast in the wrong direction and format the __disaster nicely__.

So the boring question is: 
> can we generate code? Yes. Obviously.

The useful question is: 
> can we evaluate generated code against intent?
-->

---
layout: statement
---

# Our job is not to protect <Keyword>code</Keyword>
## It is to protect __understanding__

<!--
> Our job is not to protect code like today's implementation is sacred. 

It is not.

> Some of it was written under conditions we should probably not discuss in public.

> Our job is to protect understanding. 

Understand the problem, name the constraints,
make the trade-offs explicit, and leave enough intent for the next person,
or the next agent, to continue without guessing.

-->

---
layout: statement
---

# Make the <Keyword>intent</Keyword> clear
## Then let the implementation <u>evolve</u>

<!--
So this is the closing thought.

> Make the intent clear, then let the implementation evolve.

Because the implementation will evolve. It always does.
The tools will change, the code will change, the architecture will change,
and some future version of us will look back at today's best decision and quietly judge it.

That is fine.

- The dangerous part is not change.
- The dangerous part is change without memory.

- So specify what matters.
- Plan against it.
- Implement with help.
- Evaluate without mercy.

That is Adaptive Intent Driven Development:
> not protecting the code we have, but protecting the understanding that lets the next version be better.
-->
