# NetOrbit Card Plus

A fork of the card from [NetOrbit](https://github.com/the-scott-davis/netorbit), the live radial network map for Home Assistant. It needs the NetOrbit integration installed; only the card is forked.

## What it adds

- **Zoom**: mouse wheel, pinch, or the + / − / fit buttons in the header.
- **Pan**: drag the empty background.
- **Arrange**: drag any device or hub anywhere and it stays there, for example each printer's smart plug next to its printer. Links follow while you drag. Double-click (or double-tap) an item to send it back to its automatic spot, or use *Reset all positions*.
- **Several NetOrbit entries**: with one entry per subnet, actions from the card (move, rename, remove, make a hub) go to the entry the device belongs to, not always the first one.

Positions are saved per Home Assistant user, in Home Assistant's own frontend storage, so they follow you between browsers.

## Install

HACS › ⋮ › Custom repositories › add `https://github.com/brentgl/netorbit-card-plus` with type **Dashboard**, then download **NetOrbit Card Plus** and refresh the browser.

## Use

```yaml
type: custom:netorbit-card-plus
title: Home Network
```

It takes the same options as the original `netorbit-card`, plus:

| Option | Default | What it does |
| --- | --- | --- |
| `layout_key` | `netorbit-card-plus` | Where positions are saved. Give two cards different keys to arrange them separately. |

## Licence

MIT, as the original. See [LICENSE](LICENSE).
