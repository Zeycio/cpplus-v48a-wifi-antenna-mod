# CP Plus V48A — External Wi-Fi Antenna Range Mod

A DIY guide to extending the Wi-Fi range of a **CP Plus V48A** Wi-Fi CCTV camera by
tapping the on-board antenna feed and adding an external **2.4 GHz RP-SMA antenna**.

https://zeycio.github.io/cpplus-v48a-wifi-antenna-mod/

---

## ⚠️ Before you start

- **Unplug the camera** — never work on it powered.
- Opening the housing **voids the warranty** and can permanently damage the board.
- Soldering = hot iron + fumes. Work in a ventilated space.
- The Wi-Fi front-end is static-sensitive — work grounded (ESD-safe).
- Only modify hardware you own. **You do this entirely at your own risk.**

---

## 🧰 Bill of materials

**Parts**
1. 2.4 GHz Wi-Fi antenna (RP-SMA "rubber duck" type)
2. RP-SMA bulkhead pigtail (panel-mount jack + short coax lead)
3. Thin rosin-core solder
4. Heat-shrink / hot glue (optional — insulation & strain relief)

**Tools**
- Small Phillips screwdriver
- Fine-tip soldering iron (+ flux)
- Sharp blade / scraper (to remove solder mask)
- Drill or rotary tool (small bit)
- Multimeter (optional — check for shorts)

---

## 🔧 Procedure

1. **Open the housing** — unplug the camera, then open it from the *front*; remove
   screws until the mainboard is exposed. Keep the screws in order.
2. **Find the Wi-Fi feed** — locate the printed Wi-Fi (📶) symbol on the mainboard;
   it marks the L-shaped copper feed trace of the on-board antenna.
3. **Expose the trace** — gently scrape the solder mask off the L-trace until clean
   copper shows (don't cut through it). Expose a nearby ground patch too.
4. **Prep the pigtail** — separate the coax into centre **core** (signal) and outer
   **shield** (ground); keep leads short and tin them.
5. **Solder** — core → the exposed L-trace feed, shield → ground. Keep leads short;
   make sure core and shield never touch (no short).
6. **Mount the connector** — drill a hole in the back of the housing and secure the
   RP-SMA jack with its nut/washer.
7. **Test first** — attach the external antenna, power up, connect in the app, and
   confirm it links/streams with improved range **before** closing it up.
8. **Reassemble or troubleshoot** — if it works, reassemble with strain relief. If
   not, check for shorts, cold joints, a damaged trace, or pinched wires; fix & retest.

**Tips:** keep the coax stub short (2.4 GHz cares about length/impedance); seal the
new rear hole against water (outdoor camera); optionally cut the internal-antenna
trace for a cleaner RF path if you know what you're doing.

---

## 📷 Photos

Drop your build photos into the [`images/`](images/) folder using the exact filenames
listed in [`images/README.md`](images/README.md). The website will show them
automatically; until then it shows labelled placeholders.

---

## 📝 License

Released under the [MIT License](LICENSE). "CP Plus" and "V48A" are used only to
identify the device; this project is unofficial and not affiliated with or endorsed
by the manufacturer.
