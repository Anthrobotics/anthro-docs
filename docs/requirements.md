# Requirements

In this section, we cover the requirements set out for the development, building, and shipping of Anthros. We also provide explanations for why such requirements are necessary for this project.

## Accessibility

- ***All design files, software, firmware, and documentation must be open-source under CC BY-SA-NC 4.0 licenses***. This ensures that information remains accessible to the public, developers and authors are properly credited for contributions, and remixing of files and designs for personal, educational or research purposes is allowed.
- ***Nothing can be patented***. Everything shall remain available for non-commercial  personal, educational or research purposes. Commercial licensing will be available. We will not patent any materials, nor allow patenting, as they stifle and inhibit freely accessible innovation for all. 
- ***Project files, documentation, and downloads will all be served through GitHub.*** Alternate hosting locations for files will be determined.

## Design 

- ***They must be musculoskeletal, safe, and compliant***. Robots with high-inertia designs are dangerous, and generally heavier. Humans evolved to have a great musculoskeletal system. Anthros will have them too.
- ***They must be customizable to take on any anthropomorphic appearance***. Too many humanoid robots are boring, and lack soul and character. Anthros will be unique and infinitely varied in appearance, personality and identity. Nothing is off the table here - from classic humanoid robot designs, to furry & scalie characters - all will be made possible.
- Everything shall be designed using software that is:
    - open-source, and free for commercial use; or is
    - licensed for commercial use.
- Hardware design software must support assemblies.
Examples of recommended software for hardware design includes:
    - Onshape
    - FreeCAD
Onshape is what we use, primarily due to it's seamless integration with the extensions created by K-Scale labs for URDF generation.

## Production 

- ***Anthros must be able to be built at home or in the garage***. Anthros will be the easiest and most affordable humanoids to build.
- ***Production must be scalable through added 3D-printing, laser cutting, and CNC machining capabilities.*** These additive and subtractive manufacturing methods are always improving in quality while decreasing in cost. Therefore, they provide us an excellent avenue for scaling commercial in-house production of anthros, while allowing small fabs and hobbyists to keep pace.
- ***Empower small fabs to produce anthros (under license)***. Using accessible tooling and a stable supply of core components from approved vendors will allow for smaller fabs and companies to start producing anthros. Licensing details will be worked out, but will ultimately be favored in benefiting the smaller fab, and help generate a wider selection of anthros for consumers to choose from. This will be a key factor in accelerating distrubuted and democratized manufacturing of humanoids.
- ***Moving to full vertical integration will be a gradual but constant process***. Achieving vertically integrated production of anthros will give us full control and security over our supply chain and quality. This will take time, and therefore, we must take steps to build toward this. Every year, we must produce more critical components in-house, starting with artificial muscles.

## Distribution 

- ***Files will be available on GitHub***. This ties into accessibility, but also for version control, release management, issue tracking, and more.
- ***Anthros will be sold through our webstore***. We will also sell through other online marketplaces, including the K-Scale Labs online store. As other 3rd-party fabs are stood up, they can also sell their custom anthros (under license).
- ***Anthros sold outside US/CAN must be ITAR compliant***. Some features may have to be removed for sale to the EU and other countries.

## Version Control

- ***Tracking for versions shall be simple: version X.X or vX.X***. Rapid iteration will mean moving through versions very quickly. Moving from v1.0 to v2.0 of a component's design would only take 10 iterations. We will remain flexible and adaptive to rapid changes.
- ***Naming conventions for components shall be a short, brief description of the item, with key elements separated by commas.*** For example, an M8  socket head bolt that is 40mm in length would be named "Bolt, M8, Socket Head, 40mm". 
- ***Part numbering of manufactured components shall follow this scheme:***

**AAAAA-BBBBB-CCCCC-YYYYMMDD-ZZZZ**

Where:

- AAAAA is the part name
- BBBBB is the part number
- CCCCC is the parent assembly
- YYYYMMDD is the Year/Month/Day of manufacture
- ZZZZ is the part revision 

Example: We have a mounting bracket for a drive motor, with the part number of 4, belonging to the torso assembly. It was manufactured on 12 May, 2025, and is revision B. The part record would be:

**MTRBRACKET-0004-TRSOASSY-20250412-B**

This numbering scheme can also be applied to COTS components not manufactured in-house, where:

- AAAAA is the name of the COTS component
- BBBBB is the model of the COTS component (as per the manufacturer)
- CCCCC is the parent assembly (no change from above)
- YYYYMMDD is the date the COTS component was physically inspected for serviceability
- ZZZZ is the revision of the COTS component (if applicable)

Example: A frameless brushless motor, model RI115-PH, belonging to the torso assembly. It was inspected on 15 May, 2025, passing inspection, and is revision A. The part record would be:

**MTRBLDCNOFRAME-RI115PH-TORSOASSY-20250415-A**
