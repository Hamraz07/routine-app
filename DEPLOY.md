# Deploy My Routine

1. Create a Supabase project.
2. In Supabase SQL Editor, run `supabase/schema.sql`.
3. Deploy `supabase/functions/ai-routine/index.ts` as an Edge Function named `ai-routine`.
4. Add the Edge Function secret `OPENAI_API_KEY`.
5. Optionally add `OPENAI_MODEL` if you want a different supported model.
6. Replace `__SUPABASE_URL__` and `__SUPABASE_ANON_KEY__` in `index.html` with your project's values.
7. Enable Email authentication in Supabase Auth. Configure your Site URL and redirect URLs for the final domain.
8. Host the folder as a static website (for example with a static hosting provider).
9. Test two separate accounts and verify that neither can see the other's routine.
10. Test overnight shifts, fixed college blocks, drag-and-drop, manual editing, AI changes, and week reset.
11. Before public launch, add rate limiting/cost controls and review privacy/terms requirements.
