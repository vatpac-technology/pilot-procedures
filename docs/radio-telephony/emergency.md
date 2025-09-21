---
  title: Emergency
---

--8<-- "includes/abbreviations.md"

## Simulation of Emergencies
You are welcome to simulate a variety of emergencies in accordance with the VATSIM Code of Conduct, however during times of high workload, a controller may instruct you to cancel the emergency simulation or disconnect from the network.

!!! note "Reference"
    VATSIM Code of Conduct B6
    > No flight may declare itself to have priority over another. Pilots are permitted to declare in-flight emergencies only when under air traffic control. If, for any reason, air traffic control requests the pilot to terminate the emergency, then the pilot must do so IMMEDIATELY or disconnect from the network. 

It is up to the discretion of the pilot in command as to whether to declare a Pan Pan or Mayday. However, the majority of situations will warrant a Pan Pan.

### Examples of Emergencies
| Examples of Pan Pans | Examples of Maydays |
| -------------------- | ------------------- |
| Engine failure in a multi-engine aircraft | Uncontained engine fire |
| Depressurisation | Smoke in the cabin |
| Minor flight control problem | Major flight control problem |
| Medical emergency | VFR in IMC |
| Necessary weather avoidance in contradiction of ATC clearance | |

## Urgency Call (Pan Pan)
An urgency call should be made when an aircraft requires urgent assistance but there is not an *immediate* threat to life.

!!! note "Format"
    "Pan Pan, <span class='optional'>[Pan Pan, Pan Pan]</span>, <span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Nature of Emergency</span>, <span class='placeholder'>Intentions</span>, <span class='optional'>[<span class='placeholder'>Position, Level, Heading</span>]</span>, <span class='optional'>[<span class='placeholder'>Any Other Useful Info</span>]</span>"

!!! example
    **JST430**: "Pan Pan, Melbourne Centre, JST430, engine failure, descending to `F210`, 178 POB"  
    **ML CTR**: "JST430, roger Pan"

## Distress Call (Mayday)
A distress call should be made when an aircraft requires urgent assistance and there is an immediate threat to life.

!!! note "Format"
    "Mayday <span class='optional'>[Mayday Mayday]</span>, <span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Nature of Emergency</span>, <span class='placeholder'>Intentions</span>, <span class='optional'>[<span class='placeholder'>Position, Level, Heading</span>]</span>, <span class='optional'>[<span class='placeholder'>Any Other Useful Info</span>]</span>"

!!! example
    **VOZ881**: "Mayday Mayday Mayday, Adelaide Approach, VOZ881, engine fire, require immediate return to Adelaide, 144 POB"  
    **AD APP**: "VOZ881, roger Mayday, turn right heading 360, stop climb at `A040`"

## Fuel Emergencies
See [Fuel Planning](../flight-planning/fuelplanning.md#inflight-fuel-emergencies) for descriptions of each fuel emergency.

### Minimum Fuel
!!! note "Format"
    "<span class='placeholder'>Callsign</span>, minimum fuel"

### Mayday Fuel
!!! note "Format"
    "Mayday Mayday Mayday Fuel"

## ACAS
ACAS (also referred to as TCAS) will alert pilots when they are operating in proximity to another aircraft with a **Traffic Advisory (TA)** and then provide recommended avoidance instructions through a **Resolution Advisory (RA)**.

If an RA is triggered, pilots should notify ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, TCAS RA"

Once clear of conflict, pilots should return to their assigned level and notify ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, clear of conflict, returning to <span class='placeholder'>Assigned Level</span>"

Once re-maintaining their assigned level, pilots shall notify ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, clear of conflict, <span class='placeholder'>Assigned Level</span> resumed"

During an RA, ATS are not responsible for aircraft separation. If an instruction is received during this time which would put the aircraft in further conflict, pilots must inform ATS that they are unable to comply.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, unable to comply, TCAS RA"

## Windshear Escape
If pilots experience windshear, they will generally perform the windshear escape procedure. This normally involves a maximum performance climb straight ahead until clear of the windshear.

If a windshear escape manoeuvre is performed, pilots should notify ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, windshear escape"

Once clear of windshear, pilots should return to their assigned level and notify ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, clear of windshear, returning to <span class='placeholder'>Assigned Level</span>"

If an instruction is received during this a windshear escape procedure which the aircraft is unable to comply with, pilots must inform ATS.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, unable to comply, windshear escape"