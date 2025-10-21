# ACME http-01
- Insert token/content into `acme_challenges` (token = requested path token).
- Edge function `/functions/v1/acme-http-01/.well-known/acme-challenge/:token` should be routed to this function (set proxy rule).
- Let's Encrypt will GET the token and verify ownership.
