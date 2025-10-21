# Blue/Green & Multi-Region
- Deploy web to region Blue (A) and Green (B). 
- Weight traffic via CDN/Load Balancer (0/100 → 50/50 → 0/100).
- Use read replicas for public pages, write-region for RSVPs.
- Failover runbook included in OBSERVABILITY.md.
