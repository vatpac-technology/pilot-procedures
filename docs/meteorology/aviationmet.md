---
  title: Aviation Meteorology
---

--8<-- "includes/abbreviations.md"

## Cloud
Clouds (and their associated lack of inflight visibility) pose a major threat to VFR flight and can impact the operational capability of IFR aircraft. They also bring secondary risks including icing, turbulence, and thunderstorm activity.

### Cloud Cover
Cloud cover is described by *oktas*, or how many eighths of the visible sky is obscured.

| Description | Meaning |
| ---- | ---- |
| Sky Clear (SKC) | **0**/8 of the sky obscured |
| Few (FEW) | **1-2**/8 of the sky obscured |
| Scattered (SCT) | **3-4**/8 of the sky obscured |
| Broken (BKN) | **5-7**/8 of the sky obscured |
| Overcast (OVC) | **8**/8 of the sky obscured |

!!! tip
    [VFR navigation](../navigation/vfrnavigation.md) is considered impractical with more than 4 oktas of cloud coverage.

Area forecasts may describe the frequency of cumulonimbus clouds using the following scale:

| Description | Meaning |
| ---- | ---- |
| Isolated (ISOL) | Individual clouds |
| Occasional (OCNL) | Well-separated clouds |
| Frequent (FRQ) | Clouds with little (or no) separation |

### Types
Generally, rain-producing clouds are prefixed or suffixed with *nimbo* (e.g. nimbostratus and cumulonimbus). *Cumulo* clouds are generally heaped, vertical arrangements which are frequently associated with turbulence (e.g. cumulus and stratocumulus). Layered clouds are generally prefixed or suffixed with *strato* (e.g. altostratus and cirrostratus) and form large sheets of cloud with little vertical development.

For ease of use on weather reports and forecasts, each cloud type is abbreviated to a two character term.

| Abbreviation | Cloud Type | Height | Description |
| --- | --- | --- | --- |
| Ci | Cirrus | High | Detatched, delicate filaments |
| Cc | Cirrocumulus | High | Thin layer made up of many small ripples or grains |
| Cs | Cirrostratus | High | Transparent veil covering most of the sky, creates a sun halo |
| Ac | Altocumulus | Mid | Layer of rounded masses made up of smaller particles |
| As | Altostratus | Mid | Grey layer covering most of the sky, no halo |
| Ns | Nimbostratus | Mid | Thick, grey, uniform layer with continuous preciptation |
| Sc | Stratocumulus | Low | Layer of large rolls or masses |
| St | Stratus | Low | Grey, fairly uniform layer with drizzle |
| Cu | Cumulus | Low | Groups of detatched, towering, dense clouds |
| Cb | Cumulonimbus | All | Heavy, dense, towering thunderstorm cells |

### Vertical Visibility
Where weather phenomena (generally smoke) obscures the sky but does not form cloud, the vertical visibility will be reported. This can be treated as an overcast layer of cloud at that level.

!!! example
    A SPECI which contains `VV009` would indicate vertical visibility of 900ft AAL, likely caused by a layer of smoke at that level.

## Visibility
Along with cloud, low visibility also poses a major threat to all forms of aviation. Low visibility is generally caused by precipitation, fog/mist, or other airborne particles such as bushfire smoke or dust storms.

**Fog** is cloud which touches the surface and reduces visibility below 1,000m. **Mist** is fog which reduces visibility to not less than 1,000m.

Both fog and mist (and low cloud in general) are likely to form when the [temperature and dew point](#temperature) are close together, increasing the relative humidity. Pilots can generally extrapolate the likelihood of fog by comparing the temperature and dew point split on a [METAR](./forecastsandreports.md#metar).

## Wind
Wind is described by the direction **from** which it blows.

!!! example
    Wind reported as `210/15` blows from the southwest to the northeast at 15kt. Aircraft travelling southwest would have a headwind while aircraft travelling northeast would have a tailwind.

### Surface Winds
Surface winds play a major role in determining the duty runway at an aerodrome, as aircraft generally aim to takeoff and land into wind. Failing to do so can expose the aircraft to large crosswind components (which may make keeping fixed wing aircraft travelling straight difficult) or tailwind components (which increases the GS of an aircraft for a given TAS and requires more runway length to operate from). Additionally, due to the aerodynamic effect of recirculating turbulent air through the rotor system, some helicopters have a maximum tailwind/crosswind speed in which they can hover.

Wind information can be sourced from published reports, [ATIS/AWIS](#weather-information) stations, or by looking at the windsock. When operating at landing areas without reported weather information, environmental elements such as trees, blowing smoke, and bodies of water can indicate the wind direction.

### Enroute Winds
Enroute winds impact [navigation](../navigation/vfrnavigation.md), requiring the aircraft's heading to be adjusted to compensate for any crosswind component (and maintain the track made good along the ground). Additionally, headwind or tailwind components will impact the time taken to fly a particular leg, requiring an adjustment in [trip fuel](../flight-planning/fuelplanning.md#flighttrip-fuel).

## Air Pressure
Air pressure has a moderate impact on aircraft performance. At lower pressure (generally found at higher altitudes), air density is reduced, which leads to a reduction in power from aircraft engines and a reduction in thrust from propellers/rotor blades.

### Pressure Altitude
Pilots can calculate the effect of operating at low pressures by applying a correction to their current elevation. This represents the altitude in the [standard atmosphere](#international-standard-atmosphere) where an air mass of that pressure would be found (uncorrected for temperature) and is called the Pressure Altitude. 

A variety of resources exist online to perform this calculation.

## Temperature
Temperature has a major impact on aircraft performance. At higher temperatures, air density is reduced, which leads to a reduction in power from aircraft engines and a reduction in thrust from propellers/rotor blades.

Air temperature can be measured a number of ways, however for aviation, it is commonly described as OAT.

### Density Altitude
Pilots can calculate the effect of operating at high temperatures by applying a correction to their calculated [pressure altitude](#pressure-altitude). This represents the altitude in the [standard atmosphere](#international-standard-atmosphere) where air of that density would be found and is called the Density Altitude. 

A variety of resources exist online to perform this calculation.

## International Standard Atmosphere
A set of standard atmospheric conditions have been established to create a baseline for all performance-driven data in aviation. It is often necessary to correct from the standard atmosphere to determine the effect the current atmospheric conditions will have on aircraft performance.

The standard MSL atmospheric conditions are:

| Element | Value |
| --- | --- |
| Temperature | 15 deg C |
| Temperature Lapse Rate | 2 deg C per 1,000ft of altitude *(until the tropopause at 36,000ft)* |
| Air Pressure | 1013 hPa |

In addition to calculating actual aircraft performance (based on relevant aircraft performance charts), the values above can be used to estimate the temperature at a particular altitude which may assist in the assessment of enroute [icing conditions](./hazards.md#icing).

## Weather Information
At controlled aerodromes, weather information is generally sourced from the ATIS. At uncontrolled aerodromes, weather information is generally available on the AWIS.

At landing areas without any published weather information, the QNH can be determined by adjusting the altimeter subscale until the instrument reads the current elevation. Wind direction can be determined by assessing surrounding [environmental factors](#surface-winds).