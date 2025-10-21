# Local Dev Enhancements
- Start **MailHog** (web UI on http://localhost:8025) and **Stripe CLI** forwarder:
  ```bash
  docker compose up -d
  ```
- Run Supabase locally με `supabase start` (χρειάζεται Supabase CLI).
- Τρέξε migrations:
  ```bash
  bash scripts/migrations-smoke.sh
  # και μετά με supabase CLI για πραγματική εφαρμογή
  ```
- Κάνε enqueue ένα test email στην `email_queue` και παρακολούθησε το στο MailHog.
