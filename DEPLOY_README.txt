SOLV Fleet Web App — TEST DEPLOYMENT ONLY

This deployment package excludes the historical fleet/fuel CSV files and contains no credentials.

1. Create a PRIVATE GitHub repository.
2. Upload the CONTENTS of this ZIP to the repository root (not the ZIP file itself).
3. In Vercel: Add New > Project > Import Git Repository.
4. Framework: Vite; build command npm run build; output directory dist.
5. Add environment variables in Vercel project settings:
    VITE_SUPABASE_URL = value from Supabase Project URL
    VITE_SUPABASE_ANON_KEY = Supabase publishable/anon key only
Never put the database password or service_role/secret key in Vercel VITE_ variables.
6. Deploy and test sign-in with a test project and dummy records.

PRODUCTION NOTE: Not yet audited or production tested; confirm RLS/security, backup policies, data residency, corporate approval and access control before live corporate data.
