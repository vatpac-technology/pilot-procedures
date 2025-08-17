---
  title: Terminal Areas
---

--8<-- "includes/abbreviations.md"

## Class C
### First Contact
On first contact with a terminal controller (generally 'Approach' or 'Departures'), **inbound** aircraft must report their assigned level, in-flight conditions, and the ATIS identifier.

!!! note "Format"
    "<span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Cleared Level</span>, <span class='optional'>[Visual]</span>, received <span class='placeholder'>ATIS Code</span>"

!!! example
    "Sydney Approach, QFA426, descending to `A090`, received Delta"

On first contact with a terminal controller, **outbound** aircraft must report their passing level, assigned level, and assigned heading/departure instructions (if applicable).

!!! note "Format"
    "<span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='optional'>[<span class='placeholder'>Departure Instructions</span>]</span>, passing <span class='placeholder'>Passing Level</span>, climbing to <span class='placeholder'>Assigned Level</span>"

!!! example
    "Melbourne Departures, QLK78D, turning right heading 320, passing `A023`, climbing to `A050`"

### SIDs/STARs
Aircraft on a SID/STAR will generally be given climb/descent instructions using *'climb via SID to (Level)'* and *'descend via STAR to (Level)'* phraseology. Pilots must readback the instruction exactly as it is issued. Once all height/speed restrictions have been passed, controllers may use traditional climb/descent phraseology.

!!! warning "Important"
    If an aircraft is cleared via a SID or STAR and the controller issues a climb or descent without the *'climb via SID'* or '*descend via STAR'* phraseology, this does **not** cancel any applicable SID/STAR restrictions. Pilots must continue to comply with all speed, level, and lateral tracking restrictions on the procedure.

!!! example
    "JST881, climb via SID to `F280`"

#### Cancelling Restrictions
Where a controller wishes to cancel the published altitude restrictions on a SID/STAR, they will use the following format.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, cancel level restrictions"

Where a controller wishes to cancel the published speed restrictions on a SID/STAR, they will use the following format.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, cancel speed restrictions"

### Approaches
#### Instrument Approaches
Aircraft cleared for an instrument approach in CTA will be issued a clearance of the following format.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, cleared <span class='placeholder'>Approach Type</span> approach runway <span class='placeholder'>Runway Number</span>"

!!! example
    "QJE1535, cleared ILS approach runway 27"

#### DGAs
Aircraft cleared for a DGA in CTA will be issued a clearance of the following format.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, cleared <span class='optional'>[DME or GNSS]</span> arrival <span class='optional'>[sector <span class='placeholder'>Sector Letter</span>]</span>"

!!! example
    "QLK72, cleared DME arrival sector Bravo"

#### Visual Approaches
Aircraft cleared for a visual approach in CTA will be issued a clearance of the following format.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, <span class='optional'>[<span class='placeholder'>Circuit Join Instructions</span>]</span>, cleared visual approach <span class='optional'>[tracking via the STAR]</span>"

It is important to note the difference between a **join** instruction and a **track to** instruction.

| Instruction | Meaning |
| ---- | --- |
| **Join** final | Continue on your cleared track until within 5nm of the aerodrome (by day), then join final |
| **Track to** final | Track now from your present position direct to the final leg of the circuit |

!!! example
    "RXA4847, join downwind runway 05, cleared visual approach"  

    "QFA881, cleared visual approach tracking via the STAR"  

    "LKU, track to a 5nm final, cleared visual approach"

#### Leaving CTA
At aerodromes with low overlying CTA (like YMAV during tower closed operations), the terminal controller will issue a clearance to leave CTA on descent via the instrument approach. As with any other approach clearance, this constitutes a clearance to *re-enter* CTA following the published missed approach in the event of a go around.

!!! example
    "JST607, cleared to leave controlled airspace descending via the ILS approach runway 18, no reported IFR traffic, report clear of the runway"

## Procedural Class D
### Inbound Call
On first contact with a procedural approach unit (e.g. procedural towers), report your position, assigned level, in-flight conditions, and the ATIS identifer.

!!! note "Format"
    "<span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Distance</span> miles <span class='placeholder'>Aerodrome Name</span>, <span class='placeholder'>GNSS Track/VOR Radial</span>, <span class='placeholder'>Assigned Level</span>, <span class='optional'>\[Visual]</span>, <span class='placeholder'>ATIS Code</span>"

!!! example
    "YCFS Tower, RXA6416, 32 miles Coffs Harbour on the 189 radial, descending to `A080`, visual, received Oscar"

### Departure Report
Once established on your outbound track (or in compliance with your assigned departure procedure), report your departure to the tower controller.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, tracking <span class='optional'>[<span class='placeholder'>Outbound Track</span> or via <span class='placeholder'>SID</span>]</span>, climbing to <span class='placeholder'>Assigned Level</span>"

!!! example
    "RXA6417, tracking 203, climbing to `A070`"  

    "XEB, tracking via the DUGGI ONE departure, climbing to `A070`"

### Approaches
There is no difference in phraseology used to clear an aircraft for an approach in Class C or Class D airspace, however due to airspace and surveillance coverage constraints, the controller may issue additional report requirements and/or clear aircraft to leave and re-enter CTA on descent prior to commencing the approach.

See [Class C](#approaches) for radio phraseology.