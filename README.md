# Nightbyte UBG V3

This release completes the next 10 build steps on top of V2.

1. Real login/register UI API wiring
2. User session/profile state
3. Database-backed favorites
4. Database-backed ratings
5. Server-side game search/filter/sorting
6. Game detail API and richer game metadata
7. Admin dashboard APIs for games/users/stats/events
8. Admin thumbnail upload endpoint
9. Play analytics/event log
10. Production-oriented API/error/security foundation

## Run
Node.js 20+ is recommended.

```bash
npm install
# copy .env.example to .env and change secrets
npm start
```

Open http://localhost:3000.

Default admin values come from .env.example; change them before deployment.

## Notes
- SQLite is used for this build to keep setup simple.
- For a larger production deployment, move to PostgreSQL and object storage/CDN.
- Only host or embed games you have permission to distribute.
- This project does not contain proxy/filter-bypass functionality.
