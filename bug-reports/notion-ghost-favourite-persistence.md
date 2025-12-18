# Bug Report: Ghost Favourite Page Persistence

## Summary
A page marked as a favourite in Notion can persist as a “ghost” favourite after being removed, leading to inconsistent UI state and confusion when navigating the workspace.

## Product
- Application: Notion
- Platform: [Web / Desktop / Mobile]
- OS: [Windows / macOS / iOS / Android]
- Account type: [Free / Plus / Team, if relevant]

## Preconditions
- User has an active Notion workspace
- At least one page marked as a favourite
- Sidebar favourites visible

## Steps to Reproduce
1. Mark a page as a favourite in the Notion sidebar.
2. Remove the page from favourites or delete the page.
3. Navigate away from the current view.
4. Reload the workspace or restart the application.

## Expected Result
The page should be fully removed from favourites and no longer appear in the sidebar.

## Actual Result
The page remains visible as a favourite despite being removed or deleted, creating a “ghost” entry that cannot be interacted with normally.

## Reproducibility
Intermittent – occurs inconsistently but persists once triggered.

## Severity / Impact
- Severity: Low–Medium
- Impact:
  - Causes confusion in navigation
  - Creates inconsistent UI state
  - Reduces trust in sidebar accuracy

## Notes / Observations
- Issue appears related to client-side state not refreshing correctly.
- Restarting the app does not always resolve the issue.
- Behaviour suggests cached sidebar state or sync delay.

## Attachments
- Screenshots / screen recordings (if available)

