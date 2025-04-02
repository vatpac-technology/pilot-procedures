---
title: IFR Enroute Navigation
---

--8<-- "includes/abbreviations.md"

## Track Keeping
Ensure you remain within any applicable navigation tolerance and utilise any automation which can assist with flying the aircraft. If you notice you’re off track, take immediate action to correct it and notify ATC.

Generally speaking, you should use the most precise navigation system available to you. The order of precision is as follows:  

1. Localiser  
2. GNSS  
3. VOR  
4. NDB  

## Area Navigation
The vast majority of navigation is performed using an area navigation system like GNSS. This should be supplemented with ground-based aids and your position should be cross-checked as often as practical. Additionally, after passing each waypoint, you should cross-check the programmed track and distance to the next waypoint against your flight plan, to ensure that the aircraft is navigating along the predicted path.

## Position Fixing
A positive fix is a confirmed position of your aircraft. You can get a positive fix by:

- Station passage of a navigation aid like an NDB, VOR, or DME
- Intersecting two or more position lines (like radials from VORs) that cross at a sufficiently large angle (at least 45°)
- Using an area navigation system, like GNSS

IFR aircraft are required to obtain a positive fix at least every **two hours**, unless navigating by reference to an area navigation system.

### Station Passage
Station passage occurs when your aircraft flies directly overhead a navigation aid like a VOR, NDB, or DME. This indicates you've passed the aid and need to switch to the next leg of your route.  

Some aids will produce a 'cone of confusion' directly overhead, which creates a small area where no signal is received. This will likely result in your CDI flagging and any readings disappearing.

Station passage is indicated differently for different navaids:

| Navaid | Indication |
| ---- | ---- |
| VOR | TO-FROM flag changing, cone of confusion |
| NDB | Bearing needle swinging rapidly to indicate the station's position as being behind you |
| DME | Distance reading reducing to slightly above zero (a number representing your altitude in nautical miles), then increasing |


## Navaid Ranges
### VOR
Unless otherwise notified, each VOR has the same approximate range, dependent on aircraft altitude above the station.

| Aircraft Altitude (ft) | Approximate Range (nm) |
|------------------------|------------------------|
| 1,000                  | 40                     |
| 5,000                  | 85                     |
| 10,000                 | 120                    |
| 20,000                 | 175                    |

### NDB
Each NDB transmits at a different power, resulting in a different range. Due to the way the signal propagates, some stations may have different ranges during the day and night, or in different directions.

Each station's range is listed in the ERSA entry for the airport.

## LSALT
The LSALT is the lowest altitude which ensures you are safely above any terrain or obstacles along your route. You must always plan to remain above the LSALT, unless visual by day, using a NVIS, in the process of arriving or departing an aerodrome, or being radar vectored by ATC.

Various types of LSALT exist:

| Type | Explanation |
| --- | ---- |
| Route LSALT | Calculated from the enroute or terminal area charts for a published airway |
| Grid LSALT | A grid square on an ERC or TAC, covers a wider area than a Route LSALT |
| Aerodrome MSA | Published for aerodromes with instrument approach procedures, depicted on DAP charts and providing a high resolution, sector-based LSALT |
| Pilot Calculated LSALT | A custom level calculated by the pilot by considering the highest terrain & obstacle levels along a desired track, with allowances for the navigational tolerances of the navaid in use |

!!! note
    Published Route LSALTs assume a navigational tolerance of RNP2.

### Pilot Calculated LSALT
Pilot Calculated LSALTs are primarily used to allow smaller aircraft to fly lower, often avoiding icing conditions. Calculating them is complicated and covered by the AIP.

When referring to an altitude which uses a pilot calculated LSALT, the phrase *'pilot calculated'* should be appended to the level.

!!! example
    **DFR**: "DFR, climbing to A048 pilot calculated"  
    **BLA**: "DFR, no reported IFR traffic"

### Visual Below the LSALT
When visual by day, you may maintain visual separation with the terrain and any obstacles, and descend below the LSALT. If ATC instructs you to descend below the applicable LSALT in CTA in this manner, they will append the phrase *'visual'* to any level instruction. This must be read back in the same manner.

!!! warning "Important"
    You must not accept a visual level unless you have reported visual to ATC and are assured that you can maintain ongoing visual reference to the ground or water.

!!! example
    **SAS**: "FD203, descend to A015 visual"  
    **FD203**: "Descend to A015 visual, FD203"

### NVIS Operations
Pilots may descend below the LSALT when clear of cloud by night, provided they are using NVIS. This is most common with military and special operations aircraft. When referring to an altitude below the LSALT at night where the pilot will maintain visual separation with the terrain & obstacles using NVIS, the phrase *'NVIS'* should be appended to the level.

!!! example
    **RSCU206**: "RSCU206, descending to A033 NVIS"  
    **BLA**: "RSCU206, no reported IFR traffic"