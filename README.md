# rustdeskpro-cus2

Portainer stack `rustdeskpro-cus2` on cus-dock2, managed by Portainer with git-backed
auto-update.

The compose uses `${VAR}` placeholders. The values live in the Portainer
stack environment (and in the host's `.env` for local runs) and are
deliberately NOT committed - see `.env.example` for the required keys.

## Update flow

Portainer polls this repo every 15 minutes and redeploys on a new commit.
Push to `main` (or `main`) and the stack updates itself.
