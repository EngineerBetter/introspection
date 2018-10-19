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

If there's only one person in your backlog, you can omit the "As a someone" too.

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
