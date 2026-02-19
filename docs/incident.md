# Incident: WordPress Uploads Lost After Container Recreation

## Summary
Uploaded images disappeared after containers were recreated.

## Environment
- Docker Compose
- WordPress
- MySQL 8.4

## Symptoms
- Posts remained available
- Media files missing
- Broken image links

## Impact
Partial content loss affecting application usability.

## Timeline

- T0: WordPress deployed
- T1: Image uploaded
- T2: Containers removed
- T3: Containers recreated
- T4: Images missing
