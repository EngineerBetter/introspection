# Engineering

If we could express all the subtlety of good engineering practice in a single Markdown document, then we wouldn't have jobs. So treat this as a small subset of concerns!

## Reusability and The Rule Of Three

Make something reusable when it has been duplicated three times.

Am I making something reusable before it needs to be re-used?

If the current story takes longer because you're preparing for the future, you're risking engineering something that will never be used, and making this story seem more expensive when really the velocity hit should be in a later story. This misleads the PM and the client.

## Can I use a pattern?

The use of patterns reduces diversity in the codebase, and diversity in the number of idioms that the readers of your code need to keep in mind. Complexity _requires_ diversity, so reducing diversity reduces complexity.

## Will it take longer to write this as a chore than to fix?

If making code cleaner is quicker than writing what needs to be done in a chore, do it now. If it takes any longer to fix than to write up, stick it in Tracker as a chore for someone to pick up when they're waiting for a build, or when technical debt becomes problematic.