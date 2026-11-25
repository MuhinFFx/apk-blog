# APKZone configured starter
Supabase URL and publishable key are set in app.js.
1. Create bucket `apk-files`, public, size limit 50 MB.
2. Create your auth user in Supabase.
3. Add that user ID to admins table using SQL: `insert into public.admins(user_id) values ('YOUR-USER-UUID');`
4. Deploy these static files using GitHub and Cloudflare Pages.
Never add service-role keys to this site. Public bucket downloads are publicly accessible.
