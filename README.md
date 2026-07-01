**Check it out at: [kd.jpp.fyi](https://kd.jpp.fyi)**

Helps people jamming synchronize a rotation across a session.
Open it on a phone, a laptop, or cast it to a screen the whole room can see. 
Bring up a QR code to share the session with other devices.

Born out of discussion and experimentation at the wonderful 
[Kreativ Data](https://www.skogen.pm/groups/DnnWsyJX2cAHDh7Yu) study circle.

## How it works

The wheel is divided into one ring per player. As time passes the wheel turns,
and the segments passing under the pointer are the players who are **on** right now. 
The countdown indicates when the next change is happening.

## Coordinating the rotation

Open the settings (the gear, top-right) to shape the rotation for your group:

- **Sections** — how many players (or slots) are in the rotation.
- **Active at once** — how many of them play simultaneously.
- **Switch every** — how long each turn lasts before the group rotates, in
  minutes. The active segments blink during the final 10 seconds as a heads-up
  that a swap is coming.
- **Evolving order** — when on, the rotation never settles into the same sequence.
  Instead of one repeating turn, the schedule becomes a single long, seam-free loop in
  which sections gradually weave past one another (using *plain hunting*, the pattern
  bell-ringers use), so that over the loop **everyone gets a turn alongside everyone
  else**. The wheel shows a moving **window** onto this loop; the rest is folded away
  behind a **second, dashed line** opposite the now line. The order is derived from the
  clock, so every synced device evolves identically.
  - **Mixing** — temperature: how fast the order reshuffles (how often the weave steps).
  - **Zoom** / **Show whole loop** — widen the window to see more of the
    loop at once; at full zoom the entire woven loop is shown as a static map. You can
    also pinch (touch / trackpad) or ⌘-scroll to zoom. *(These two are local viewing
    controls and aren't shared in the QR.)*

## Making it readable across the room

- **Shape** — `Half`, `Full`, or `Portrait`, to fit whatever screen you're on.
  Tapping the centre of the dial cycles through the shapes too.
- **Identifier** — label sections with Numbers, Letters, Animals, or nothing.
- **Label position** — keep labels centred, pinned to the edge so they stay
  visible, or sitting on the now line.
- **Dark mode** — follows your system by default; toggle to override.
- **Speed** — `1×` for real time, or `60×` (useful for debugging)

## Sharing a setup

Tap **Show QR code** to get a QR (and link) that encodes the whole rotation
config — sections, active count, interval, evolving order and its mixing,
speed, identifier, and shape.
Anyone who scans it lands on the same wheel, already configured. All the wheels
that have the same settings are automatically synced as long as everyones clocks
are the same.

---

## Running and deploying

### Local preview

```sh
npm install
npm run dev
```

Or just open `public/index.html` directly in a browser — it works standalone.
