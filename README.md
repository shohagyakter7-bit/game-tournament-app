# Game Tournament Starter (Full-stack skeleton)

This archive contains:
- backend/ : Node.js Express + Socket.IO minimal server (in-memory demo)
- mobile/  : React Native skeleton with App.js demo
- admin/   : Simple React admin dashboard demo
- db/      : Postgres migration SQL (001_init.sql)

## Next steps I recommend (to productionize)
- Replace in-memory stores with Postgres + Redis
- Add proper JWT middleware & refresh token flow
- Add Dockerfile(s) & Kubernetes manifests
- Integrate payments ONLY for non-cash/cosmetic items and consult legal counsel

## Quick run (backend demo)
cd backend
npm install
npm run dev

## Docker & docker-compose (local dev)
Run the following to start Postgres, Redis, backend and admin:
```
docker-compose up --build
```
This will expose:
- Backend: http://localhost:4000
- Admin: http://localhost:3001

## GitHub Actions CI
A basic CI workflow was added at `.github/workflows/ci.yml`. It installs backend deps and builds a Docker image as an example. Extend it with tests and deploy steps.

