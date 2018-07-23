## written by FancyAction

# Communication

Standups and team text chat in Slack.<br>
Links are shared and stored in Toby collection and in the information repo <br>

# Workflow
MVP features (needs) and connected refactors & bugs are added to Waffle inbox.

# Issues
When issues are added to Waffle, they automatically appear on GH issues.

1. Use appropriate labels in Waffle:"Feature/Refactor/Style/Bug" and "Scope: Need/Scope: Wanted"
2. Claim an issue with the assignee button in the top-right corner of the issue.
3. Next, create a new local branch in the format: "tag/#Issue-This-Fixes-thing" (e.g. "feature/#16-format-numbers")
4. Push the new branch to GitHub, before making any commits. Waffle will auto-move the issue to "In Progress"
5. When finished, commit and push again. In the Pull Request title or description, write "closes #issueNumber". Waffle will move the issue to Review.
6. After another member has looked over the Pull Request, they will merge into development and delete remote branch. Waffle will move issue to Done.