---
  title: Instrument Approaches
---

--8<-- "includes/abbreviations.md"

## Background
Instrument approaches provide a charted, surveyed path for aircraft to safely descend below the LSALT in adverse weather conditions or at night. They are also commonly flown during VMC to provide a stable, predictable flight path for the aircraft to follow.

The procedures are categorised as either [2D](#2d-approaches) or [3D](#3d-approaches), and can be flown as a runway aligned approach (terminating at a position from which the pilot can land on the aligned runway) or as a [circling approach](#circling-approaches).

!!! tip
    AIP ENR 1.5 details a number of IAP-relevant items and is suggested further reading for pilots who want to learn more about the rules which govern IFR flying in the real world.

### Charts
Charts for procedures in the Australian FIR are published by Airservices Australia (available for free on the AIP website) or by Jeppesen (available with the Navigraph subscription).

!!! tip
    VATPAC's [Chart Finder](https://vatpac.org/membership-hub/tools/charts){target=new} tool provides free, easy access to all Airservices Australia charts.

Each IAP chart features a description of the procedure (including relevant tracks and distances to be flown), navaid information, the minimum altitude to which the procedure may be flown, and the published missed approach to be followed in case a landing can't be carried out. Refer to the user guide of your chosen chart provider for details on interpreting each type of chart.

Any coded procedure in an aircraft's FMS or GPS should be cross-checked with the appropriate chart prior to commencing the approach. Additionally, the chart should be reviewed to identify the relevant details which will impact if/when a pilot will conduct a missed approach, and how they will manoeuvre the aircraft to land if they become visual.

### Descent Below the LSALT
There are a variety of situations where real pilots may descend below the LSALT, but for VATSIM purposes, the following simplification is sufficient:

> You must remain above the LSALT unless you are visual by day, under ATC control in controlled airspace, or conducting an instrument approach.

When utilising an IAP to descend below the LSALT, you must ensure that you track via an initial approach fix. In some situations, ATC will vector you to join the approach after the IAF in controlled airspace.

All ground-based navaids must be tuned and identified (using their morse code identifier or an appropriate aircraft system) prior to commencing the approach.

It may be necessary to apply a correction to the published minima, depending on the source of QNH used. See [Altimetry](../flight-planning/altimetry.md#instrument-approach-corrections) for more details.

## 3D Approaches
3D approaches provide both lateral and vertical guidance, and generally allow for a lower minima. The minima for 3D approaches is a 'Decision Altitude' which may reference either radio height (above the threshold elevation) or barometric altitude (AMSL).

### ILS/GLS
An ILS uses radio waves to transmit a localiser (lateral tracking) and glideslope (vertical tracking) path for an aircraft to follow. A GLS provides the same functionality but uses highly accurate GNSS to do so. The ILS frequency is tuned into a VHF Nav radio, while a GLS is setup through the aircraft's FMS or GPS system. An additional radio panel component may be present in some aircraft to enter the GLS code.

When ATC is providing vectors to intercept the LOC/FAC, expect to be established at least 2nm prior to the FAP.

### RNP (LNAV/VNAV)
An RNP (LNAV/VNAV) uses specialised aircraft equipment to produce a pseudo-glideslope for the aircraft to follow during an area-navigation-based approach (generally GNSS). 

## 2D Approaches
2D approaches provide lateral guidance only. The vertical profile must be maintained manually by the pilot during the approach. The minima for 2D approaches is a 'Minimum Descent Altitude' which may be maintained until reaching the missed approach point. If the pilot is unable to conduct a landing at that point, a missed approach must be carried out.

Most 2D approaches follow a 3° descent profile, with distance/altitude guidance tables to help pilots determine whether they are on profile. As a general rule of thumb, a 3° profile involves descending 320ft/1nm or 1,000ft/3nm. This makes determining whether you are on, above, or below profile easier.

!!! example
    The profile height of an aircraft on a **5nm** final is roughly **1,600ft**. If a pilot finds themselves at 1,520ft, they can determine that they are slighly below profile.

To maintain a 3° profile descent, pilots can determine the required vertical speed by multiplying their groundspeed by 5.

!!! example
    To maintain a 3° profile descent at **160kt**, a vertical speed of roughly **800fpm** is required.

### RNP
An RNP uses an aircraft's area navigation system (typically GNSS) to track via pre-programmed waypoints along a surveyed path. They are commonly flown at aerodromes not equipped with a 3D approach. Due to the varying position of real world satellites, pilots must ensure that a sufficient number of satellites will be within view of the aircraft prior to conducting an RNP approach using GNSS. This problem is rarely seen in a simulator.

You must commence an RNP approach from an IAF waypoint unless instructed by ATC in controlled airspace to join at the Intermediate Fix.

Each waypoint on an approach is named using a pre-defined format. The first 3 characters describe the location (and may include a version number), the 4th character describes the direction from the aerodrome, and the last character describes the waypoint type.

!!! example
    The Final Fix on the YSDU RNP RWY 05 is named `DBOWF`.  

    - **DBO** describes the aerodrome (Dubbo)
    - **W** describes the direction (west of the aerodrome)
    - **F** describes the waypoint type (Final Fix)

    The Initial Approach Fixes on the YMOR RNP RWY 19 are named `OR2NA`, `OR2NB`, and `OR2NC`. 

    - **OR2** describes the aerodrome (Moree) and the version number of the procedure design (2)
    - **N** describes the direction (north of the aerodrome)
    - **A/B/C** describes the waypoint type (Initial Approach Fix)

### LOC
A Localiser approach uses the lateral tracking guidance of the localiser beam without reference to the glideslope. They are generally flown when an ILS is partially unserviceable or where local terrain does not allow for a glideslope to be installed.

### VOR
A VOR approach uses a defined VOR radial which is established as the inbound approach course. VOR approaches may be joined from a variety of positions (as dictated by the chart), generally from:

- A position on the inbound radial
- Overhead the aid (involving an outbound radial and either a procedure turn or pilot-driven turn to intercept the inbound radial)
- A position on a DME arc (involving flying along the arc until reaching the inbound radial)

### NDB
An NDB approach uses the deflection of the ADF needle to track along a defined radial/bearing. Like VOR approaches, NDB approaches may be joined from a variety of positions.

- A position on the inbound radial
- Overhead the aid (involving an outbound radial and either a procedure turn or pilot-driven turn to intercept the inbound radial)
- A position on a DME arc (involving flying along the arc until reaching the inbound radial)

### DME/GNSS Arrivals (DGAs)
Whereas instrument approaches generally prescribe specific tracks to be flown, DGAs provide a variety of sectors for an aircraft to track via, allowing pilots to remain above the relevant MSA as they track towards a VOR or NDB. DGAs terminate in the circling area, requiring a [circling approach](#circling-approaches) unless the aircraft is able to complete a straight-in landing.

These arrivals give pilots flexibility to safely descend below the LSALT without having to manoeuvre to join an instrument approach, which saves time and fuel. Where manoeuvring is required during the arrival, it must be completed prior to the FAF. From the FAF, the aircraft must track direct to the navaid.

## Circling Approaches
Pilots must select the minima to which they will conduct an instrument approach. They have the option of completing an approach to the straight-in minima (and then conducting a straight-in landing) or to the circling minima (and manoeuvring within the circling area).

Aerodromes with circling approaches have surveyed circling areas, calculated by connecting arcs of a given radius from each usable runway threshold. Pilots will generally maintain the circling minima while they manoeuvre the aircraft inside the circling area to join the circuit. Once they are at a suitable point, they will commence descent in accordance with a normal circuit.

Some charts dictate 'No Circling Areas', where the normal circling height might not be sufficient to avoid terrain or obstacles. These areas *may* be entered by day only.

## Missed Approaches
For VATSIM purposes, a missed approach must be conducted any time an aircraft is:

- Not visual at the minima
- Loses visual reference with the runway environment in the circling area
- Unstable during the final segment of the approach
- Unable to complete the approach (due to navaid or aircraft system failure)

Unless visual by day, if a go around or missed approach is required, an aircraft conducting an instrument approach must conduct the published missed approach (as per the chart). 

!!! note
    A clearance to conduct an instrument approach in CTA constitutes a clearance to conduct the published missed approach. No additional clearance is required (including to re-enter CTA where the instrument approach procedure tracks the aircraft to leave CTA vertically or laterally).

    An explicit airways clearance **is** required if an instrument approach is commenced from OCTA and the published missed approach (or any other missed approach intentions) involve entering CTA.

Where a failure of the navaid or aircraft system renders the approach impossible to continue, the published missed approach should be carried out to the best of the pilot's ability (including dead reckoning where necessary).