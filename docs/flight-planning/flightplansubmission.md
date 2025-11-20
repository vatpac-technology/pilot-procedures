---
  title: Flight Plan Submission
---

--8<-- "includes/abbreviations.md"

A flight plan should be submitted for all IFR flights, and VFR flights inside CTA or with the intention of requesting flight following. A flight plan is not required for local aerodrome operations like circuits.

!!! tip
    ATS can create a flight plan for you if required, however this will involve detailing all aspects of your aircraft and intended flight over the radio. In the majority of cases, it is simplier to file a flight plan yourself.

## Callsigns
When filing and connecting as an aircraft belonging to an established operator (such as an airline), pilots should use the **three letter ICAO** operator prefix, *not the two letter IATA* code.

!!! example
    To connect as a Qantas aircraft, the three letter ICAO identifier **QFA** should be used, not the two letter ICAO code **QF**.

Any ICAO operator callsign can be used. A list of further approved callsigns (including local aeromedical, general aviation, and Defence callsigns) is available in [Radio Telephony](../radio-telephony/operatorcallsigns.md).

!!! tip
    If you are using a callsign which is foreign to Australia (or refers to a virtual airline or other lesser known operator), the actual callsign name should be included in your [flight plan remarks](#radio-callsign).

When connecting as a general aviation aircraft (or operating the aircraft using its registration as your callsign), remove the hyphen which separates the registration prefix and suffix. The *'VH'* prefix should only be included for flights outside of Australian territory.

!!! example
    When operating **VH-CYF** wholly within Australian territory, the callsign **CYF** would be used (and filed on your flight plan).

    When operating outside of, entering, or leaving Australian territory, the callsign **VHCYF** would be used and filed.

## Aircraft Type
The full **ICAO** aircraft type code should be used on a flight plan.

!!! example
    A Boeing 747-400 would file using the aircraft type **B744**.

## EOBT
The estimated off-blocks time field is used by ATS software to order all submitted flight plans and aids controllers in estimating future workload. Additionally, invalid or nonsensical EOBT times may result in your flight plan being hidden from controllers due to the system assuming it is irrelevant.

Ensure that an appropriate EOBT is filed. Where unforeseen delays occur prior to departure, consider contacting the relevant ATS unit to amend your EOBT.

!!! example
    **VOZ1252**: "Sydney Delivery, VOZ1252, we'll be a bit delayed tonight, would you mind updating our EOBT to 0930?"

## Unrecognised Landing Areas
If your departure or destination does not have a recognised ICAO code, replace it with `ZZZZ` and include a remark with the position of the landing area. It is good practice to include an additional remark detailing the name of the landing area, for use on the radio if required.

**The format of your remarks field is important.** Ensure that you use the format shown below:

| Remark Abbreviation | Meaning |
| --- | --- |
| `DEP/<position>` | Position of departure aerodrome/landing area |
| `DEST/<position>` | Position of destination aerodrome/landing area |

See [Custom Waypoints](#custom-waypoints) for details on how to format custom positions.

!!! example
    **Departure**: `ZZZZ`  
    **Remarks**: `DEP/2730S15327E RMK/2730S15327E IS DUSTBOWL STATION`

## Equipment Codes
The equipment and transponder codes you file in your flight plan will impact how ATS process your navigation requirements, and control how you appear on their radar scope. **Equipment** codes refer to the navigational equipment your aircraft is equipped with. **Transponder** codes refer to the type of transponder and ADS-B system installed in your aircraft.

A full list of equipment codes can be obtained through various online sources (searching for *ICAO* equipment codes - not FAA), with the most commonly used summarised below:

| Equipment Code | Explanation |
| --- | --- |
| D | DME |
| E1 | FMC with ACARS |
| F | ADF |
| G | GNSS |
| L | ILS |
| O | VOR |
| S | Standard - ILS, VOR, VHF |
| T | TACAN |
| W | RVSM |

!!! example
    An aircraft equipped with GNSS, ILS, VOR, DME, and ADF receivers, VHF comms, and RVSM-compliant altimeters would file `SDFGW`.

| Transponder Code | Explanation |
| --- | --- |
| A | Mode A Transponder |
| B1 | ADS-B Out |
| B2 | ADS-B In/Out |
| C | Mode C Transponder |
| E | Mode S Transponder with ADS-B |
| G1 | ADS-C |

!!! example
    An aircraft equipped with a Mode S transponder which supports both ADS-B In and Out would file `EB2`

## Filed Route
The Route Details field should contain only the waypoints and airways you intend to fly. You should **not** include plain English items.

!!! failure "Wrong"
    **Route**: `VFR COASTAL`

!!! success "Correct"
    **Route**: `DCT` (or any other approximate known waypoint names)  
    **Remarks**: `COASTAL FLYING`
    
Whatever route you file in your flight plan **must match** what you load into your aircraft's FMS/GPS. Additionally, the route field should not include the departure and destination aerodrome codes, as these have dedicated fields.

!!! tip
    A common mistake made by pilots conducting circuits at an aerodrome is to file a flight plan containing the route `CCT` (or similar). ATS software converts the route into known waypoints and draws a route to Central City, USA, flagging the flight plan for all controllers along the way.

    For circuits, a flight plan is generally not required, however if a pilot wishes to file one, they should file a route of `DCT` and include a remark indicating their intention to conduct circuits.

### Custom Waypoints
Custom waypoints can be included in your route by referencing lat/long positions or bearing/distance information from a known waypoint.

Lat/long positions should take the format of: **DDHHCDDHHC**, where:

- **DD** = Degrees
- **HH** = Hours
- **C** = Cardinal direction (i.e. N, S, E, W)

!!! example
    The position **-32.7957, 151.8407** would be expressed as **3247S15150E**.

Positions can also be expressed with reference to a known position, using the format: **WPTBBBDDD**, where:

- **WPT** = Known waypoint code
- **BBB** = Bearing outbound from the known waypoint (as a three digit number)
- **DDD** = Distance from the known waypoint (as a three digit number)

!!! example
    A position **25nm on the 045 bearing** (northeast) from YSSY would be expressed as **YSSY045025**.

## Remarks
### Airwork and Planned Delays
During training or special operation flights, it may be necessary to conduct airwork at a predetermined position before continuing on your flight planned route. This should be indicated using the **DLE/<position><time>** format. Additionally, for practice instrument approaches or coded clearances, a remark should be included to dictate this request.

!!! example
    A pilot is conducting a training flight around the Melbourne Basin, with practice approaches at YMEN (for 10 min), YMAV (for 20 min) and YMMB (for 30 min).  
    **Filed Route**: `DCT ESDAN DCT AV DCT MB DCT`  
    **Remarks**: `DLE/ESDAN0010 AV0020 MB0030 RMK/ESDAN26ILS AV36VOR MBNDBA`

!!! example
    A pilot is conducting Search and Rescue operations within a 10nm radius of a position defined as **WG288030**, for 30 min.  
    **Filed Route**: `DCT WG288030 DCT`  
    **Remarks**: `DLE/WG2880300300 RMK/SAR OPERATIONS WI 10NM OF WG288030`

### Priority Status
When simulating special operations, you are permitted to file a priority status in your remarks using the **STS/<status>** format. This will control how your flight plan is displayed to controllers.

| Status | Meaning |
| --- | --- |
| `STS/MEDEVAC` | Aircraft engaged in life critical transportation of severely ill patients |
| `STS/HOSP` | Aircraft engaged in non-life-critical transportation of medical operations, personnel, or ill patients |
| `STS/FFR` | Aircraft engaged in Fire or Flood Relief operations |
| `STS/SAR` | Aircraft engaged in Search and Rescue Operations |
| `STS/HEAD STATE` | Aircraft carrying the Prime Minister |
| `STS/STATE` | Aircraft part of the defence force, military, or customs |

!!! note
    Under the VATSIM Code of Conduct, no flight may declare itself to have priority over another. Filing a priority status in your flight plan will not result in being prioritised above other aircraft (contrary to the real world), however it may signal ATS to provide track shortening or to facilitate your planned operations.

### Radio Callsign
Where an unusual or non-standard callsign has been filed (see [Callsigns](#callsigns)), include the full radio callsign in your remarks using the **RTF/<callsign>** format.

!!! example
    **Filed Callsign**: `YMA`  
    **Remarks**: `RTF/COMPASS`

### Voice Rules
At the bottom of the VATSIM flight plan form, you are able to select your voice rules. Ensure this is set correctly to minimise disruption to ATS. If necessary, you can update this during your flight by informing ATS. As per the [VATSIM Code of Conduct](https://vatsim.net/docs/policy/code-of-conduct), voice is the preferred method of communication on VATSIM. Account holders should use voice if able to do so but must accommodate the use of text to support those with a disability and are unable to utilize voice. Only unaltered speech is permitted to be transmitted.

| Option | Meaning |
| --- | --- |
| Voice | Able to send and receive voice communication |
| Text | Not able to send or receive voice communication, text communication required |
| Receive Only | Able to receive voice but only able to respond via text |

!!! warning "Important"
    Pilots - Shall be able to, at a minimum, receive voice but may send messages via text (Receive Only). Account holders with a disability who are unable to receive and/or transmit voice, such as due to a hearing disability, may use a lower level of voice capability but may be required to explain the inability to comply with this section to a VATSIM Supervisor upon request.