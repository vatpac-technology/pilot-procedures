---
  title: Forecasts and Reports
---

--8<-- "includes/abbreviations.md"

## Aviation Products
### METAR
A **METAR** is a snapshot report indicating the current meteorological conditions at the time the report is issued. In the context of flight simulation, it can be used to aid situational awareness and conduct performance calculations, but not for any flight planning purposes. METARs are published on a fixed time schedule, generally every thirty minutes.

### SPECI
A **SPECI** is a METAR which has been published outside of the regular cycle due to abnormal weather conditions or large meteorological changes since the last report. It serves the same purpose as a METAR and cannot be used for flight planning purposes.

SPECIs may be published for a range of conditions, including:

- A sudden shift in wind, temperature, or QNH
- Visibility below the alternate minima or 5km
- BKN or OVC cloud below the alternate minima or 1,500ft
- Significant weather such as thunderstorms or fog

### TAF
A **TAF** is an aviation forecast which covers a small radius of the nominated location. It can be used to determine the forecast weather conditions at an aerodrome for the purposes of [flight planning](../flight-planning/fuelplanning.md#weather-holdingalternate-fuel).

TAFs at some major aerodromes include the **TAF3** remark, indicating that they are updated more frequently and to a more accurate standard during the first three hours of their validity. Some flight planning concessions apply to TAF3s, which are detailed in AIP ENR 1.1 10.

### Area Forecasts
A number of visual area forecasts are available, which provide forecast weather conditions in a wider area. These can be used to determine the enroute weather conditions (and any associated limitations) and to provide an appreciation for the weather at aerodromes without a dedicated weather report/forecast.

Area forecasts are generally available on the NAIPS website and include GAF (for use at or below A100) and SIGWX (for use between A100 and F630) products.

## Where to Find Them
METARs and TAFs can be sourced from a number of sources.

- [NAIPS](https://www.airservicesaustralia.com/naips/): Real world system maintained by Airservices Australia, providing access to reports, forecasts, first/last light calculations, a large variety of meteorological charts, and more
- [VATPAC Pilot Tool](https://vatpac.org/membership-hub/tools/pilot): An all-in-one tool providing access to weather reports, forecasts, and ATISes, as well as easy access to aerodrome charts for your nominated origin and destination
- [VATPAC Weather Data Tool](https://vatpac.org/membership-hub/tools/wx): A dedicated tool allowing members to access weather reports, forecasts, and ATISes, without linking a specific VATSIM flight

## Interpreting Data
### Written Reports/Forecasts
METARs/SPECIs and TAFs reference the following datums:

| Element | Datum |
| ------- | ----- |
| Wind | Degrees *true* |
| Cloud | Feet AAL |

### METAR
METARs/SPECIs follow a specific format which makes interpreting them straightforward.

!!! note "Format"

    ``` mermaid
        flowchart LR        
        A[*METAR/SPECI*] --- B[Location] --- C[Timestamp] --- D[*AUTO*];
    ```
    ``` mermaid
        flowchart LR
        E[Wind] --- F[Visibility] --- G[Weather] --- H[Cloud];
        E --- Z[*CAVOK*] --- I[Temperature/Dew Point];
        H --- I;
    ```
    ``` mermaid
        flowchart LR
        J[QNH] --- K[Other Remarks];
    ```

Visibility, weather, and cloud will be omitted when the requirements of CAVOK are met.

!!! example
    `METAR YSSY 220000Z 13011KT 9999  SHOWERS IN VICINITY SCT035 SCT045 BKN055 19/17 Q1019 RMK RF00.0/000.4`

Recent rainfall is commonly included in the remarks section, displaying the amount of rain in the previous 10 minutes and the amount of rain since 9am local time (separated by a forward slash). In the METAR example above, YSSY has had 0mm of rain the past 10 min and 0.4mm of rain since 9am local.

### TAF
TAFs are comprised of a header and footer section, with the actual forecast weather contained between.

!!! example
    ```
    TAF YSSY 212309Z 2200/2306
    09014KT 9999  LIGHT RAIN SCT008 BKN020
    FM220800 08016KT 9999 SHOWERS OF LIGHT RAIN SCT008 BKN013
    FM222000 04016KT 9999 SHOWERS OF LIGHT RAIN SCT008 BKN013
    BECMG 2300/2302 04016KT 9999 SHOWERS OF LIGHT RAIN SCT010 BKN016
    TEMPO 2200/2208 07015G25KT 2000 SHOWERS OF MODERATE RAIN BKN008 SCT020TCU
    TEMPO 2208/2306 05020G30KT 2000 SHOWERS OF MODERATE RAIN BKN008 SCT020TCU
    RMK
    T 19 18 18 18 Q 1019 1017 1016 1017
    TAF3 
    ```

#### Header
!!! note "Format"

    ``` mermaid
        flowchart LR
        A[*TAF*] --- B[Location] --- C[Timestamp] --- D[Valid From/Valid To]
    ```

The validity period expresses time as a four digit timestamp in the format of *DDHH*. In the example below, the forecast is valid from 2200 (0000z on the 22nd day of the month) until 2306 (0600z on the 23rd day of the month).

!!! example
    `TAF YSSY 212309Z 2200/2306`

#### Weather
Each line of the TAF represents a period of time and the associated forecast weather for that period.

!!! note "Format"
    
    ``` mermaid
        flowchart LR
        A[Change Indicator] --- B[Wind] --- C[Weather] --- D[Cloud]
    ```

The first line of the TAF has no change indicator and is valid from the commencement of the validity period.

!!! example
    ```
    09014KT 9999  LIGHT RAIN SCT008 BKN020
    FM220800 08016KT 9999 SHOWERS OF LIGHT RAIN SCT008 BKN013
    ```

Several change indicators are used to indicate that the associated weather is only relevant during a given time period.

| Abbreviation | Meaning |
| ----- |---- |
| **FM** | The weather is expected to change *from* the given timestamp onwards, until the next change indicator |
| **BECMG** | The weather is expected to change slowly between the two four digit (*DDHH*) timestamps, until the next change indicator |
| **INTER** | The forecast weather is expected to be present for periods of up to 30 min between the two four digit (*DDHH*) timestamps |
| **TEMPO** | The forecast weather is expected to be present for periods of up to 60 min between the two four digit (*DDHH*) timestamps |

Where there is a probability of thunderstorms or poor visibility, an INTER/TEMPO will be prefixed with either **PROB30** or **PROB40**.

!!! example
    A TAF detailing `PROB30 TEMPO 2202/2204 VRB20G30KT 2000 SHOWERS OF MODERATE RAIN BKN003 SCT025TCU` would describe a 30% probability of up to 60 min of gusty, variable wind, showers of rain, and low cloud between 0200z and 0400z on the 22nd day of the month.

#### Remarks
The end of the TAF forecasts the outside air temperature and QNH at three hour intervals. Additional remarks may be included, such as indicating the forecast's TAF3 status.

!!! example
    ```
    RMK
    T 19 18 18 18 Q 1019 1017 1016 1017
    TAF3 
    ```

### Common Abbreviations
The VFRG (and AIP GEN 3.5) lists common abbreviations used in aviation meteorological products. A small selection are shown below:

| Abbreviation | Weather Descriptor |
| ---- | --- |
| BC | Patches |
| BL | Blowing |
| DR | Drifting |
| FZ | Freezing |
| MI | Shallow |
| SH | Showers |
| TS | Thunderstorms |
| PR | Partial |
| VC | Vicinity |

| Abbreviation | Weather Phenomena |
| ---- | ---- |
| BR | Mist |
| DU | Dust |
| FG | Fog |
| FU | Smoke |
| HZ | Haze |
| RA | Rain |
| VA | Volcanic Ash |

!!! example
    A METAR detailing `SHRA` would describe **showers** of **rain**.  

    A METAR detailing `VCTS` would describe **thunderstorms** in the **vicinity**.  

    A METAR detailing `BLDU` would describe **blowing dust**.

### Intensity Qualifiers
Precipitation, dust storms, and sandstorms may be prefixed with an intensity qualifier to denote how intense the weather phenomenum is.

| Prefix | Meaning |
| --- | --- |
| - | Light |
| | Moderate |
| + | Heavy |

!!! example
    A METAR detailing `+SHRA` would describe **heavy showers** of **rain**.

### Weather Information Services
Weather services like AWIS and ATIS reference the following datums:

| Element | Datum |
| ------- | ----- |
| Wind | Degrees *magnetic* |
| Cloud | Feet AAL |