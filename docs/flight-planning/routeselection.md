---
  title: Route Selection
---

--8<-- "includes/abbreviations.md"

If you intend on remaining outside controlled airspace and away from busy areas & major obstacles, you can generally select the route of your choice. However, if you are planning to enter CTA or visit a major aerodrome, careful route selection will make it considerably easier for ATC to clear you as requested. A number of [third-party tools](#use-of-third-party-tools) exist to help with route selection but each have shortcomings and limitations, so it's helpful to be aware of how to perform this task manually.

## VFR Route Selection
When operating VFR, you are required to determine your position with a visual fix every 30 minutes (see [VFR Navigation](../navigation/vfrnavigation.md#navigation-requirements) for more info), so it is important that you plan your route with enough identifiable landmarks to allow frequent visual fixes. Using a VTC, VNC, or WAC (available on the [Airservices Australia](https://www.airservicesaustralia.com/aip/aip.asp) website), plot your departure and destination airports, then assess any route requirements to remain clear of obstacles, CTA, or PRDs. From there, select a route which will provide easy visual navigation, with frequent landmarks (such as mountain peaks, lakes, river junctions, towns, racetracks, etc) on and either side of your planned track. Also look for lead-in features which will aid in the early recognition of each landmark.

When operating near CTA or PRDs, apply a conservative lateral buffer or plan a level which remains clear of the boundary. If ATC see you tracking towards airspace without a clearance, they're likely to send you a 'contact me' request.

If you plan to enter or transit CTA, especially around major Class C aerodromes, plan a backup route which remains OCTA, in case an airways clearance is unavailable.

## IFR Route Selection
IFR flights are generally planned along pre-defined airways, joining ground-based navaids or RNAV waypoints together along surveyed paths. This provides pilots with terrain/obstacle clearance assurance and helps manage traffic in busy terminal areas by defining a designated inbound and outbound track. Some airways are designated as one-way tracks, while others allow traffic to utilise it in both directions.

Pilots should use an ERC in conjunction with a TAC around major aerodromes to determine the best route. For operations at or below FL200, use the ERC-L (low). Operations above FL200 should use the ERC-H (high). Some remote aerodromes aren't serviced by airways, so it may be desirable to plan direct to an appropriate fix instead.

When planning a route, consider any airspace requirements (particularly when operating to, from, or in the vicinity of major aerodromes) and ensure you comply with the [ERSA Flight Planning Requirements](#ersa-flight-planning-requirements) as detailed below. Also consider the terrain you'll be flying over. During the winter months, icing can become a serious threat to aircraft without ice protection equipment and an alternate route may need to be planned to avoid areas of high terrain, allowing the aircraft to operate in the warmer air at lower altitudes. Each degree of latitude/longitude on an ERC-L is divided into a grid, and a Grid LSALT is published for each square denoting the lowest safe altitude for operations in that area. Pilots can use these Grid LSALTs to ensure they'll remain above any limiting obstacles/terrain, even if they need to deviate off their planned route.

### ERSA Flight Planning Requirements
The ERSA Flight Planning Requirements (FPR) document lists required tracking points and vertical restrictions which help manage traffic flow into and out of busy aerodromes. Ensure that your planned route complies with any restrictions imposed by the FPR. If your planned departure and destination aerodrome (or initial tracking points) are not listed in the document, you can assume that no planning requirements apply. In this case, plan a route in accordance with the advice above to respect any one-way airways or other planning requirements.

!!! tip
    If the required route listed in the FPR is undesirable (e.g. it adds significant track miles) and the weather is suitable, consider departing VFR or remaining OCTA until you are outside the terminal area.

## Altitude Selection
Appropriate level selection depends on your flight rules, route, and intention to enter or remain clear of CTA.

For IFR, determine the highest LSALT out of the airways you've selected or the Grid LSALT, if not flying via airways for your entire route. For VFR, identify the highest obstacles/terrain and select a level which provides a safe buffer (generally 500ft, or 1000ft if above a populated area) above. 

<figure markdown>
![Grid LSALTs (circled) over Flinders Island for each green grid square](img/gridlsalts.png){ width="700" }
  <figcaption>Grid LSALTs (circled) over Flinders Island for each green grid square</figcaption>
</figure>

Next, adjust your chosen level to comply with the hemispherical level rule. IFR flights should plan an odd level (e.g. 7,000ft) when flying east and an even level (e.g. 8,000ft) when flying west, up to 41,000ft. VFR flights should comply with this rule, but add 500ft to the determined level. A full list of available altitudes is replicated below:

| IFR - Track 000 to 179 | IFR - Track 180 to 359 |
| ----- | ----- |
| 3,000ft | 2,000ft |
| 5,000ft | 4,000ft |
| 7,000ft | 6,000ft |
| 9,000ft | 8,000ft |
| FL110 | 10,000ft |
| FL130 | FL120 |
| FL150 | FL140 |
| FL170 | FL160 |
| FL190 | FL180 |
| FL210 | FL200 |
| FL230 | FL220 |
| FL250 | FL240 |
| FL270 | FL260 |
| FL290 | FL280 |
| FL310 | FL300 |
| FL330 | FL320 |
| FL350 | FL340 |
| FL370 | FL360 |
| FL390 | FL380 |
| FL410 | FL400 |
| FL450 | FL430 |
| FL490 | FL470 |
|  | FL510 |

| VFR - Track 000 to 179 | VFR - Track 180 to 359 |
| ----- | ----- |
| 3,500ft | 2,500ft |
| 5,500ft | 4,500ft |
| 7,500ft | 6,500ft |
| 9,500ft | 8,500ft |
| FL115 | 10,500ft |
| FL135 | FL125 |
| FL155 | FL145 |
| FL175 | FL165 |
| FL195 | FL185 |
| FL215 | FL205 |
| FL235 | FL225 |
|  | FL245 |

!!! note
    When planning to operate VFR outside CTA at 3,000ft AMSL or below, you may select any desired altitude without regard for the table above.

!!! tip
    These rules apply to pilots at the flight planning stage. Once airborne, you may request climb to non-standard levels, subject to surrounding traffic and ATC requirements.

## Use of Third-Party Tools
Flight planning can be greatly simplified through the use of the many available third-party tools, although caution should be taken when utilising them.

[SimBrief](https://simbrief.com){target=new} is a popular site designed to automate route selection and fuel planning. Pay extra attention when selecting a route from the suggested list, as they may have been submitted by users with little flight planning experience. It is good practice to confidence check the suggested route against another source, and where available, select the purple 'Preferred Route' (which have been uploaded by VATPAC staff). It is also recommended that you add extra fuel (using the built-in input boxes) where required, as per [Fuel Planning](./fuelplanning.md).

VATPAC's [Pilot Assist](https://vatpac.org/membership-hub/tools/pilot){target=new} tool can be helpful for generating weather forecasts and accessing charts for your planned flight. The system can also be used to generate a route which complies with the ERSA FPR.

Some aerodromes and terminal areas feature specific procedures for pilots to comply with. These procedures have been summarised in [Local Procedures](../../local-procedures/), where you'll find flight planning advice as well as in-flight procedural guidelines.

Applications like Navigraph allow pilots to plot out their intended flight plan on appropriate maps and charts. For those without a subscription, the free [SkyVector](https://skyvector.com){target=new} provides similar functionality. Be aware that the system is primarily designed for use in the USA and whilst Australian coverage is generally good, the VFR mapping system is lacking compared to other options.