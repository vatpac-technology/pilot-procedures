---
  title: Controlled Aerodromes
---

--8<-- "includes/abbreviations.md"

## Airways Clearance
### Route Clearances
!!! note "Format"
    "*(ATC Unit)*, *(Callsign)*, to *(Destination)*, request clearance"

ATC will respond with an airways clearance. During your readback, you should advise them of your parking bay (if known).

!!! example
    *QFA421 is an IFR B738*  
    **QFA421**: "Sydney Delivery, QFA421, to YMML, request clearance"  
    **SY ACD**: "QFA421, cleared to YMML via WOL, flight planned route, runway 16R, GROOK1 departure WOL transition, climb via SID to A050, squawk 3231, departure frequency 129.7"  
    **QFA421**: "Cleared to YMML via WOL, flight planned route, runway 16R, GROOK1 departure WOL transition, climb via SID to A050, squawk 3231, departure frequency 129.7, bay 3, QFA421"  

    *TEK is a VFR Cherokee*  
    **TEK**: "Sydney Delivery, TEK, to YCNK, request clearance"  
    **SY ACD**: "TEK, cleared to YCNK via SYHD, flight planned route, runway 16L, climb to A035, squawk 0542, departure frequency 123.0"  
    **TEK**: "Cleared to YCNK via SYHD, flight planned route, runway 16L, climb to A035, squawk 0542, departure frequency 123.0, TEK"

### Circuits
!!! note "Format"
    "*(ATC Unit)*, *(Callsign)*, for circuits, request clearance"

In response, ATC will issue a clearance to operate in the circuit area, not above an appropriate altitude. A squawk code will not always be issued.

!!! example
    **LKU**: "Melbourne Delivery, LKU, for circuits, request clearance"  
    **ML ACD**: "LKU, cleared to operate in the circuit area, not above A020, squawk 0100"  
    **LKU**: "Cleared to operate in the circuit area, not above A020, squawk 0100, LKU"

### PDCs
A PDC may be issued over text by a controller to assist with their workload. In Australia, a PDC **must be read back on frequency**.

When reading back a PDC, only the following items must be transmitted by the pilot:

- SID (including transition, if applicable)
- Squawk Code
- Parking Bay

!!! warning "Important"
    Advise the controller of your intention to readback your PDC by establishing contact with them first, to allow them to cross-check your readback against your flight data record.

!!! example
    **VOZ723**: "Sydney Delivery, VOZ723, PDC readback"  
    **SY ACD**: "VOZ723"  
    **VOZ723**: "GROOK1 departure, WOL transition, squawk 4412, bay 32, VOZ723"  

## Pushback & Engine Start
### Engine Start
Authorisation to commence engine start is generally not required, unless advised on the ATIS, the ERSA, or [Local Procedures](../../local-procedures/).

!!! note "Format"
    "*(ATC Unit)*, *(Callsign)*, *(Parking Position)*, request engine start"

### Pushback
!!! note "Format"
    "*(Callsign)*, *(Parking Position)*, request pushback"

## Taxi
### Fixed Wing
!!! note "Format"
    "*(Callsign)*, *(ATIS Code)*, request taxi, *[(Desired Holding Point)]*"

In response, ATC will provide taxi instructions to the runway or to an intermediate point if required. Where unrestricted taxi to the runway (or your parking bay) is not immediately available, you may receive instructions to hold short of a position or give way to other aircraft.

!!! example
    **JST512**: "JST512, received F, request taxi, holding point B4 or better"  
    **SY SMC**: "JST512, taxi via B4, hold short of B"  
    **JST512**: "Taxi via B4, hold short of B, JST512"

    **SY SMC**: "JST512, give way to the Qantas 737 northbound on B, taxi to holding point B4, runway 16R"  
    **JST512**: "Give way to the Qantas 737, taxi to holding point B4, runway 16R, JST512"

### Helicopters
Helicopters can either ground taxi, air taxi, or air transit around an aerodrome.

| Taxi Technique | Meaning |
| -------------- | ------- |
| Ground Taxi | Traditional taxi using an aerodrome's taxiways, by helicopters equipped with wheels |
| Air Taxi | Transit of a helicopter in ground effect and at less than 20kt |
| Air Transit | Expeditious transit of a helicopter at or below 100ft AGL and at speeds greater than those during air taxiing |

Helicopter pilots should generally nominate which method they would like to use, however air transits may not always be available.

!!! example
    **HSZ**: "Bankstown Ground, helicopter HSZ, taxiway F, for the main pad, received V, request air taxi"  
    **BK SMC**: "HSZ, air taxi to the main pad"  
    **HSZ**: "Air taxi to the main pad, HSZ"
  
## Takeoff & Landing
### Reporting Ready
After receiving unrestricted taxi instructions to the holding point and after completing all necessary pre-takeoff checks, report 'ready' to ADC.

!!! note "Format"
    "*(ATC Unit)*, *(Callsign)*, ready"

!!! warning "Important"
    In Australia, only international aircraft will be explicity transferred from SMC to ADC (and vice versa). Domestic aircraft should switch to the ADC frequency without direction from SMC when approaching the instructed holding point and when ready for departure.

### Takeoff Clearance
ATC may provide departure instructions with a takeoff clearance, including an assigned heading or a turn instruction.

!!! example
    "RXA6166, assigned heading left 230, runway 34L, cleared for takeoff"

!!! warning "Important"
    You must obtain departure instructions prior to commencing your takeoff roll if you have been cleared via a radar SID. If ATC fails to provide relevant instructions, it is your responsibility to query them.

### Landing Clearance
ATC may provide runway vacating instructions, wind information, and/or other relevant information with a landing clearance.

!!! example
    **SY ADC**: "QLK52D, the crossing runway is available to vacate, wind 180 degrees at 18kt, runway 16R, cleared to land"  
    **QLK52D**: "16R, cleared to land, QLK52D"

### Outside the Manoeuvring Area
Helicopters and some light aircraft may operate from areas outside the manoeuvring area, such as hospital helipads or small airstrips inside the CTR, or other locations on the aerodrome. A takeoff/landing clearance **will not** be provided in these situations but approval must be sought to become airborne inside the control zone.

After obtaining an airways clearance, ATC will instruct you to *'report airborne'* or *'report on the ground'*.

!!! example
    *RSCU201 is a VFR helicopter at St George Hospital (inside the Sydney CTR)*  
    **RSCU201**: "Sydney Tower, helicopter RSCU201, St George Hospital, for YSBK, received F, ready"  
    **SY ADC**: "RSCU201, cleared to YSBK direct, climb to A015 visual, squawk 0466, report airborne"  
    **RSCU201**: "Cleared to YSBK direct, climb to A015 visual, squawk 0466, RSCU201"  

    **RSCU201**: "RSCU201, airborne"

!!! example
    *YOE is a VFR helicopter inbound on the Maroubra inbound helicopter route to YSSY*  
    **YOE**: "Sydney Tower, helicopter YOE"  
    **SY ADC**: "YOE, Sydney Tower, cleared visual approach to H8, report on the ground"  
    **YOE**: "Cleared visual approach to H8, YOE"  

    **YOE**: "YOE on the pad"

## Circuits
### Takeoff Clearance
Unless it is implied by runway configuration or ERSA/[Local Procedure](../../local-procedures/), circuit direction will be nominated with takeoff clearance.

!!! example
    "LKU, make left circuit, runway 29L, cleared for takeoff"

### Downwind report
You must report downwind on each circuit, to advise ATC of your intentions.

!!! note "Format"
    "*(Callsign)*, downwind, *(Intentions)*"

| Intention | Meaning |
| --------- | ------- |
| Touch and Go | Conduct a touch and go |
| Full Stop | Conduct a full stop landing |
| Stop and Go | Land, come to a complete stop, then commence takeoff roll without vacating |
| *(Details)* Departure | After a touch and go, depart the circuit area as described |
