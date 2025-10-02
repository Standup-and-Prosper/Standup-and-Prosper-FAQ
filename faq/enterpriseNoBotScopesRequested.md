## Error details: `no_bot_scopes_requested`

If you see an error in the Slack login screen screen that looks like this, it means you are attempting to log into Slack using your Enterprise Slack Workspace.

<img width="664" height="445" alt="enterpriseNoBotScopesRequested" src="https://github.com/user-attachments/assets/a6756710-c8aa-4132-be9f-1447ae45ffdb" />



For enterprise Slack accounts, Slack separates identifiers into "Enterprise Identifier" and "Workspace Identifiers". There are many workspaces in a single enterprise account. When installing Standup & Prosper into your Slack account, you can either install it at the enterprise level or at the team workspace level.

## Solution

When you want to log into Standup & Prosper after you have installed the bot, you must always log in with a specific workspace. This is a limitation from Slack. The workspace you want to chose should match the workspace where your standups are configured. As each workspace can configure their own standups, choosing the correct workspace to log in with is crucial.

<img width="726" height="815" alt="image" src="https://github.com/user-attachments/assets/db4e8daa-913e-47b7-b1c2-b8dae7fba61f" />


