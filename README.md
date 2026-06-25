**Check it out at: [kd.jpp.fyi](https://kd.jpp.fyi)**

Helps people jamming synchronize a rotation across a session.
Open it on a phone, a laptop, or cast it to a screen the whole room can see. 
Bring up a QR code to share the session with other devices.

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
- **Splits** — whether the active players sit together in one block on the wheel
  or are broken into several groups spread around it.

## Making it readable across the room

- **Circle size** — scale the dial. You can also pinch (touch / trackpad) or
  ⌘-scroll to zoom.
- **Shape** — `Half`, `Full`, or `Portrait`, to fit whatever screen you're on.
  Tapping the centre of the dial cycles through the shapes too.
- **Identifier** — label sections with Numbers, Letters, Animals, or nothing.
- **Label position** — keep labels centred, pinned to the edge so they stay
  visible, or sitting on the now line.
- **Dark mode** — follows your system by default; toggle to override.
- **Speed** — `1×` for real time, or `60×` (useful for debugging)

## Sharing a setup

Tap **Show QR code** to get a QR (and link) that encodes the whole rotation
config — sections, active count, interval, splits, speed, identifier, and shape.
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
