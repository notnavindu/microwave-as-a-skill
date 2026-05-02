---
name: toshiba-em131a5c
description: >
  Operate a Toshiba EM131A5C. Invoke this skill when the user needs to
  perform cooking, reheating, defrosting, or other functions on this
  specific model. Do not generalise to other Toshiba models.
---

- **Manufacturer:** Toshiba
- **Model:** EM131A5C
- **Type:** countertop
- **Wattage:** 1100W
- **Capacity:** 34L
- **Interface:** number pads + dedicated sensor pads (Sensor Reheat, Frozen Pizza, Frozen Entrée, Potato, Rice, Veggie) + 1 LB Defrost + Custom Defrost + Power Level + Cook Time + START ADD 30 SEC + One Touch Start pads (1–6) + Favorite + Clock + Kitchen Timer + STOP Cancel
- **Source:** https://www.manualslib.com/manual/1445879/Toshiba-Em131a5c-Bs.html

The EM131A5C has a flat numeric keypad layout. Most cooking operations start by pressing Cook Time and entering digits, then adjusting power level if needed before pressing START. The six One Touch Start pads (labelled 1–6) provide a shortcut: pressing pad 1 starts 1 minute at full power, pad 2 starts 2 minutes, and so on up to 6 minutes. The START ADD 30 SEC pad starts 30 seconds at full power from standby and adds 30 seconds during active cooking. Power level can be set before entering cook time or after — the manual states "prior to or during cooking" — but must be set before pressing START. The humidity sensor controls require specific conditions (room under 95°F, food over 4 oz, dry cavity) and should not be interrupted before the cooking time appears in the display.

## Quick Start

### One Touch Start

**Invoke:** Press number pads 1–6 directly from standby.
**Parameters:** None. Each pad number sets that many minutes at 100% power.
**Execute:** Cooking starts immediately on pad press.
**Returns:** Oven beeps 5 times at completion.

### START ADD 30 SEC

**Invoke:** Press START ADD 30 SEC from standby.
**Parameters:** Each press adds 30 seconds at 100% power, up to a maximum of 99 minutes 99 seconds.
**Execute:** First press starts cooking immediately.
**Returns:** Oven beeps 5 times at completion.
**Edge cases:** Time can be added during active Microwave Cooking and Time Defrost. Cannot be added during Weight Defrost or Kitchen Timer.

## Power Levels

Ten power levels are available.

| Display | Power |
|---|---|
| PL10 | 100% |
| PL9 | 90% |
| PL8 | 80% |
| PL7 | 70% |
| PL6 | 60% |
| PL5 | 50% |
| PL4 | 40% |
| PL3 | 30% |
| PL2 | 20% |
| PL1 | 10% |

### Setting power level

**Invoke:** Press Cook Time, enter desired time, then press Power Level — PL10 displays.
**Parameters:** Press the number pad corresponding to the desired level (1–10).
**Execute:** Press START ADD 30 SEC.
**Returns:** Time counts down; oven beeps 5 times at completion.
**Edge cases:** Power level must be set after Cook Time, not before. If no power level is set, cooking runs at PL10 (100%).

## Reheating

### Sensor Reheat

**Invoke:** Press Sensor Reheat; SC-1 displays.
**Execute:** Press START ADD 30 SEC.
**Returns:** Oven detects steam and sets cooking time automatically. Oven beeps 5 times at completion.
**Edge cases:** Food must be covered with a vented lid to allow steam to escape. Room temperature must be below 95°F (35°C). Food weight must exceed 4 oz (110 g). Oven and glass tray must be dry. Do not open door before cooking time appears in display. Not suitable for bread, dry biscuits or cake, raw food, beverages, or frozen food. Minimum food temperature: 40°F (5°C).

## Defrost

### 1 LB Defrost

**Invoke:** Press 1 LB Defrost; display shows 1.0, DEF., and Lbs.
**Execute:** Press START ADD 30 SEC.
**Returns:** DEF. flashes and remaining defrost time displays. Oven beeps 5 times at completion.

### Custom Defrost

**Invoke:** Press Custom Defrost.
**Parameters:** Enter food weight using number pads; select food category.
**Execute:** Press START ADD 30 SEC.
**Returns:** Defrost time is calculated automatically from the entered weight and category. Oven beeps 5 times at completion.

## Sensor Menu

The sensor menu pads cook specific foods automatically using humidity detection.

| Pad | Display | Food |
|---|---|---|
| Sensor Reheat | SC-1 | Reheat (see Reheating section) |
| Frozen Pizza | SC-2 | Frozen Pizza |
| Frozen Entrée | SC-3 | Frozen Entrée |
| Potato | SC-4 | Potato (puncture with fork; space 1 inch apart; up to 4 on turntable) |
| Rice | SC-5 | Rice |
| Veggie | SC-6 | Fresh Vegetables |

**Invoke:** Press the desired sensor pad; the corresponding SC- code displays along with Auto and SENS.
**Execute:** Press START ADD 30 SEC.
**Returns:** Sensor detects steam and sets time automatically. Oven beeps 5 times at completion.
**Edge cases:** Same conditions apply as Sensor Reheat. Do not open door before cooking time appears.

## Auto Menus

### Custom Cook and Soften/Melt

| Code | Function | Amount |
|---|---|---|
| CC-1 | Custom Cook | — |
| CC-2 | Custom Cook – Bacon | — |
| CC-3 | Custom Cook – Frozen Roll/Muffin Reheat | — |
| CC-4 | Custom Cook – Beverage | — |
| CC-5 | Custom Cook – Chicken Pieces | — |
| S-1 | Melt – Butter/Margarine | 1–3 sticks |
| S-2 | Melt – Chocolate | 4/8 oz |
| S-3 | Melt – Cheese | 8/16 oz |
| S-4 | Melt – Marshmallows | 5/10 oz |
| S-5 | Soften – Butter | 1–3 sticks |
| S-6 | Soften – Ice Cream/Frozen Juice | 6/12/16 oz |
| S-7 | Soften – Cream Cheese | 3/8 oz |

**Invoke:** Press Auto Menu pad repeatedly until the desired code displays.
**Parameters:** Use number pads to select serving size or weight where applicable.
**Execute:** Press START ADD 30 SEC.

## Popcorn

**Invoke:** Press Popcorn repeatedly to select bag size: 1.75 oz → 3.0 oz → 3.5 oz.
**Execute:** Press START ADD 30 SEC; Auto and Oz display. Auto flashes when cooking begins.
**Returns:** Oven beeps 5 times at completion.

## Multi-Stage Cooking

A maximum of two stages can be set. Quick Touch sensor pads cannot be used in multi-stage cooking.

**Invoke:** Press Favorite to begin sequence programming.
**Parameters:** Set Cook Time for stage 1, then Power Level for stage 1. Set Cook Time for stage 2, then Power Level for stage 2.
**Execute:** Press START ADD 30 SEC.
**Returns:** Stages execute in sequence. Saved sequences can be recalled by pressing Favorite.

### Retrieving a saved sequence

Press Favorite; the saved program code displays. Press START ADD 30 SEC to run.

## Child Lock

**Invoke:** Press and hold Power Level for 3 seconds; a long beep sounds and Lock displays.
**Deactivate:** Press and hold Power Level for 3 seconds; long beep sounds and Lock disappears.

## Kitchen Timer

**Invoke:** Press Kitchen Timer once; 00:00 displays.
**Parameters:** Enter time using number pads (maximum 99 minutes 99 seconds).
**Execute:** Press START ADD 30 SEC to start countdown.
**Returns:** Timer indicator disappears; oven beeps 5 times at completion. No cooking occurs during kitchen timer.
**Edge cases:** No cooking function can be set while the kitchen timer is active.

## Error States

- **Sensor cooking does not start or gives unexpected results:** Room temperature exceeded 95°F (35°C), food was below 4 oz, or cavity/tray was not dry before cooking. Reset and ensure conditions are met.
- **Arcing or sparking:** Non-microwave-safe cookware in use, or food residue on cavity walls. Stop immediately and clean cavity before continuing.
