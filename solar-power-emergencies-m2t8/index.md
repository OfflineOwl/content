# Solar Power for Emergencies

> **Harvest the Sun When the Grid Goes Down** - Solar power is the most reliable renewable energy source for emergency preparedness. With the right setup, you can keep critical devices charged indefinitely.

## Why Solar for Emergencies?

- **Fuel-free:** No gasoline, propane, or other consumables needed
- **Silent operation:** Unlike generators, solar panels make no noise
- **Low maintenance:** No moving parts, minimal upkeep
- **Scalable:** Start small and expand as budget allows
- **Long lifespan:** Quality panels last 20-25+ years

---

## Portable Power Stations

A portable power station (sometimes called a solar generator) is a large rechargeable battery with built-in inverter and charging ports. This is the easiest entry point for emergency solar power.

### What to Look For

| Feature | Why It Matters |
|---------|---------------|
| **Capacity (Wh)** | Determines how long you can run devices. 500Wh is a solid starting point. |
| **Inverter output (watts)** | Must exceed the wattage of your largest device. |
| **Solar input (watts)** | Higher input = faster recharge. Look for 100W+ input capability. |
| **Battery chemistry** | LiFePO4 (lithium iron phosphate) lasts 2,500-3,500 cycles vs. 500-800 for standard lithium-ion. |
| **Weight** | Consider portability. Under 15 lbs is easily portable. |
| **Output ports** | AC outlets, USB-A, USB-C, 12V DC (car port). More variety = more flexibility. |
| **Pass-through charging** | Ability to charge and discharge simultaneously. |

### Sizing Your Power Station

**Calculate your daily needs:**

| Device | Watts | Hours/Day | Wh/Day |
|--------|-------|-----------|--------|
| Phone charging | 15 | 2 | 30 |
| LED lantern | 5 | 6 | 30 |
| NOAA weather radio | 3 | 4 | 12 |
| Laptop | 60 | 2 | 120 |
| CPAP machine | 40 | 8 | 320 |
| Fan | 30 | 6 | 180 |

**Rule of thumb:** Your power station should hold at least **1.5x your daily Wh consumption** to account for inefficiency losses and partial cloudy-day recharges.

### Budget Options

- **Under $200:** 200-300Wh capacity. Good for phones, radios, and LED lights only.
- **$200-500:** 500-700Wh. Covers most basic emergency needs for a small household.
- **$500-1,000:** 1,000-1,500Wh. Can run a CPAP, small fans, and charge multiple devices daily.
- **$1,000+:** 2,000Wh+. Can handle small appliances, multiple medical devices, and extended outages.

---

## Solar Panels for Emergency Use

### Panel Types

| Type | Efficiency | Weight | Durability | Best For |
|------|-----------|--------|------------|----------|
| **Monocrystalline** | 20-23% | Moderate | Excellent | Best overall performance |
| **Polycrystalline** | 15-18% | Moderate | Good | Budget-friendly |
| **Flexible/thin-film** | 10-13% | Light | Fair | Portable/backpack use |
| **Foldable portable** | 18-22% | Light | Good | Emergency kits, mobility |

### Sizing Your Solar Panel

**The key formula:**

```
Panel Wattage Needed = Daily Wh Consumption / Peak Sun Hours / 0.8
```

**Peak sun hours** vary by location and season:
- **Southwest US (summer):** 6-7 hours
- **Midwest US (summer):** 5-6 hours
- **Northeast US (summer):** 4-5 hours
- **Winter (most areas):** 2-4 hours
- **Overcast days:** 1-2 hours (significantly reduced)

**Example:** You need 200Wh/day and get 4 peak sun hours:
```
200 / 4 / 0.8 = 62.5 watts minimum
```
A 100W panel gives you a comfortable margin.

### Panel Placement and Angles

**Optimal placement:**
- Face panels **due south** (in Northern Hemisphere)
- Angle equals your **latitude** for year-round average
- In **summer**, reduce angle by 15 degrees
- In **winter**, increase angle by 15 degrees
- Adjust every 2-3 hours to track the sun if possible

**Practical tips:**
- Avoid **any shade** -- even partial shade on one cell dramatically reduces output
- Place on a south-facing roof, or prop on the ground with a makeshift stand
- Keep panels **clean** -- wipe with a soft cloth regularly
- Snow reflects light and can actually boost output when panels are clear

| Your Latitude | Winter Angle | Summer Angle | Year-Round Average |
|---------------|-------------|-------------|-------------------|
| 25 degrees (South FL) | 40 degrees | 10 degrees | 25 degrees |
| 35 degrees (Memphis) | 50 degrees | 20 degrees | 35 degrees |
| 40 degrees (Denver) | 55 degrees | 25 degrees | 40 degrees |
| 45 degrees (Minneapolis) | 60 degrees | 30 degrees | 45 degrees |

---

## Battery Types for Solar Storage

### Comparison

| Battery Type | Cost | Lifespan (cycles) | Weight | Temperature Tolerance | Maintenance |
|-------------|------|-------------------|--------|----------------------|-------------|
| **LiFePO4** | High | 2,500-3,500 | Low | Good | None |
| **Lithium-ion (NMC)** | Moderate | 500-800 | Low | Fair | None |
| **AGM (sealed lead-acid)** | Low | 300-500 | Heavy | Good | None |
| **Flooded lead-acid** | Lowest | 500-1,000 | Heavy | Good | Regular (water levels) |
| **Gel lead-acid** | Moderate | 500-800 | Heavy | Good | None |

### Recommendations by Use Case

- **Portable emergency kit:** LiFePO4 power station (best weight-to-capacity ratio, longest lifespan)
- **Budget home backup:** AGM batteries with a charge controller and inverter
- **Long-term off-grid setup:** LiFePO4 battery bank (highest lifetime value despite upfront cost)
- **Temporary/short-term use:** Standard lithium-ion power station (lowest upfront cost)

### Important Battery Rules

- **Never discharge lead-acid batteries below 50%** (damages the battery permanently)
- LiFePO4 can safely discharge to **20%** regularly
- Store batteries in a **cool, dry location** (extreme heat shortens lifespan)
- Keep terminals clean and connections tight
- **Never mix battery types** or old and new batteries in a bank

---

## Connecting Solar Panels to Power Stations

### Direct Connection

Most portable power stations accept solar input via:
- **MC4 connectors** (industry standard for solar panels)
- **Anderson Powerpole connectors**
- **Proprietary connectors** (some brands use their own)

**Steps:**
1. Check your power station's **solar input voltage range** (e.g., 12-45V)
2. Ensure your panel's **open-circuit voltage (Voc)** is within that range
3. Connect panel to power station using the correct cable/adapter
4. Place panel in direct sunlight
5. Verify the power station shows charging

### Using a Charge Controller (Larger Systems)

For systems with separate batteries (not all-in-one power stations):

- **PWM charge controller:** Simpler, cheaper, less efficient. Fine for small systems under 200W.
- **MPPT charge controller:** More expensive, 15-30% more efficient. Recommended for systems 200W+.

**Basic wiring order:**
1. Connect charge controller to battery **first**
2. Then connect solar panels to charge controller
3. Disconnect in reverse order (panels first, then battery)

---

## Realistic Expectations

### What Solar Can and Cannot Do

**Solar CAN reliably power:**
- Phone and tablet charging
- LED lighting
- Portable radios and communication devices
- Small fans
- CPAP machines (with adequate battery)
- Laptop computers (with adequate battery)
- Small 12V refrigerators (with a large enough system)

**Solar CANNOT practically power (with portable systems):**
- Full-size refrigerators (requires 1,000Wh+ daily)
- Air conditioning
- Electric stoves/ovens
- Electric water heaters
- Space heaters
- Well pumps (possible with large dedicated systems)

### Weather Impact

| Conditions | Expected Output |
|-----------|----------------|
| Full sun | 80-100% of rated watts |
| Light clouds | 50-70% |
| Overcast | 15-30% |
| Heavy overcast/rain | 5-15% |
| Snow (panels clear) | 80-100% (reflection can help) |

**Plan for worst case.** Size your battery to carry you through 2-3 cloudy days without a full recharge.

---

## Maintaining Solar Equipment

### Solar Panels

- **Clean regularly** with water and a soft cloth (no abrasive cleaners)
- **Inspect wiring and connectors** for damage, corrosion, or loose connections
- **Check for physical damage** (cracks, delamination, discoloration)
- **Store folding panels** flat or loosely rolled, never sharply creased

### Power Stations and Batteries

- **Charge to 50-80%** for long-term storage (LiFePO4 and lithium-ion)
- **Recharge every 3-6 months** during storage to prevent deep discharge
- **Keep firmware updated** if your power station has update capability
- **Store in a climate-controlled space** when possible (avoid garages in extreme heat/cold)
- **Test under load quarterly** to verify capacity has not degraded

---

## Checklist: Emergency Solar Setup

### Essential Equipment

- [ ] Portable power station (500Wh minimum recommended)
- [ ] Solar panel (100W minimum recommended)
- [ ] Correct cables and adapters to connect panel to power station
- [ ] USB cables for all your devices
- [ ] 12V car adapter cables (if needed)
- [ ] Extension cord rated for your power station's output

### Knowledge

- [ ] Know your daily power consumption in Wh
- [ ] Understand your panel's optimal angle for your latitude
- [ ] Know the solar input specs for your power station
- [ ] Have practiced setting up and connecting your system
- [ ] Know which devices to prioritize when power is limited

### Maintenance Schedule

- [ ] Monthly: Visual inspection of panels and cables
- [ ] Quarterly: Full charge and discharge test of power station
- [ ] Quarterly: Clean panel surfaces
- [ ] Annually: Test all connectors and replace damaged cables
- [ ] Annually: Verify full system output matches rated specs
- [ ] Every 3 months during storage: Recharge batteries to 50-80%

---

## Quick Reference: Emergency Charging Times

**Using a 100W solar panel in full sun:**

| Device | Battery Size | Approximate Charge Time |
|--------|-------------|------------------------|
| Smartphone | 4,000 mAh | 1-2 hours |
| Tablet | 8,000 mAh | 2-4 hours |
| Power bank (20,000 mAh) | 74Wh | 1-1.5 hours |
| Laptop | 50-60Wh | 1-1.5 hours |
| 500Wh power station | 500Wh | 6-8 hours |
| 1,000Wh power station | 1,000Wh | 12-15 hours |

**Note:** These times assume direct connection and full sun. Real-world conditions with clouds and suboptimal angles will increase charge times by 30-100%.

---

*Last updated: March 2026*
*License: CC-BY-SA 4.0*
