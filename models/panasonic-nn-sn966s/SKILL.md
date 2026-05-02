---
name: panasonic-nn-sn966s
description: >
  Operate a Panasonic NN-SN966S. Invoke this skill when the user needs to
  perform cooking, reheating, defrosting, or other functions on this
  specific model. Do not generalise to other Panasonic models.
---

- **Manufacturer:** Panasonic
- **Model:** NN-SN966S
- **Type:** countertop
- **Wattage:** 1250W
- **Capacity:** 62L
- **Interface:** dedicated function pads (Sensor Reheat, Sensor Cook, Inverter Turbo Defrost, Keep Warm, Popcorn) + Power Level + Quick 30/More + Timer/Clock/Less + Number Pads + Stop/Reset + Start
- **Source:** https://www.manualslib.com/manual/2317087/Panasonic-Inverter-Nn-Sn966s.html

The NN-SN966S uses Panasonic Inverter technology, which delivers power as true continuous output at the selected level rather than cycling the magnetron on and off at full power. At P5 (50%), the oven runs continuously at half power — not full power for half the time. This is most noticeable during defrost, where conventional cycling leaves partially cooked edges while the centre remains frozen. All controls are discrete pads; there is no dial. Number pads enter time and weight directly. The Quick 30/More pad adds 30-second increments during manual cooking and also functions as a +20% time adjustment when used with sensor functions. Timer/Clock/Less subtracts 30-second increments and adjusts sensor functions by –20%.

## First Use Setup

After first plugging in, the oven prompts for two preferences before the clock:

1. Press Start once, then press Timer/Clock/Less to cycle between Metric (g/kg) and Imperial (oz/lb) weight units. Stop on the desired system.
2. Press Start once, then press Timer/Clock/Less to toggle Beep on or Beep off.
3. Press Stop/Reset to confirm. A colon (:) appears in the display.

## Quick Start

### Quick 30

**Invoke:** Press Quick 30/More (each press adds 30 seconds, up to 5 minutes).
**Parameters:** Power defaults to P10 (100%). Select a different power level first if needed.
**Execute:** Press Start.
**Returns:** Time counts down; five beeps at completion.

## Reheating

### Sensor Reheat

**Invoke:** Press Sensor Reheat.
**Parameters:** Optionally press Quick 30/More to add 20% more time, or Timer/Clock/Less to subtract 20%. Do not open the door until two beeps sound.
**Execute:** Press Start.
**Returns:** Two beeps when steam is detected and cooking time appears in display. Five beeps at completion.
**Edge cases:** Room temperature must be below 95°F (35°C). Food weight must exceed 4 oz (110 g). Oven cavity, glass tray, and any utensils must be dry before use. Do not use for bread or other dry foods, raw food, beverages, or frozen food.

## Defrost

### Inverter Turbo Defrost

**Invoke:** Press Inverter Turbo Defrost.
**Parameters:** Enter food weight using Number Pads (maximum 6 lbs / 3 kg). Weight is entered in pounds and tenths of a pound (e.g., 1.0, 2.5).
**Execute:** Press Start.
**Returns:** For larger items, two beeps sound midway — open door and turn over or rearrange food, then close and continue. Five beeps at completion.
**Edge cases:** Remove wrapper before defrosting. Place roasts fat-side down; whole poultry breast-side down. Large items may remain icy in the centre; standing time after defrosting will complete the process. Drain liquids during defrosting.

## Power Levels

**Invoke:** Press Power Level.
**Parameters:** P10 (100%) displays by default. Press Power Level repeatedly until the desired level appears.

| Display | Power |
|---|---|
| P10 | 100% |
| P9 | 90% |
| P8 | 80% |
| P7 | 70% |
| P6 | 60% |
| P5 | 50% |
| P4 | 40% |
| P3 | 30% |
| P2 | 20% |
| P1 | 10% |

Maximum cooking time at P10 is 30 minutes. At any other power level, the maximum is 99 minutes 99 seconds.

### Manual cooking

**Invoke:** Press Power Level, select level.
**Parameters:** Enter cooking time using Number Pads.
**Execute:** Press Start.
**Returns:** Time counts down; five beeps at completion.

## Sensor Cook

**Invoke:** Press Sensor Cook until the number for the desired food appears in the display.
**Parameters:** Optionally adjust with Quick 30/More (+20%) or Timer/Clock/Less (–20%).
**Execute:** Press Start.
**Returns:** Two beeps when steam detected and cooking time displays. Five beeps at completion.
**Edge cases:** Same conditions as Sensor Reheat: room below 95°F, food over 4 oz, dry cavity and tray. Do not open door before the two-beep signal.

### Sensor Cook codes

| Code | Food | Amount |
|---|---|---|
| 1 | Oatmeal | ½–1 cup (40–80 g) |
| 2 | Breakfast Sausage | 2–8 links |
| 3 | Omelet | 2–4 eggs |
| 4 | Quinoa | ¼–1 cup (45–180 g) |
| 5 | Soup | 1–2 cups (250–500 ml) |
| 6 | Frozen Entrées | 8–28 oz (220–800 g) |
| 7 | Frozen Pizza | 8 oz (220 g) single |
| 8 | Potatoes | 1–4 potatoes, 6–8 oz each (170–220 g) |
| 9 | Fresh Vegetables | 4–16 oz (110–450 g) |
| 10 | Frozen Vegetables | 6–16 oz (170–450 g) |
| 11 | Rice | ½–1½ cups (110–335 g) |
| 12 | Frozen Dinners | 11–16 oz (300–450 g) |
| 13 | Pasta | 2–8 oz (55–220 g) |
| 14 | Fish Fillets | 4–16 oz (110–450 g) |

## Keep Warm

**Invoke:** Press Keep Warm.
**Parameters:** Set warming time using Number Pads (maximum 30 minutes).
**Execute:** Press Start.
**Returns:** Time counts down; five beeps at completion.
**Edge cases:** Keep Warm only functions as a final stage after manual cooking. It cannot follow sensor operations, auto functions, or Inverter Turbo Defrost.

## Popcorn

**Invoke:** Press Popcorn.
**Parameters:** Press Popcorn once for 3.5 oz (99 g), twice for 3.0 oz (85 g), three times for 1.75 oz (50 g). Optionally adjust with Quick 30/More (adds 10 seconds per press) or Timer/Clock/Less.
**Execute:** Press Start. Cooking time appears in the display after several seconds.
**Returns:** Five beeps at completion.
**Edge cases:** Do not leave unattended. Stop if popping slows to 2–3 seconds between pops.

## Multi-Stage Cooking

Up to two power stages can be programmed in sequence. Standing Time and Delayed Start can also be combined with manual cooking.

### Standing time

After entering a cook stage, press Timer/Clock/Less, set stand time with Number Pads, press Start. Two beeps signal the transition from cooking to standing; five beeps when standing time ends.

### Delayed start

Press Timer/Clock/Less first, enter delay time with Number Pads, then set power level and cook time normally. Press Start; delay counts down, then cooking begins.

**Edge cases:** Standing time and delayed start cannot be programmed before any automatic function (Sensor Cook, Sensor Reheat, Popcorn, Inverter Turbo Defrost).

## Child Lock

**Invoke:** Press Start three times; the lock symbol appears in the display.
**Deactivate:** Press Stop/Reset three times; display returns to time of day.

## Clock

**Invoke:** Press Timer/Clock/Less twice while not cooking; the colon blinks.
**Parameters:** Enter the time of day using Number Pads.
**Execute:** Press Timer/Clock/Less. The colon stops blinking.
