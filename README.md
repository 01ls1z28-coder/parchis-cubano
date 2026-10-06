# Tinajón (Parchís Cubano)

Static build of Jorge Guerra's Tinajón table game for GitHub Pages at:

`https://01ls1z28-coder.github.io/parchis-cubano/`

Asset paths are rooted at `/parchis-cubano/`, so opening `index.html` with `file://` will not work. To preview locally:

```bash
mkdir -p /tmp/tinajon-serve/parchis-cubano
cp -R . /tmp/tinajon-serve/parchis-cubano/
cd /tmp/tinajon-serve
python3 -m http.server 8080
# open http://localhost:8080/parchis-cubano/
```

On Windows (PowerShell), from this folder's parent:

```powershell
New-Item -ItemType Directory -Force -Path .\serve\parchis-cubano | Out-Null
Copy-Item -Recurse -Force .\static-site\* .\serve\parchis-cubano\
cd serve
python -m http.server 8080
# open http://localhost:8080/parchis-cubano/
```

Online multiplayer uses peer-to-peer WebRTC. Peers find each other through public Nostr relays (Trystero). Game data stays between browsers. Some networks need a TURN server; without one, those pairs may fail to connect.

Created by Jorge Guerra.
