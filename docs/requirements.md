# Requirements

In this section, we cover the requirements set out for the development, building, and shipping of Anthros. We also provide explanations for why such requirements are necessary for this project.

## Accessibility

- ***All design files, software, firmware, and documentation must be open-source under appropriate licenses***. This ensures that information remains accessible to the public, developers and authors are properly credited for contributions, and remixing of files and designs for personal, educational or research purposes is allowed. The licenses are as follows:
    - **Hardware and Design Files** - **[CERN-OHL-S v2](https://ohwr.org/cern_ohl_s_v2.pdf)**
    - **Software and Firmware** - **[MIT](https://opensource.org/license/mit)**
    - **Documentation** - **[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)**
- ***Nothing can be patented***. Everything shall remain available for personal, educational or research purposes. Commercial use will be allowed. Patents stifle and inhibit freely accessible innovation for all, and go against the very principles of open-source work. 
- ***Project files, documentation, and downloads will all be served through GitHub.*** Alternate hosting locations for files will be determined.

## Design 

- ***They must be musculoskeletal, safe, and compliant***. Robots with high-inertia designs are dangerous, and generally heavier. Humans evolved to have a great musculoskeletal system. Anthros will have them too.
- ***They must be customizable to take on any anthropomorphic appearance***. Too many humanoid robots are boring, and lack soul and character. Anthros will be unique and infinitely varied in appearance, personality and identity. Nothing is off the table here - from classic humanoid robot designs, to furry & scalie characters - all will be made possible.
- ***Everything shall be designed using software that is***:
    - open-source, and free for commercial use; or is
    - licensed for commercial use.
- ***Hardware design software must support assemblies***.
Examples of recommended software for hardware design includes:
    - Onshape
    - FreeCAD
Onshape is what we use, primarily due to it's seamless integration with the extensions created by K-Scale labs for URDF generation.

## Production 

- ***Anthros must be able to be built at home or in the garage***. Anthros will be the easiest and most affordable humanoids to build.
- ***Production must be scalable through added 3D-printing, laser cutting, and CNC machining capabilities.*** These additive and subtractive manufacturing methods are always improving in quality while decreasing in cost. Therefore, they provide us an excellent avenue for scaling commercial in-house production of anthros, while allowing small fabs and hobbyists to keep pace.
- ***Empower small fabs to produce anthros***. Using accessible tooling and a stable supply of core components from approved vendors will allow for smaller fabs and companies partnered with Anthrobotics to start producing anthros. This will help scale production, and help generate a wider selection of anthros for consumers to choose from. This will be a key factor in accelerating distrubuted and democratized manufacturing of humanoids.
- ***Moving to full vertical integration will be a gradual but constant process***. Achieving vertically integrated production of anthros will give us full control and security over our supply chain and quality. This will take time, and therefore, we must take steps to build toward this. Every year, we must produce more critical components in-house, starting with artificial muscles.

## Distribution 

- ***Files will be available on GitHub***. This ties into accessibility, but also for version control, release management, issue tracking, and more.
- ***Anthros will be sold through our webstore***. We will also sell through other online marketplaces, including the K-Scale Labs online store. As other 3rd-party fabs partnered with Anthrobotics are stood up, they can also sell their custom anthros.
- ***Anthros sold outside US/CAN must be ITAR compliant***. Some features may have to be removed for sale to the EU and other countries.

## Version Control

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



 
