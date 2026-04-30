---
name: lg-lmc0975st
description: >
  Operate an LG LMC0975ST. Invoke this skill when the user needs to
  perform cooking, reheating, defrosting, or other functions on this
  specific model. Do not generalise to other LG models.
manufacturer: LG
model: LMC0975ST
type: countertop
wattage: 1000W
capacity: 25L
interface: SmoothTouch glass controls — dedicated function keys (Auto Cook, Auto Reheat, Popcorn, Defrost, Power Level, Cook Time, Timer On/Off) + slide touch +/– bar + STOP/Clear + START/Enter
source: https://www.manualslib.com/manual/2457776/Lg-Lmc0975st.html
---

The LMC0975ST is part of LG's NeoChef line, featuring Smart Inverter technology (continuous power output at the selected level, not duty-cycle pulsing) and an EasyClean interior coating that resists stains. Controls are SmoothTouch glass — there are no physical buttons that depress. The +/– area functions both as discrete touch targets and as a slide bar: swipe right on the bar to increase a value quickly, swipe left to decrease it, or press the + or – ends individually for single-increment changes. Most operations begin by opening the oven door and pressing STOP/Clear to reset, then selecting a function, using +/– to set values, and pressing START/Enter. When cooking ends, a chime sounds and "End" appears in the display; the chime repeats every minute until the door is opened or a button is pressed.

## Quick Start

**Invoke:** Close oven door. Press STOP/Clear. Press START/Enter.
**Parameters:** Starts 30 seconds at 100% power. Each additional press of START/Enter adds 30 seconds.
**Execute:** First START/Enter press starts cooking immediately.
**Returns:** Chime sounds; End displays at completion.

## Reheating

### Auto Reheat

**Invoke:** Open oven door. Press STOP/Clear. Press Auto Reheat repeatedly to select the desired category.
**Parameters:** Press + until the correct amount appears in the display.

| Code | Category | Amount |
|---|---|---|
| Ar-1 | Beverage | 1–2 cups (240 ml per cup) |
| Ar-2 | Casserole | 10–20 oz |
| Ar-3 | Dinner plate | 1 plate |
| Ar-4 | Pie | 1–3 slices |
| Ar-5 | Pizza | 1–3 slices |

**Execute:** Close oven door. Press START/Enter.
**Returns:** Chime sounds; End displays at completion.

## Defrost

The LMC0975ST has four preset defrost cycles. A chime sounds partway through each cycle; open the door and turn, separate, or rearrange the food, then press START/Enter to continue.

| Code | Category | Weight range |
|---|---|---|
| dEF1 | Meat | 0.1–6.0 lbs |
| dEF2 | Poultry | 0.1–6.0 lbs |
| dEF3 | Fish | 0.1–4.0 lbs |
| dEF4 | Bread | 0.1–2.0 lbs |

**Invoke:** Open oven door. Press STOP/Clear. Press Defrost repeatedly until the desired category displays (dEF1–dEF4).
**Parameters:** Press + until the correct weight appears in the display (in 0.1 lb increments).
**Execute:** Close oven door. Press START/Enter.
**Returns:** Midway chime to check and turn food. Chime sounds at completion; End displays.

## Power Levels

Ten power levels are available. If no power level is selected, the oven defaults to 100% (P-HI).

| Display | Power | Example use |
|---|---|---|
| P-HI | 100% | Boiling water, browning meat |
| P-90 | 90% | |
| P-80 | 80% | |
| P-70 | 70% | |
| P-60 | 60% | |
| P-50 | 50% | Whole poultry |
| P-40 | 40% | |
| P-30 | 30% | |
| P-20 | 20% | |
| P-10 | 10% | Keeping dishes warm |

### Manual cooking with power level

**Invoke:** Open oven door. Press STOP/Clear. Press Cook Time.
**Parameters:** Press + or – until the desired cooking time appears in the display. Press Power Level — P-HI displays. Press – to decrease power level in 10% increments if desired.
**Execute:** Close oven door. Press START/Enter.
**Returns:** Chime sounds; End displays at completion.

### Adjusting time during cooking

Press + to add 10 seconds; press – to subtract 10 seconds.

## Auto Cook

**Invoke:** Open oven door. Press STOP/Clear. Press Auto Cook repeatedly to select the desired category.
**Parameters:** Press + until the correct amount appears in the display.

| Code | Category | Amount |
|---|---|---|
| Ac-1 | Bacon | 2–4 slices |
| Ac-2 | Fresh Vegetable | 1–4 cups |
| Ac-3 | Frozen Entrée | 10–40 oz |
| Ac-4 | Frozen Vegetable | 1–4 cups |
| Ac-5 | Oatmeal | 1–2 servings |
| Ac-6 | Potato | 1–4 potatoes |
| Ac-7 | Rice | ½–2 cups |

**Execute:** Close oven door. Press START/Enter.
**Returns:** Chime sounds; End displays at completion.

## Popcorn

**Invoke:** Open oven door. Press STOP/Clear. Press Popcorn once — PoP displays.
**Execute:** Close oven door. Press START/Enter.
**Returns:** Chime sounds at completion.
**Edge cases:** Do not leave unattended. Do not use a brown paper bag.

## Child Lock

**Invoke:** Touch and hold STOP/Clear for approximately 3 seconds; Loc appears in the display and a melody sounds.
**Deactivate:** Touch and hold STOP/Clear for approximately 3 seconds; Loc disappears and a melody sounds.

## Clock

**Invoke:** Open oven door. Press + repeatedly to toggle between 12-hour and 24-hour modes.
**Parameters:** Press START/Enter to confirm the clock mode. Press + or – to select the desired hour. Press START/Enter to confirm. Press + or – to select the desired minutes. Press START/Enter to finish.
**Edge cases:** Press and hold + or – to move through numbers quickly.

## Kitchen Timer

**Invoke:** Press Timer On/Off once; 10 displays in the display.
**Parameters:** Press + or – until the desired time appears.
**Execute:** Press START/Enter. Countdown begins.
**Returns:** Melody sounds; End displays. Press STOP/Clear to dismiss.
**Deactivate before completion:** Press Timer On/Off once; display returns to time of day.

## Interrupting Cooking

Open the door — cooking stops, display light stays on. Close the door and press START/Enter to resume. To cancel and clear remaining time: open the door and press STOP/Clear.

## Smart Diagnosis

Press and hold the Smart Diagnosis pad on the control panel while holding the mouthpiece of a phone up to the Smart Diagnosis logo on the oven, when directed to do so by LG service centre personnel. This transmits operational data to assist with remote diagnostics.
