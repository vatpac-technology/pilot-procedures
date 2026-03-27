---
  title: Aerodrome 
---

--8<-- "includes/abbreviations.md"

## Radio Setup
Avionics and radio hardware setup is generally pilot preference. Aircraft with a requirement to maintain two-way communications with ATC (e.g. IFR aircraft operating OCTA) will need to manage both the relevant ATC frequency and local CTAF.

A common radio setup is:

| COM 1 | COM 2 |
| --- | --- |
| ATC/Area Frequency | CTAF |

### Single Radio Aircraft
Aircraft equipped with a single radio engaged in IFR operations must continue to comply with the two-way communication requirement (outlined above). When operating OCTA in the vicinity of an aerodrome, these aircraft will need to switch between the relevant ATC frequency and the local CTAF.

Pilots **must report** when leaving an ATC frequency in this manner, including listing the CTAF they are switching to.

!!! phraseology
    **RXA6518**: "RXA6518, switching to Parkes CTAF 126.7"  
    **GUN**: "RXA6518, identification terminated"

!!! warning "Important"
    You **must not** leave an ATC frequency whilst inside controlled airspace. For aircraft equipped with a single radio, pilots must wait until they leave CTA and then notify ATC that they are switching frequencies. 

## ATC Frequency
### Taxi
Immediately prior to, or during, taxi at a Class G aerodrome, IFR aircraft must make a taxi report to the enroute or terminal controller managing the overlying airspace.

!!! note "Format"
    "<span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Aircraft Type</span>, <span class='optional'>[<span class='placeholder'>Persons on Board</span> POB]</span>, IFR, taxiing <span class='placeholder'>Location</span> for <span class='placeholder'>Destination</span>, runway <span class='placeholder'>Departure Runway</span>"

    *POB is not required for scheduled air transport flights.*

!!! example
    "Melbourne Centre, RXA6588, SAAB 340, IFR, taxiing YORG for YPKS, runway 29"

    "Sydney Approach, FWC, Cessna 172, 3 POB, IFR, taxiing YWBN for YYNG, runway 35"

In response, ATC will likely issue a squawk code and traffic statement of any relevant nearby aircraft.

#### Low Overlying CTA
Some aerodromes, particularly those in the capital city terminal areas or procedural towers where the tower is closed, have low overlying CTA steps which may be difficult to avoid on departure. In these situations, ATC will issue an airways clearance for aircraft planned into CTA prior to departure.

!!! example
    **QLK101D**: "Brisbane Centre, QLK101D, Dash 8, IFR, taxiing YCFS for YSSY, runway 21"  
    **INL**: "QLK101D, squawk 1202, no reported IFR traffic, report lined up for airways clearance"  
    **QLK101D**: "Squawk 1202, wilco, QLK101D"  

    **QLK101D**: "QLK101D, lined up"  
    **INL**: "QLK101D, cleared to YSSY via SORTI, flight planned route, climb to `F120`"  
    **QLK101D**: "Cleared to YSSY via SORTI, flight planned route, climb to `F120`, QLK101D"

#### Poor Radio Reception
Where poor radio reception precludes establishing contact with ATC on the ground, report airborne to commence your SARWATCH service.

!!! note "Format"
    "<span class='placeholder'>ATC Unit</span>, <span class='placeholder'>Callsign</span>, airborne <span class='placeholder'>Location</span>"

After establishing contact, [report your departure](enroute.md#departure).

!!! example
    **IBU**: "Melbourne Centre, IBU, airborne YMRY"  
    **WOL**: "IBU, squawk 3277, no reported IFR traffic"  
    **IBU**: "Squawk 3277, departed YMRY 44, tracking 340, climbing to `A080`, estimating ATGOD at 12, IBU"  
    **WOL**: "IBU, no reported IFR traffic for climb to `A080`, area QNH 1009"  
    **IBU**: "Area QNH 1009, IBU"

### Arrival
After landing at their destination, or where insufficient radio coverage exists on the ground, at a suitable time during their arrival, IFR aircraft must report their arrival to ATC and cancel their SARWATCH.

!!! note "Format"
    "<span class='placeholder'>Callsign</span>, <span class='placeholder'>Location</span>, cancel SARWATCH"

!!! example
    **EWQ**: "EWQ, Charleville, cancel SARWATCH"  
    **ISA**: "EWQ, Charleville SARWATCH terminated"

SARWATCH termination is not required to be read back by the pilot. Once your SARWATCH has been terminated, your flight has finished in the eyes of ATC. No further services will be provided to you.

## CTAF Frequency
When operating within, or approaching, the vicinity of a non-controlled aerodrome, you should tune the appropriate CTAF and make broadcast radio calls as deemed appropriate.

!!! note "Format"
    "<span class='placeholder'>Location</span> traffic, <span class='placeholder'>Callsign</span>, <span class='placeholder'>Message</span>, <span class='placeholder'>Location</span>"

You are only required to make a radio broadcast on a CTAF where you consider it necessary to avoid a collision with another aircraft. However, common sense would suggest that regular, structured broadcasts are the best way to mitigate potential conflict and aid other pilots in their situational awareness.

Pilots should reply to any received broadcast with their own position and intentions (and any other relevant information) where they deem potential for conflict.

!!! note
    The *vicinity* of an aerodrome is a broad term with no strict definition. As a general rule, pilots should broadcast on the frequency when within roughly **5 to 8 minutes laterally** and when intending to operate in the airspace from the **surface to roughly 5,000ft above ground level**. In practice, this translates to a 10 nautical mile radius for small, piston aircraft like Cessna 172s and Piper Cherokees, and up to a 30 nautical mile radius for high performance aircraft like turboprops and jets.

    Good airmanship would dictate monitoring the CTAF even when outside this volume of airspace where it is known that high-performance aircraft are operating in the vicinity.

### Finding the Correct Frequency
The CTAF for each aerodrome can be found by referencing its appropriate ERSA entry or reviewing its aerodrome chart. These resources are available on the Airservices website for free or through providers like Navigraph, Chartfox and the [VATPAC Tools](https://vatpac.org/tools){target=new} page.

Additionally, the [VATSIM AIP](https://my.vatsim.net/pilots/aip){target=new} includes all VATPAC aerodromes, with information including the correct frequency to use. This is particularly important for locations like Sydney, Melbourne, and the other Class C airports which operate 24 hours a day in the real world. VATPAC have defined an appropriate CTAF for these locations which should be used by pilots when there is no ATC coverage online.

!!! tip
    Pilots can type **.ctaf** into any VATSIM pilot client to display the appropriate frequency to use at any aerodrome.

### Recommended Calls
#### Departures
Pilots departing an aerodrome are encouraged to make a CTAF broadcast when they are:

- Taxiing for departure

!!! example
    "Dubbo traffic, Cessna 182 CSA, taxiing to runway 05, Dubbo"

- Entering the runway

!!! example
    "Dubbo traffic, Cessna 182 CSA, entering and backtracking runway 05, Dubbo"

- Commencing the takeoff roll

!!! example
    "Dubbo traffic, Cessna 182 CSA, rolling runway 05 for a downwind departure to the southwest, climbing to `A065`, Dubbo"

- Departing the circuit

!!! example
    "Dubbo traffic, Cessna 182 CSA, departed downwind runway 05, passing `A023`, climbing to `A065`, tracking 214 to Griffith, Dubbo"


#### Arrivals
Pilots arriving to aerodrome are encouraged to make a CTAF broadcast when they are:

- About to enter the vicinity of the aerodrome

!!! example
    "Cowra traffic, Cub ELN, 11 miles south southeast, `A045`, inbound, estimating the circuit area at 36, Cowra"


- Joining the circuit

!!! example
    "Cowra traffic, Cub ELN, joining downwind runway 15, Cowra"


- Clear of the runway

!!! example
    "Cowra traffic, Cub ELN, clear of all runways, Cowra"

#### Overflyers
Pilots overflying an aerodrome are encouraged to make a CTAF broadcast when they are:

- About to enter the vicinity of the aerodrome

!!! example
    "Wagga traffic, Helicopter SUA, 8 miles west, `A035`, overflying to the east, estimating overhead at 40, Wagga"


- Overhead

!!! example
    "Wagga traffic, Helicopter SUA, overhead, `A035`, tracking to the east, Wagga"

#### Circuits
Pilots conducting circuits at an aerodrome are encouraged to make CTAF broadcasts as appropriate to mitigate conflict with other aircraft. At a minimum, broadcasting on the base leg with your intentions is generally acceptable.

!!! example
    "Winton traffic, Cherokee KLR, base, runway 14, touch and go, Winton"