---
  title: Alternate Requirements
---

--8<-- "includes/abbreviations.md"

## Introduction
An alternate aerodrome is an aerodrome nominated by the pilot at the flight planning stage which will be used as a divert point should the planned destination become unsuitable for any reason. In the real world, there are many reasons why an alternate may need to be carried. This page simplifies some of the real world rules and highlights the ones which are applicable for VATSIM operations.

Any alternate you nominate must not, itself, require an alternate.

## Alternate due Weather
When planning a flight, make careful study of your destination's TAF and take note of the cloud, visibility, and wind during the period of **30 minutes either side of your ETA** (60 minute window). Compare the forecast values with the alternate minima described below. If a TAF is not available for your arrival window, you must hold an alternate.

You must plan an alternate (or carry sufficient holding fuel, see [Fuel Planning](fuelplanning.md)) if:

- There is **more than scattered cloud** below the alternate minima, or
- The **visibility is less** than the alternate minima, or
- The **wind (including any gusts) exceed** the aircraft's crosswind or tailwind limitations, or
- The forecast indicates **thunderstorms or their associated severe turbulence**

!!! note
    When calculating the amount of cloud at a given level, the following rules apply:

    - FEW plus FEW equals SCT
    - FEW plus SCT equals BKN

!!! tip
    You can access TAFs and METARs for your departure & destination airports (as well as all available charts) using VATPAC's Pilot Assist tool.

### VFR Alternate Minima
The VFR alternate minima, by both day and night, is as follows:

| Cloud | Visibility |
| ----- | ---------- |
| 1,500ft AGL | 8km |

For helicopters operated under Day VFR to an uncontrolled (Class G) aerodrome, the alternate minima is reduced to:

| Cloud | Visibility |
| ----- | ---------- |
| 1,000ft AGL | 3km |

!!! note
    An alternate is not required if you are flying under Day VFR and plan to remain within 50nm of the departure aerodrome.

### IFR Alternate Minima
The IFR alternate minima is described on any approach chart for that aerodrome. The figures are formatted as cloud height above ground level and visibility in kilometres.

!!! example
    An alternate would be required for a Category C aircraft landing at Adelaide (YPAD) with more than scattered cloud below **1,480ft AGL** and/or visibility below **6.0km**.
    <figure markdown>
    ![Adelaide Alternate Minima (example only, not for operational use)](img/ypadminima.png){ width="700" }
      <figcaption>Adelaide Alternate Minima (example only, not for operational use)</figcaption>
    </figure>

!!! note
    See [Aircraft Categories](#aircraft-categories) below to determine your aircraft's category. 

If your destination does not have an instrument approach, you must plan an alternate if the forecast indicates weather conditions below:

| Cloud | Visibility |
| ----- | ---------- |
| LSALT +500ft | 8km |

## Alternate due Navaids
### IFR
An alternate must be held for IFR flights if due to the aircraft's equipment or the destination aerodrome's navigation aids, a single point of failure in the aircraft or on the ground would cause a loss of approach capability. In practice, this means that if your destination has only a single approach type available or your aircraft has only a single piece of equipment which can receive that data, you must carry an alternate.

!!! example
    Flying a King Air (with a single GNSS, and multiple VHF NAV & ADF equipment onboard) to Orange (YORG), which has published RNP approaches but no ground based aids, would require an alternate, as a loss of RAIM or GNSS integrity would result in the aircraft being unable to conduct an approach.  

    Flying a C172 (with a single GNSS and a single VHF NAV) to Sydney (YSSY) would *not* require an alternate, as a failure of a single piece of equipment in the aircraft (e.g. the GPS) or on the ground (e.g. the ILS) would not prevent the aircraft from conducting an approach (they could still utilise the RNP or ILS approach, depending on the source of failure).

### Night VFR
An alternate, within 1 hour flying time, is required for Night VFR flights unless:

- The aircraft is equipped with GNSS, or
- The destination is served by a ground-based navaid which the aircraft has equipment to receive

## Aircraft Categories
Aircraft are grouped into categories for the purpose of flight planning and terminal procedure design. Some aircraft can be operated in multiple categories based on operator preference, but for simplicity, it is sufficient to choose the category which best reflects the average day-to-day operation using the table below.

| Category | Final Approach Speed | Example |
| -------- | -------------------- | ------- |
| A | up to 90 KIAS | Cessna 172 |
| B | 91 to 120 KIAS | Beechcraft King Air |
| C | 121 to 140 KIAS | SAAB 340 |
| D | 141 to 165 KIAS | Airbus A380 |
| E | 161 to 210 KIAS | Something huge! |
| H | N/A | Helicopters |