# My Routine — Production Build

My Routine is a multi-user, cloud-backed routine planner with natural-language AI scheduling.

## Included in this build
- Private Supabase accounts and row-level security.
- Personalized greetings and profile name.
- Monday–Sunday routine with automatic selection of the real current weekday.
- College mapping can be represented as fixed activities (the original mapping is preserved in the local prototype).
- Add, edit, delete and complete activities.
- Overnight activities (for example 20:00–08:00).
- Drag-and-drop swapping for non-fixed activities.
- Week overview.
- Natural-language AI planner with review-before-save.
- Deterministic server-side conflict validation, including cross-midnight conflicts.
- One automatic AI repair pass when validation fails.
- Completion state preservation when a generated plan keeps an identical activity slot/name.
- Installable PWA shell.
- User data isolation through Supabase RLS.

## Important
This package is production-oriented but is not a hosted service by itself. You still need to configure Supabase, deploy the Edge Function, add your OpenAI key, replace the placeholders in `index.html`, and host the site.

Before a public launch, test email confirmation/recovery, rate limiting, abuse controls, API cost limits, timezone/DST edge cases, long overnight schedules, consecutive night shifts, and backups.
