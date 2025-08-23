---
  title: Controlled Airspace
---

--8<-- "includes/abbreviations.md"

## Airways Clearances
An airways clearance must be obtained **before** entering CTA by contacting the relevant ATS unit responsible for the airspace. This may take the form of an airways clearance on the ground at a [controlled aerodrome](../radio-telephony/Controlled%20Airspace/aerodrome.md#airways-clearance), or airborne if transiting from uncontrolled airspace to CTA.

Australia regards the following classes of airspace as **controlled airspace**:

- Class A
- Class C
- Class D
- Class E (for IFR aircraft, see [Class E Airspace](#class-e-airspace) for more details)

### Class E Airspace
In Class E Airspace, IFR aircraft require an airways clearance prior to entry.

VFR aircraft, however, do not require a clearance. Instead, VFR aircraft must maintain a listening watch to the relevant ATS frequency and respond to any radio calls which are directed to them.

### Coded Clearances
Generally, an airways clearance will specify a clearance limit, the approved route to fly, and any vertical restrictions, as well as other details (such as a squawk code and departure procedure) as required. A *coded clearance* is a published procedure which includes these details by default, removing the need for ATS to specify them over the radio. 

Coded clearances are generally defined in/out of, and surrounding, busy controlled aerodromes, or in congested controlled airspace. Details can be found in local ERSA FAC entries and [Local Procedures](../local-procedures/).

!!! example
    **Regular Clearance**: *"CYF, cleared to YSBK via HBB, SYHD, MANLY, LRF, maintain A015"*  
    **Coded Clearance**: *"CYF, cleared Harbour Scenic One"*

## Controlled Aerodromes
At a controlled aerodrome, pilots require clearance or approval to pushback, taxi, takeoff, and land from any area inside the **manoeuvring area**. CASA publish manoeuvring area maps on their [website](https://www.casa.gov.au/search-centre/aerodrome-manoeuvring-maps), showing the extent of each controller's jurisdiction. Pilots must contact the most appropriate ATS unit to obtain clearance to operate inside the manoeuvring area.

!!! tip
    VATSIM employs the [Top Down Rule](./vatsimoperations.md#top-down-rule) to provide pilots with the best possible service when few controllers are online. Ensure you contact the correct controller for any aerodrome services when the aerodrome controllers themselves are not online.

### Frequency Transfers
#### SMC/ADC
In Australia, only international aircraft will be explicitly transferred from SMC to ADC (and vice versa). Domestic aircraft should switch to the ADC frequency without direction from SMC when approaching the instructed holding point and when ready for departure.

!!! example
    *AM210 is taxiing at YSSY for YBTH. They will <strong>not</strong> be explicitely transferred to ADC.*  
    **SY SMC**: "AM210, cross runway 25, taxi to holding point B10, runway 34L"  
    **AM210**: "Cross runway 25, taxi to holding point B10, runway 34L, AM210"  
    *As they approach the holding point, the pilot switches to the ADC frequency.*  
    **AM210**: "Sydney Tower, AM210, ready"
    
    *UAL870 is taxiing at YSSY for KLAX. They <strong>will</strong> be explicitely transferred to ADC.*  
    **SY SMC**: "UAL870, cross runway 25, taxi to holding point A6, runway 34L"  
    **UAL870**: "Cross runway 25, taxi to holding point A6, runway 34L, UAL870"  
    **SY SMC**: "UAL870, report ready to tower, 120.5"  
    **UAL870**: "120.5, UAL870"

#### Departures Controller
An explicit frequency transfer from ADC to Departures will be given for all aircraft. This may be included with the takeoff clearance or issued after the aircraft has become airborne. Do not switch to the Departures frequency until this instruction has been issued. Pilots in receipt of an airways clearance which included a 'Departure Frequency' should switch to that frequency when they are instructed to *'contact departures'*.

### Airport Efficiency Procedures
Major aerodromes have published airport efficiency procedures which provide guidance to pilots to minimise runway occupancy and improve overall traffic capacity. Importantly, these procedures specify the preferred runway exit which pilots should plan to vacate at when landing. Pilots should plan to vacate at these exits by default, and if an alternate exit is preferred, should inform ADC on first contact.

!!! example
    Any aircraft landing on **runway 34L** at YSSY with the intention of parking at the **domestic terminal** should plan to vacate at **taxiway B9**.

Airport efficiency procedures are published in dedicated DAP charts of the same title.

### Class C
Major controlled aerodromes are surrounded by Class C airspace. An airways clearance is required for all operations into, out of, and in the vicinity of a Class C aerodrome.

### Class D
Busy regional aerodromes, or smaller capital city aerodromes, are designated Class D aerodromes. An airways clearance is required for all operations in Class D airspace, however a takeoff clearance constitutes a clearance to operate within, or to leave, the Class D CTR (the airspace in contact with the ground). This means that pilots wishing to conduct circuits inside the CTR, or who wish to depart from the CTR directly into Class G airspace, will not receive an explicit airways clearance.

!!! phraseology
    *VH-LKU is a VFR P28A intending to depart from YSBK into Class G airspace on track to the training area.*  
    **LKU**: "Bankstown Tower, Warrior LKU, holding point A8, runway 29R, upwind departure, ready"  
    **BK ADC**: "LKU, runway 29R, cleared for takeoff"

    *FD213 is an IFR B350 intending to depart from YSBK into the overlying Class C airspace.*  
    **FD213**: "Bankstown Ground, FD213, to YBTH, request clearance"  
    **BK SMC**: "FD213, cleared to YBTH via KADOM, flight planned route, BK9 departure, climb via SID to A030, squawk 3236"  
    **FD213**: "Cleared to YBTH via KADOM, flight planned route, BK9 departure, climb via SID to A030, squawk 3236, FD213"

Class D aerodromes include a portion of Class D airspace managed by ADC. Aircraft intending to enter the airspace from Class G must report their position and intentions to ADC prior to entering CTA. In Class D airspace, two-way communications established between ATS and the pilot constitutes a clearance to enter CTA in the manner described.

!!! example
    *AI9 is a VFR DA42, reporting inbound to YCFS from the south. The response by ADC establishes two-way communications, so AI9 may enter CTA direct to YCFS at A025.*  
    **AI9**: "Coffs Tower, Diamond AI9, NHS, A025, inbound, received C"  
    **CFS ADC**: "AI9, Coffs Tower"
    
    *YPH is a VFR DA40, reporting inbound to YCFS from the north. ADC has instructed them to standby, so they must **not** enter CTA, as this does not establish complete two-way communications.*  
    **YPH**: "Coffs Tower, Diamond YPH, WGG, A015, inbound, received C"  
    **CFS ADC**: "YPH, Coffs Tower, standby"

#### Metro D
Metro D aerodromes are small Class D aerodromes situated in busy terminal areas. They generally feature a small CTR with a limited lateral and vertical definition, and no overlying Class D CTA. Instead, they often sit directly below or adjacent to Class C CTA.

The [Class D](#class-d) rules described above apply to Metro D aerodromes. In addition, there are often local procedures which dictate implied frequency transfers to circuit join instructions, specified in the local ERSA FAC entry and [Local Procedures](../local-procedures/). Pilots must ensure they are familiar with all local procedures prior to operating at these aerodromes.

## Pilot Tracking/Level Requests
Whilst inside CTA, pilots must comply with the latest route clearance which they have received and maintain any assigned level. If alternate tracking or a different level is desired, this must first be requested and approved by ATS.

Changes of level are common due to enroute weather, prevailing winds, or traffic, and should be requested as per [Change of Level](../radio-telephony/Controlled%20Airspace/enroute.md#change-of-level).

Tracking to waypoints further along a pilot's planned route (track shortening) or to positions not on a pilot's flight plan should be requested as per [Amended Route](../radio-telephony/Controlled%20Airspace/enroute.md#amended-route).

Where [bad weather](../meteorology/hazards.md) presents a hazard to an aircraft, deviations around it should be requested as per [Route Deviation](../radio-telephony/Controlled%20Airspace/enroute.md#route-deviation).

If a pilot wishes to conduct airwork inside CTA, this must be first requested and approved, as per [Airwork](../radio-telephony/airwork.md).

## ATC Instructions
Pilots must comply with any ATS-issued instructions in a timely manner. If a delay is experienced (due to aircraft malfunction or pilot competence), inform ATS so that an alternate instruction may be issued.

!!! important
    VATSIM is a learning environment for both controllers and pilots, and it is expected that pilots will need a helping hand from time to time.

    If you do not understand an instruction or you are having trouble complying with it, **don't stay quiet, speak up!** Controllers can always explain themselves more clearly or provide an alternate instruction. Failure to inform the controller may result in frustration later on in the flight when their systems detect that you are off course, at the wrong level, or operating in contravention of the issued instruction.

### Sequencing
A variety of sequencing techniques are used by controllers to ensure a smooth, efficient, predictable flow of traffic. You must comply with any sequencing or delaying instructions issued.

#### Speed Control
Generally speaking, an ATS request to *'report speed'* refers to your current indicated airspeed. If a controller wishes to learn your TAS or Mach number, they will ask for these details explicitely.

If you are instructed to reduce to **minimum speed** or increase to **maximum speed** (or any other variation of these speeds), you should acknowledge the instruction and comply immediately. There is no need to inform the controller of the actual achieved speed.

!!! phraseology
    **GUN**: "ANZ19, reduce to minimum speed"  
    **ANZ19**: "Reduce to minimum speeed, ANZ19"

!!! note
    *'Minimum/maximum speed'* is not a fixed speed. Pilots are expected to fly as fast or slow as possible, considering aircraft configuration, environmental factors, operational requirements/considerations, and other factors. As an aircraft climbs or descends, pilots are expected to adjust their speed to continue complying with the instruction.

    E.g. an aircraft instructed to *"maintain maximum speed to the field"* is expected to fly as fast as the pilot is comfortable and to reduce speed as needed to configure for landing, while maintaining the best forward speed throughout.

Controllers may issue speed control for a particular phase of flight.

!!! example
    *"Speed on climb 250kt or less"*

Some instructions may also include self-cancelling conditions.

!!! example
    *"Speed 300kt or greater until TAMMI"*
    
Where a controller wishes to adjust your profile descent speed, they may do so by issuing an indicated airspeed to maintain on transition from the Mach range to the IAS range. This speed should be maintained in lieu of your planned descent IAS until reaching a published speed limitation.

!!! example
    *"Reduce to Mach decimal 78, transition into 250kt"*

#### Vectors
Where speed control is insufficient or impractical, ATS will provide vectors to increase an aircraft's track miles and absorb any remaining delay. All heading instructions must be complied with in a timely manner and pilots must not alter their heading unless authorised by ATS.

#### Holding
If delays are excessive, ATS may issue holding instructions. When holding at a published hold (where details are available on an ERC/TAC or approach chart), the inbound course, turn direction, and timing/DME limit specified should be used. When holding at an unpublished hold (where no details are published for that waypoint), ATS will specify these details.

There are a variety of procedures specific to holds, which are covered on the [Holding](../navigation/holding.md) page.

In the real world, it is common practice for pilots to be issued an onwards clearance which includes a nominated hold exit time. Pilots are responsible for ensuring they adjust their speed and the length of the pattern (with ATS approval) to pass over the holding fix at the specified time. This practice is rare online but sometimes offered to experienced pilots. Pilots in receipt of a hold exit time must cross the holding fix at up to **0 seconds late** and **60 seconds early**.

Some airliner avionics will allow pilots to adjust the required time of departure from the fix, with the aircraft autothrottle adjusting the speed to meet the time. For aircraft not equipped with suitable automation, a simple calculation can determine the length of each outbound leg to meet the required time. Based on the current aircraft speed, determine the number of minutes to lose, then determine how long a single hold may take based on an arbitrary outbound length. Try different leg length values until the total delay becomes a multiple of the time taken for one holding pattern.

!!! example
    An aircraft has been issued with an onwards clearance which results in a total delay of **12 min**. The pilot may complete **two holding patterns** with an outbound **leg time of 2 min** and rate 1 turns, resulting in a total of 6 min per hold.

Note that this calculation assumes that each turn will be conducted at rate 1 (and therefore take 1 min to complete a 180° turn). If this is not the case, the calculation should be adjusted to compensate.

#### Predictable Sequencing Waypoints
Predictable sequencing waypoints allow ATS to increase an aircraft's track miles to achieve a necessary delay, whilst providing pilots with a known distance to run (unlike during vectors where the track miles remaining are generally unknown). This helps pilots plan more predictable, profile-driven descents.

<figure markdown>
![Caption](./img/predictablesequencingwaypoints.png){ width="600" }
    <figcaption>Predictable Sequencing Waypoints on the **Q29** Airway<br><small>E.g. Tracking ANLID to DOVEX to BULLA adds 2 min</small></figcaption>
</figure>

!!! tip
    Details of each set of waypoints are contained in [Local Procedures](../../local-procedures/).

In response to an instruction to track via a new sequencing waypoint, pilots must promptly enter the waypoint into their flight management system and track in accordance with the ATS instruction.

!!! warning "Important"
    Some instructions will require pilots to track **from their present position** while others will require tracking **from a nominated waypoint**. Ensure you operate in accordance with the provided instruction and query the controller if you need clarification.

#### Waypoint Crossing Times
In the real world, delays which don't necessitate holding will generally be absorbed by issuing a waypoint crossing time to a pilot. The pilot will then adjust their own speed to cross the waypoint at the given time. This practice is rare online but is gaining popularity as more pilots become familiar with the procedure. Pilots in receipt of a waypoint crossing time must cross the fix at up to **0 seconds late** and **30 seconds early**.

Complying with a crossing time is simple. Most airliners have the ability to provide a Required Time of Arrival, either through a dedicated **RTA** page or by editing the waypoint details on the flight plan page. 

Pilots of aircraft without these systems should adjust their speed (generally involving a speed reduction) until their FMS/GPS indicates the required ETA for the relevant waypoint. If the aircraft reaches minimum speed but is still too early for the assigned time, the pilot must inform ATS so that alternate delaying action can be provided.

!!! example
    An aircraft has been issued an instruction to cross **WELSH** at time **43**. The FMS indicates that the aircraft will currently reach WELSH at time 38. To comply with the time, the pilot should reduce speed (to not below minimum speed) until the FMS ETA for WELSH changes to 43.

    Given that the accepted window for the crossing time is 0 seconds late and up to 30 seconds early, the pilot should then increase speed slightly so that the FMS indicates an ETA of 42. This way, they can be sure that they are in the 30 seconds prior to time 43.

## Separation Standards
Different classes of airspace have different operating requirements from pilots and services provided by ATS. This is explained in detail on the [Airspace Overview](./index.md) page.

As a summary, pilots can expect the following separation standards to be applied to them in CTA.

| Airspace Class | IFR | VFR | SVFR |
| --- | --- | --- | --- |
| **A** | Separated from all aircraft | - | - |
| **C** | Separated from all aircraft | Separated from IFR, traffic info on other aircraft | Separated from SVFR (where visibility is less than VMC), traffic info on other aircraft |
| **D** | Separated from IFR and SVFR, traffic info on VFR | Traffic info on all aircraft | Separated from SVFR (where visibility is less than VMC), traffic info on other aircraft |
| **E** | Separated from IFR, traffic info on other aircraft | Traffic info on all aircraft | - |
| **G** | Traffic info on all aircraft | Traffic info on all aircraft (only if receiving SIS) | - |

### Visual Separation
In some situations, a separation standard must be maintained between two aircraft, but doing so would result in a delay for one or more pilots. In these situations, ATS may delegate separation responsibility to the pilot, using visual separation.

Visual separation responsibility will only be issued to a pilot when both aircraft are operating at or below `A100` and the pilot reports:
- that they have the other aircraft in sight, and
- that they can maintain visual separation with the aircraft

The delegation of separation responsibility does **not** authorise a pilot to manoeuvre in contradiction of their authorised clearance. If alternate tracking is required, pilots must still request this and await ATS approval.

!!! phraseology
    *RSCU203 is a VFR helicopter who wishes to depart from Royal Prince Alfred Hospital, which sits directly under the YSSY RWY 16L approach path.*  
    **SY ADC:** "RSCU203, report sighting a Jetstar A320 on a 6nm final RWY 16L"  
    **RSCU203:** "Traffic sighted, RSCU203"  
    **SY ADC:** "RSCU203, are you able to maintain own separation with the Jetstar A320?"  
    **RSCU203:** "Affirm, RSCU203"  
    **SY ADC:** "RSCU203, maintain own separation with the Jetstar A320, caution wake turbulence, report airborne"  
    **RSCU203:** "Maintain own separation with the Jetstar A320, wilco, RSCU203"