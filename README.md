# REVIVAL Team Board

Internal task board for Dr. Lily Baker's REVIVAL team (Lily, Kasper, Laura), served at https://team.repatternco.com.

- `index.html` is the whole site: dashboard, a tab per person, the monthly member goal.
- Data lives in the Supabase project **REVIVAL Team Board** (tables `board_tasks`, `board_goals`, `board_members`).
- Sign-in is by email link. Only emails listed in `board_members` can see or change anything, so the publishable key in `index.html` is safe to keep in this repo. Never put a secret or service key here.
- To give someone access, add their email to `board_members` in Supabase.
- `CNAME` tells GitHub Pages to serve the site on team.repatternco.com.
