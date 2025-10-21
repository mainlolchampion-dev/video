# Observability
- **/functions/v1/metrics** exposes Prometheus text format (counts of main tables).
- Import `observability/dashboards/invitations.json` in Grafana.
- Use GitHub Actions `load-test` job (k6) to smoke load test.
