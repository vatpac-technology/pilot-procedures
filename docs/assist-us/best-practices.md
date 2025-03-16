---
  title: Best Practices
---

--8<-- "includes/abbreviations.md"

When contributing to this project, aim to follow the best practices outlined below to ensure your changes are standardised and fit in with the existing format.

## File Names
Ensure new files are named lowercase only, so that the menu items are sorted alphabetically in a predictable way.

## Links

All links that navigate a user away from the SOPs site should have `{target=new}` appended - this opens the link in a new tab.

=== "Internal Link"

    ``` md
    [Internal Link](enroute.md)
    ```

=== "External Link"

    ``` md
    [External Link](https://vatpac.org){target=new}
    ```

!!! warning
    All external links should use the `https` protocol.

## ATC Unit Names
Where available, controller positions should be referred to by their callsign (e.g. Sydney Director).  Where multiple positions are discussed in close proximity, consider **bolding** the sector names.

## Altitudes
Describe any altitudes in the format of `Axxx` (for altitudes below 10,000ft) or `Fxxx` (for flight levels above 10,000ft) and wrap them in backticks.

!!! example
    ``` md
    The procedure should be flown at `A010`
    ```  
    The procedure should be flown at `A010`

## Radio Calls & Coordination
It is recommended to include an example highlighting any unique or lesser-known radio calls which apply to a procedure. Where applicable, a reference should be included to the AIP or other source which refers to that radio call/procedure.

### Example Radio Call Formatting
Example radio calls should take the following format:  

``` md
**STATION NAME**: "Message"
```

!!! example
    **VOZ1545**: "VOZ1545, request descent"  
    **HUO**: "VOZ1545, descend to FL130" 

### Phraseology Formatting
To maintain consistency with the format used in AIP GEN, wrap pieces of information which should be replaced by actual data by the pilot in brackets and italicize them. Any optional items should be wrapped in square brakets.

Radio call formats should be wrapped in a `!!! note "Format"` admonition. In situations where the context makes it obvious that the contents are the format of the call, you can remove the header with ```!!! note ""`. Consider following a Format admonition with an Example admonition, for clarity.

``` md
    *(ATC unit)*, *(aircraft callsign)*, descending to *(cleared level)*, received *(ATIS identifier)*, *[(inflight conditions)]*
```

!!! example
    Contact Adelaide Approach and request clearance for the procedure.

    !!! note "Format"
        "Adelaide Approach, *(your callsign)*, *(your position)*, *(your altitude)*, received *(ATIS identifier)*, request coastal northbound"