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

## Pushback & Taxi
### Pushback

 `"[Callsign] request push"` <Sub> note in normal operations start approval is not explicitly required </Sub>

### Engine start

 **There is only one type of engine start that needs ATC clearance in Australia. This is a Cross-bleed start, only applicable to jets that need to start 1 engine on the bay with ground crew assistance prior to pushback.**
  ~~`"[Callsign], Bay [Number] request cross-bleed start and push"`~~

### Taxi

Request:`"[Callsign] with information [ATIS info] Ready for taxi [Runway]"`
  
 A taxi instruction will be laid out as follow, `"[Callsign] Taxi via [routing] to [Taxi limit/end]"`
 A clearance may advice you to Hold short, give way or cross a runway.
 
  - Hold short `"Hold short of [taxi way]"`
  - Hold short of runway `"... Holding point [Point] Runway [Identifier]"`
  - Give way `"...Give way to [Callsign/company] [Aircraft type]..."`
  - Runway crossings `"...on [taxi-way] cross [runway]..."` Alternatively `"...Cross [Runway]..."`
  
  Readback: Readback all instructions as they were issued to you. Pen and paper doesn't hurt.

## Takeoff & Landing
### Report Ready
  on first contact with Tower, or when ready to depart, ensure you report ready for departure. As tower can't issue a take-off clearance untill you do so. There are 2 methods of doing this. 
    
  You can either report that you will be ready when you reach the holding point with `"[Station] [Callsign] ready upon reaching [Holding point]"`

  Else you can report that you're ready when waiting at the holding point with `"[Station] [Callsign] Ready [Holding point]"`

### Take-off clearance
 As a general rule, a take-off clearance will only consist of  `"[callsign][runway],clear for take-off"`

How ever, there may be special requirements that need to be followed like `"[Callsign][Runway],Clear for Imidiate take-off/no delay"` Or, `"[Callsign] Assigned heading xxx/[special requirements],[Runway] Clear for take-off"`

With all clearances you are required to read back all special instructions/requirements. HOW EVER, if tower report new winds, winds readback not required.

Take-off readback should look like: `"Cleared for take-off [Sepcial instructions] [Callsign]"`

## Helicopter Operations
Helicopters have the fun little quirk of being able/having to leave the ground to get around, even away from the runway. There are 2 ways of completing this, either air taxi, or air transit. ATC will decide which is best in the senario, usually prioritising air taxi.

Heli pilots should be ready to either depart from their position or to manuver to a helipad/runway

Request:`"[Station][Callsign] Ready for departure."`

### Air taxi

A-Taxi clearance `"[Callsign] Airtaxi not above [Height] AGL, [Taxi instructions]"` (AGL standing for above ground level)

Readback:`"Cleared air taxi not above [Height], [Taxi instructions],[Callsign]"`

### Air Transit

A-Transit clearance`"[Callsign] Cleared air transit [destniation] not above [Height] AGL"`

Readback:`"Cleared Air transit [Destniation] not above [Height][Callsign]"`

## Circuits
You will know your circuit direction either from your clearance OR runway config, if there is any chance of missinterpretation tower will advise in take-off clearance. Tower may also specify "report downwind" as a reminder, how ever even if they don't specify this you must report downwind ALWAYS.
### Take-off clearance
Normal:`"[Callsign], runway [Identifier], clear for take-off"`
Specified:`"[Callsign], Make [direction] Circuit, report downwind, runway [identifier] clear for take-off"`

### Downwind report
<Sub>Reminder, you must always report turning onto or level on downwind with intentions </Sub>

Turn, Touch and Go:`"[Callsign], turning downwind [Runway], touch and go"`

Touch and Go:`"[Callsign] downwind [Runway] touch and go"`

Turn, Full Stop:`"[Callsign] turning downwind [Runway] full stop"`

Full Stop:`"[Callsign] downwind [Runway] Full stop"`

Departure (not previously discussed):`"[Callsign] downwind [Runway] for departue to [Point/Destniation]"`
