# Security Notes
- Enforce HTTPS and HSTS at reverse-proxy (e.g., Cloudflare or Vercel)
- Set CSP via proxy/server headers for stricter rules than meta tag.
- Validate file uploads (mime & size) at client and edge.
- Verify webhook signatures (Stripe/Twilio/Resend).
- Rate limit RSVP/public endpoints via `rate-limit` function.
- Keep SUPABASE_SERVICE_ROLE_KEY server-side only (never in client).
