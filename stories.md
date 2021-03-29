# Stories

Writing good stories is hard.

Above all else, remember the promise upon which trust between the customer and the engineering team is based:

_We will sustainably deliver the most important thing via the shortest route._

We must demonstrate to stakeholders exactly what user value we have delivered and are working on at any given time. We can't work in a deadline-free, no-fixed-deliverable methodology unless we keep the above promise, and more importantly, _are trusted_ to keep the above promise.

## Does this story say what a persona can now do?

What is it that the customer can do after the story, that they couldn't do before?

## Who is the customer?

The persona should not be the engineering team, nor the PM. The persona should be an end user or customer.

Creating a persona of the engineering team leads to mistaking chores for stories, and makes the team appear to be delivering value when in fact they are making themselves more efficient. The pay-off for this should be increased velocity later, not the earning of velocity now.

## Does this story deliver user value?

If any story does not, to the best estimate of the PM, deliver user value, then we're abusing the trust of business stakeholders. Any time we dress up a chore as a story, we're lying to the product owner.

## Does this story express a value statement?

Stories must express user value in a testable statement. Stories must not be imperative instructions of "_do the thing_", as these instructions are meaningless to non-technical staff and could be chores in disguise.

* Good: I can cross the river.
* Bad: Build a bridge.

Perhaps the engineering team is better at building rafts than bridges. Why do we want a bridge?

## Can the story be expressed more succinctly?

Can you use fewer words to express the value to be delivered?

* Good: As a visitor I can see the home page
* Bad: As a visitor I want to be able to see the home page
* Bad: As a visitor I should be able to see the home page

If there's only one persona in your backlog, you can omit the "As a someone" too.

## Does this story have too many deliverables?

In most cases, it's better to have many small specific stories than one that asks you to do three things.

Tell-tale smell: the story has a list of things for you to act upon.

## Is this story specific?

* Bad: As an app developer I can find all the docs in one place
* Good: As an app developer I can find the logging docs on GitHub
* Good: As an app developer I can find the networking docs in Confluence

If a story doesn't say _exactly_ what needs doing, then we can't estimate complexity, and there could be all sorts of assumption hiding, ready to bite us in the backside.

Tell-tale smell: the story mentions an unspecified plural

## Avoid "As a Persona I want..."

If you didn't want it, it wouldn't be in the backlog.

## How should I express my acceptance criteria?

Two common formats which work, depending on context:

- Gherkin language (GIVEN, WHEN, THEN)

This is good when you need to be explicit about the start and end state.

- Explicit list of steps

This is easy for engineers to follow, but requires a more granular level of understanding.

## Do the acceptance criteria define the user experience?

It is the Product Manager's responsibility to define the interface of the product. Acceptance criteria should define what the user experience and interface are.

Imagine a backlog for a CLI tool. A new feature is to be added to allow a size of VM to be specified.

* Good: When I run `cli --vm large` I get a large VM
* Bad: When I ask for a large VM, I get one

The PM is the guardian of the user experience, and such an important facet should not be left to the whims of whichever engineer happens to pick up the story.

## Is this a chore or part of a story?

The outcome of a chore should be to increase the long-term velocity of the engineering team.

A chore should _not_ be a technical task that is on the critical path to business value. If something that _must_ happen to deliver a story is broken out into a chore, this disguises complexity - it makes a story look simpler and shorter. Working on chores that are actually parts of stories can make it look to stakeholders as if the engineering team is spending time working on its own stuff instead of on the business' priorities. This is dangerous in a low-trust environment.

There will be times when it makes sense to play a genuine chore before a story, in order to make delivering that story easier. This is different to taking a critical part of a story and separating it out into a fake chore.

Possible reasons to break this rule are to make progress more visible. However, this then obscures information that the original story was either too big or unavoidably complex.

## Is this a spike or part of a story?

The outcome of a spike is information - usually _"can this be done?"_

A spike should not be used to work out _how_ something should be implemented. Deciding on the best/most appropriate implementation is part of every day work on stories, and every engineer has the authority to make whatever decisions they think are best.

If a decision is poor, there are plenty of after-the-fact safeguards:

* A new pair rotating onto the story
* Other engineers later encountering the code, and raising concerns in a retro
* Lower velocity as a result of the sub-optimal choice

If the tests pass, and the acceptance criteria are met, then we can live with any technical decision until it causes a problem. If it never causes a problem, then we don't have to fix it, and it probably wasn't a poor choice to start off with.
