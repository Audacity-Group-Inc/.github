# Audacity Group Inc
Audacity Group Inc connects real-time marketing signals to revenue, so every dollar you spend accelerates your sales force.

Post to click, click to lead, lead to deal, deal to revenue.

## Jetfly · Attribution Pilot
Jetfly traces a social post through its tracked link (UTM tags) and lead page to a Salesforce Opportunity, and credits revenue back to every campaign that influenced it, with single-touch and multi-touch side by side.

## How it's controlled
- Each agent runs as its own Salesforce Integration User with a least-privilege permission set.
- Jetfly: Read on Lead, Campaign, Campaign Member, Contact, Opportunity, Account; Create and Edit on Lead only. No delete, no Lead Status.
- Every action is logged under the agent's own user in the standard audit trail.
- A person approves record changes and qualifies every lead to SQL.

## Testing
Assign the Jetfly integration user its permission set from the managed package. Publish a post with a tracked link; the click creates a Lead automatically added to Campaign A. Add the same contact to Campaign B, then convert to an Opportunity with Campaign Influence on. The Jetfly dashboard shows each opportunity's process (time in each stage) bridged to its revenue, credited by single-touch and multi-touch from the same data.

## Status
The managed package is in development. Source repositories are private.
