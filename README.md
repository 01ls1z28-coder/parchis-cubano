# Tinajón (Parchís Cubano)

A static build of Jorge Guerra's Tinajón table game for GitHub Pages.

Play locally with a tiny static server (opening `index.html` via `file://` will not work for modules):

```bash
python3 -m http.server 8080
# then open http://localhost:8080/
```

On GitHub Pages this site is meant to live at:

`https://01ls1z28-coder.github.io/parchis-cubano/`

Online multiplayer uses peer-to-peer WebRTC. Peers find each other through public Nostr relays (Trystero). Game data stays between browsers. Restricted networks without a TURN server may fail to connect.

Created by Jorge Guerra.
