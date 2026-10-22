# REVIVAL Team Board

Internal task board for Dr. Lily Baker's REVIVAL team (Lily, Kasper, Laura), served at https://team.repatternco.com.

- `index.html` is the whole site: dashboard, a tab per person, the monthly member goal.
- Data lives in the Supabase project **REVIVAL Team Board** (tables `board_tasks`, `board_goals`, `board_members`).
- Sign-in is by email and password. No emails are sent. Only emails listed in `board_members` can see or change anything, so the publishable key in `index.html` is safe to keep in this repo. Never put a secret or service key here.
- To give someone access: create their user in Supabase (Authentication → Users → Add user → Create new user, tick Auto Confirm User) and add their email to `board_members`.
- To reset a password: delete the user in Authentication → Users and create it again with a new password. Tasks aren't tied to accounts, so nothing on the board is lost.
- `CNAME` tells GitHub Pages to serve the site on team.repatternco.com.
