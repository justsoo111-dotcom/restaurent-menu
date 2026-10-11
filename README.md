# Restaurant menu — GitHub Pages + Supabase

Self-contained static front end. Database tables and image bucket use `restaurant_*` names and are separated from the vape catalog.

Read `README-AR.txt` for full Arabic deployment steps. Run `restaurant-supabase-setup.sql`, create an Auth user, add its UID to `restaurant_admins`, and fill `restaurant-config.js` with the project URL and public publishable key. Never add service-role/secret keys, database passwords, or admin passwords to the public repository.
