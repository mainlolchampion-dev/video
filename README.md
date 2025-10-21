# .env Auto-Fill

This tool populates your `.env` automatically from your local Supabase instance.

## Requirements
- Supabase CLI installed
- You have run: `supabase start`

## Usage
Inside your project root (where `.env.mock-local` is located), copy these files into `scripts/` and run:

### macOS/Linux
```bash
node scripts/env-autofill.mjs
# or
bash scripts/env-autofill.sh
```

### Windows (PowerShell)
```powershell
node scripts\env-autofill.mjs
# or
powershell -ExecutionPolicy Bypass -File scripts\env-autofill.ps1
```

The script will:
1. Create `.env` from `.env.mock-local` if missing.
2. Read `supabase status --json`.
3. Write `VITE_SUPABASE_URL`, `SUPABASE_URL`, `VITE_SUPABASE_ANON_KEY`, `SUPABASE_SERVICE_ROLE_KEY` into `.env`.
