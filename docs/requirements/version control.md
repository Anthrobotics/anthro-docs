# Version Control

## Information for late-stage prototypes and production-ready components

- ***Tracking for versions shall be simple: version X.X or vX.X***. Rapid iteration will mean moving through versions very quickly. Moving from v1.0 to v2.0 of a component's design would only take 10 iterations. We will remain flexible and adaptive to rapid changes.
- ***Naming conventions for components shall be a short, brief description of the item, with key elements separated by commas.*** For example, an M8  socket head bolt that is 40mm in length would be named "Bolt, M8, Socket Head, 40mm".
- ***Some components will contain both a part record AND serial mumber***. This is for warranty  purposes, to aid in repairs, and to track high-value or controlled components.
- ***Part records of manufactured components shall follow this scheme:***

**AAAAA-BBBBB-CCCCC-YYYYMMDD-ZZ**

Where:

- AAAAA is the part name
- BBBBB is the part number
- CCCCC is the parent assembly
- YYYYMMDD is the Year/Month/Day of manufacture
- ZZ is the part revision 

Example: We have a mounting bracket for a drive motor, with the part number of 4, belonging to the torso assembly. It was manufactured on 12 May, 2025, and is revision B. The part record would be:

**MTRBRACKET-0004-TRSOASSY-20250412-B**

This record scheme can also be applied to COTS components not manufactured in-house, where:

- AAAAA is the name of the COTS component
- BBBBB is the model of the COTS component (as per the manufacturer)
- CCCCC is the parent assembly (no change from above)
- YYYYMMDD is the date the COTS component was physically inspected for serviceability
- ZZ is the revision of the COTS component (if applicable)

Example: A frameless brushless motor, model RI115-PH, belonging to the torso assembly. It was inspected on 15 May, 2025, passing inspection, and is revision A. The part record would be:

**MTRBLDCNOFRAME-RI115PH-TRSOASSY-20250415-A**

***Important notes for revision codes:***

- Codes denoting prototype components not yet approved or ready for release will start with the uppercase letter **X** followed by a version number of the prototype.
- Codes denoting components approved for production and release will be denoted with uppercase letters used in sequence, beginning with **A**. The letters **I, O, Q, X and Z** will be omitted. When the single letters have been exhausted, the revisions following **Y** shall be **AA, AB** through **AY**. Should **AA to AY** be exhausted, the next sequence shall be **BA, BB**, etc. Revision letters shall not exceed two characters. (as per ASME Y14.35M-1997, Section 5)

- ***The following manufactured components entering production for release models will be serialized based on class:
    - **PCBs (A)**
    - **Compute Systems (B)**
    - **Power Supplies (C)**
    - **Motors (D)**
    - **Communication Devices (E)**
    - **Sensors (F)**
- ***Components matching the above descriptions that are manufactured in-house will be designated a serial number using the following scheme:***

**X-YYYY-ZZZZZZZZ**

Where:

- X is the item class (see the list above)
- Y is the year of production
- Z is the item number, increasing in value by one for each item produced


