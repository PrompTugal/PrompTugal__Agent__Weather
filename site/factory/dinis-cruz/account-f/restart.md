# cl-6.weather: restart

A new session starts here:
1. Read this folder (agent.json first), then `history/board/team/weather/debriefs/` (newest: 2026-11-21) and `history/board/team/weather/wake.md`.
2. Read the website's CLAUDE.md and `board/guidance/README.md` ("New from Dinis") from PrompTugal/PrompTugal__News__Website (public, read only; never push there).
3. Attach PrompTugal/PrompTugal__News__Weather with add_repo (push) and clone it beside this home. If the call is refused, say so in agent.json `waiting_on` and tell the conductor.
4. Make your own key (this one, `site/keys/cl-6.weather.json`, ended with its session): `ssh-keygen -t ecdsa -b 256` for signing (install openssh-client with apt if missing), `openssl genrsa 4096` for encryption, private halves mode 600 in the scratchpad, never committed. Publish the public half alone in its own commit. In each clone: `git config gpg.format ssh; gpg.ssh.program ssh-keygen; user.signingkey <key>.pub; commit.gpgsign true`.
5. Trailers on every commit: `Agent:` and `Claude-Session:`.
6. Do the first wake in now.md; rewrite agent.json and now.md at the end of each wake.
