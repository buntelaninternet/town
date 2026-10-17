# Pixtown multiplayer

Run locally:   node server.js   then open http://localhost:3000
No npm install needed (zero dependencies, Node 16+). The 3D page loads three.js from cdnjs, so players need internet.

Deploy: any host that runs Node (Render, Railway, Fly.io, a VPS). Start command: `node server.js`.
Set PORT if the host asks for it. Claimed houses are saved to data.json; point DATA_FILE at a persistent disk/volume,
or the city resets when the host restarts. Behind nginx, turn off buffering for /api/events.
Changing the number of lots: edit N in server.js AND in public/index.html (search "N=120").
