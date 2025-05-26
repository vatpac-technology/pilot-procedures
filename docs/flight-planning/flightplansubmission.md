---
  title: Flight Plan Submission (TODO)
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

## Equipment Codes (TOD)

## Filed Route
- should mirror what you put in your FMS
- don't include plain english, only waypoint codes
- for things like CCTs, leave blank or DCT with remark

## Remarks
### Airwork and Planned Delays
- 'DLE/YMAV0020'
- 'RMK/AV ILS'
- 'RMK/HARBOUR SCENIC ONE'

### Priority Status
- MEDEVAC, FFR, etc

### Radio Callsign
RTF/QANTAS

### Voice Rules
- importance of selecting correct option for voice, text, receive only