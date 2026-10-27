# CS5610 Bonus 5: Svelte Counter

A 2 × 2 grid of clickable squares built with Svelte. Each square toggles independently between white (off) and black (on). The counter above the grid shows how many squares are currently on.

The parent `App.svelte` passes an `onToggle` callback to each `Counter.svelte` component so it can update the total.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed in the terminal.

## Demo

[Watch the short screen recording](svelte-counter-demo.mov).
