---
  title: Enroute 
---

--8<-- "includes/abbreviations.md"

## IFR
### Taxi
For IFR taxi phraseology to ATS, see [Aerodrome](aerodrome.md#taxi).

### Departure
After taking off and setting course for your first tracking point, inform ATC of your departure. If you haven't already received an airways clearance, ensure that you stop your climb below the base of CTA.

The appropriate call depends on whether you expect to be identified or not. If in doubt, assume you are *not* identified.

#### Identified
!!! note "Format"
    "<span class='placeholder'>Callsign</span>, <span class='placeholder'>Position</span>, passing <span class='placeholder'>Current Level</span>, climbing to <span class='placeholder'>Requested Level</span>, estimating <span class='placeholder'>First Waypoint</span> at <span class='placeholder'>ETA</span>"  

!!! example 
    "QLK101D, 3nm southwest of Coffs Harbour, passing `A043`, climbing to `F180`, estimating SORTI at 43"

#### Not Identified
!!! note "Format" 
    "<span class='placeholder'>Callsign</span>, departed <span class='placeholder'>Location</span> <span class='placeholder'>Time of Departure</span>, tracking <span class='placeholder'>Outbound Track</span>, climbing to <span class='placeholder'>Requested Level</span>, estimating <span class='placeholder'>First Waypoint</span> at <span class='placeholder'>ETA</span>" 

!!! example 
    "EWQ, departed YQLP 18, tracking 076, climbing to `F130`, estimating CV at 51"

### Descent 
As you approach top of descent, ATC will provide a clearance to leave CTA (if required) and a traffic statement for your arrival, as well as the current area QNH (if cruising above the transition layer).

!!! example
    **ISA**: "EWQ, when ready leave controlled airspace descending, no reported IFR traffic, area QNH 1021"  
    **EWQ**: "When ready leave controlled airspace descending, area QNH 1021, EWQ"

### Arrival
For SARWATCH cancellation phraseology, see [Aerodrome](aerodrome.md#arrival).

## VFR Flight Following
Flight following provides VFR aircraft operating in Class E and G airspace with a surveillance service. The service is only available within ATS surveillance coverage and subject to ATC workload. Pilots will receive:

- Traffic information on any potentially conflicting aircraft
- Area QNH and meteorological hazard information
- Position/navigational assistance (on request)

### Initiating the Service
To request flight following, establish contact with the ATS unit responsible for the airspace.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, request flight following"

If flight following is not available, the controller will advise *"surveillance not available"*. Otherwise, they will request your position and intentions, and may provide a squawk code to aid in identification.

!!! example
    **VFC**: "Melbourne Centre, Piper Warrior VFC, request flight following"  
    **GUN**: "VFC, squawk 0455, report position and intentions"  
    **VFC**: "Squawk 0455, currently 15nm southeast of YBTH, `A065`, tracking for YTEM, VFC"  
    **GUN**: "VFC, identified, no reported traffic, area QNH 1022"  
    **VFC**: "Area QNH 1022, VFC"

### Notifying ATS Provider of Changes
Whilst receiving a surveillance service, you must notify ATC prior to changing frequencies or making any change to your track/level. See [Enroute Requests](#enroute-requests) for the phraseology to use.

### Cancelling the Service
Flight following may be cancelled by the pilot at any time.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, cancel flight following"

The service may also be terminated by the controller due to workload or lack of surveillance coverage. In either case, you will be advised *"identification service terminated"* when you are no longer being offered a surveillance serve.

!!! example
    **VFC**: "VFC, cancel flight following"  
    **GUN**: "VFC, identification service terminated, squawk 1200, frequency change approved"  
    **VFC**: "Squawk 1200, frequency change approved, VFC"

## Enroute Requests
When established outside of controlled airspace, there is no requirement for authorisation to change your flightpath. However, when receiving an identification service, you must obtain traffic information on any change you will shortly commence, to ensure that doing so doesn't cause conflict with other aircraft.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, request traffic for <span class='placeholder'>intended change</span>"

!!! example
    **FWC**: "FWC, request traffic direct ARMWD"  
    **ARL**: "FWC, no reported IFR traffic"

    **LKU**: "LKU, request traffic for climb to `A060`"  
    **ARL**: "LKU, no reported IFR traffic"