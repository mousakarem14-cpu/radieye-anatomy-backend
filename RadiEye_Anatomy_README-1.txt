RadiEye Anatomy — Rebuild package

Files:
- RadiEye_Anatomy_Full_Rebuild.html : responsive bilingual frontend preview with theme toggle, library filters, lesson progress/bookmarks stored locally, navigation, and sample admin/account screens.
- RadiEye_Anatomy_Supabase_Schema.sql : starting PostgreSQL/Supabase schema with roles, content workflow, media rights metadata, learning paths, bookmarks, progress, reviews, and row-level security policies.

How to preview:
1. Open the HTML file in a modern browser.
2. Test the Arabic/English toggle and light/dark theme.
3. Test library filters/search, lesson bookmark/completion, profile summary, and responsive mobile menu.

Production status:
This package is NOT yet a production platform. The HTML is a frontend prototype. Login, admin permissions, content publishing, cloud media storage, and member data are not connected to a live backend. The SQL is a starting schema and must be reviewed/tested in a new Supabase project before use. Never put a Supabase service-role key in browser code.

Before launch:
- Create Supabase project and configure Auth providers, redirect URLs, email templates, backups and storage buckets.
- Review and test all RLS policies, especially role assignment and profile updates.
- Build the production frontend in a framework such as Next.js and connect it to Supabase using public anon/publishable credentials only.
- Add secure admin/editor workflows, audit logs, rate limits, error monitoring, privacy policy, terms, and backup/restore tests.
- Replace sample lessons and counts with medically reviewed content and properly licensed images; store source and license metadata for every asset.
- Test Arabic/English content completeness, keyboard accessibility, contrast, mobile layouts, and all page states.
