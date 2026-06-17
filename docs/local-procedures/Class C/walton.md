---
  title: Walton (YSWS)
---

--8<-- "includes/abbreviations.md"

## Taxiing
The Walton Apron frequency is not replicated on VATSIM. Aircraft on the cargo apron shall contact SMC for pushback or taxi (unless [pushback requests on ACD](#pushbacktaxi-on-acd) procedures are active).

## Sydney CTA C10
The volume of Class C airspace overhead Camden (known as SY CTA C10) has a lower level that varies according to the time of day. During the hours of 23:00 - 06:00 Sydney local time, the airspace within the C10 area is lowered to `A015`.

<figure markdown>
![Sydney CTA C10 Airspace](../img/sy_cta10.png){ width="400" }
  <figcaption>Sydney CTA C10 Airspace</figcaption>
</figure>

The status of the C10 CTA step will be notified on the YSWS ATIS for the awareness of pilots intending to operate in the area.

## Departures
VFR aircraft should expect to depart via a visual departure, on track to their first tracking point.

### SID Selection
YSWS uses four different SID designators to differentiate between different variations of SIDs that will be issued, according to the time of day, weather, and runway mode in use.

|      | SID Designator | Condition                     |
| ---- | -------------- | ----------------------------- |
| D    | Day            | Between 0530-2300 Local       |
| H    | Hot/Heavy      | Temperature ≥ 35° C, or<br>Heavy aircraft unable to meet level restrictions (on request) |
| N    | Night          | Between 2300-0530 Local, when RRO is **not** in use |
| Q    | RRO            | Between 2300-0530 Local, when RRO is **in use**  |

!!! warning "Important"
    It is vital that pilots select the **correct SID** and comply with all published **speed and altitude restrictions**, as failure to do so may result in a loss of separation with aircraft operating on nearby procedures.

IFR aircraft should expect to be issued with a SID as per below:

=== "05"
	=== "Day"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | BENBU    | **BENBU D** SID |
		| Jet     | CAWLY<br>DIPSO<br>EVONN<br>NOBAR<br>OLSEM<br>OPTIC | **TESAT D** SID, Relevant Transition |
		| Jet     | PKS VOR  | **PKS D** SID   |
		| Jet     | TEEVE    | **TEEVE D** SID |
		| Jet     | LEECE<br>NWA NDB | **TONTO D** SID, Relevant Transition | 
		| Jet     | All others | RADAR SID |
		| Non-Jet | DIPSO<br>KAMBA<br>NOBAR | **KAMBA D** SID, Relevant Transition |
		| Non-Jet | South<br>Southeast<br>Southwest | **ADPAV D** SID |
		| Non-Jet | All others | **ISDIT D** SID |
		
	=== "Hot/Heavy"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | LEECE<br>NWA NDB | **TONTO H** SID, Relevant Transition |
		

	=== "Night"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | BENBU    | **BENBU N** SID |
		| Jet     | CAWLY<br>EVONN<br>OPTIC | **ENDEV N** SID, Relevant Transition |
		| Jet     | DIPSO<br>EVONN<br>NOBAR | **PASGO N** SID, Relevant Transition |
		| Jet     | EXETA<br>LEECE<br>NWA NDB | **REDAS N** SID, Relevant Transition |
		| Jet     | TEEVE    | **TEEVE N** SID |
		| Jet     | PKS VOR  | **TEEVE N** SID, Relevant Transition |
		| Jet     | All others | RADAR SID |
		| Non-Jet | KAMBA    | **KAMBA N** SID |
		| Non-Jet | All others | As per Jets |

=== "23"
	=== "Day"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | BENBU    | **BENBU D** SID |
		| Jet     | CAWLY<br>DIPSO<br>EVONN<br>NOBAR<br>OLSEM<br>OPTIC | **TESAT D** SID, Relevant Transition |
		| Jet     | PKS VOR  | **PKS D** SID   |
		| Jet     | TEEVE    | **TEEVE D** SID |
		| Jet     | LEECE<br>NWA NDB | **TONTO D** SID, Relevant Transition | 
		| Jet     | All others | RADAR SID |
		| Non-Jet | EXETA<br>NWA NDB<br>WOL NDB | **REGER D** SID, Relevant Transition |
		| Non-Jet | North and East | **LEKID D** SID |
		| Non-Jet | All others | RADAR SID |
		
		
	=== "Hot/Heavy"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | LEECE<br>NWA NDB | **MELIT H** SID, Relevant Transition |


	=== "Night"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | BENBU    | **BENBU N** SID |
		| Jet     | CAWLY<br>EVONN<br>OPTIC | **ENDEV N** SID, Relevant Transition |
		| Jet     | DIPSO<br>NOBAR | **PASGO N** SID, Relevant Transition |
		| Jet     | EXETA<br>LEECE<br>NWA NDB | **REDAS N** SID, Relevant Transition |
		| Jet     | TEEVE    | **TEEVE N** SID |
		| Jet     | PKS VOR  | **TEEVE N** SID, Relevant Transition |
		| Jet     | All others | **REDAS N** SID, RADAR Transition |
		| Non-Jet | KAMBA    | **KAMBA N** SID, Relevant Transition |
		| Non-Jet | All others | As per Jets |
		
	=== "RRO"
		| Type    | Via      | SID           |
		| ------- | ------   | ------------- |
		| Jet     | BENBU    | **BENBU Q** SID |
		| Jet     | CAWLY<br>DISPO<br>EVONN<br>NOBAR<br>OLSEM<br>OPTIC | **ENDEV Q** SID, Relevant Transition |
		| Jet     | EXETA<br>LEECE<br>NWA NDB | **TONTO Q** SID, Relevant Transition |
		| Jet     | TEEVE    | **TEEVE Q** SID |
		| Jet     | PKS VOR  | **TEEVE Q** SID, Relevant Transition |
		| Non-Jet | KAMBA    | **KAMBA Q** SID |
		| Non-Jet | All others | As per Jets |


### Pushback/Taxi on ACD
During periods of high traffic, pilots may be required contact ACD for pushback. ACD will assess aerodrome congestion and sequence departing aircraft before transferring them to SMC. Delays should be expected.

When the ATIS includes `ALL DEPARTURES MUST REQUEST PUSH BACK ON 118.65`, all pilots must contact ACD when ready for pushback or taxi (if no pushback is required).

!!! phraseology
    **JST14:** "JST14, bay 21L, request pushback"  
    **WS ACD:** "JST14, standby, estimated delay 10 minutes"  

When instructed, pilots must switch to SMC and **monitor** the frequency. **Do not contact SMC**, they will call you.

!!! phraseology
    **WS ACD**: "JST14, standby for ground, 124.05"  
    **JST14**: "Standby for ground, 124.05, JST14"  

    *Pilot switches to 124.05 and <strong>waits for the controller to contact them</strong>.*

    **WS SMC**: "JST14, Walton Ground, pushback approved"  
    **JST14**: "Pushback approved, JST14"

There may be a delay on the SMC frequency before the controller contacts you. Pilots should only initiate contact with SMC if a significant amount of time has passed since the frequency transfer and no contact has been made by the controller. During busy periods with high frequency congestion, delays may be lengthy.

## Arrivals
ILS, RNP, and RNP(AR) approaches are available to both runways.

IFR aircraft can expect to be processed via a STAR for the most suitable approach.

### STAR Designators
YSWS uses different STAR designators to differentiate between different variations of STARs that will be issued, according to the time of day and runway mode in use.

|      | STAR Designator | Condition                     |
| ---- | --------------- | ----------------------------- |
| A/B  | Day             | Between 0530-2300 Local       |
| N    | Night           | Between 2300-0530 Local, when RRO is **not** in use |
| Q    | RRO             | Between 2300-0530 Local, when RRO is **in use**  |

!!! warning "Important"
    It is vital that pilots select the **correct STAR** and comply with all published **speed and altitude restrictions**, as failure to do so may result in a loss of separation with aircraft operating on nearby procedures.