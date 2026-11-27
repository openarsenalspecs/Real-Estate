# HelixPlan
**The geometry was always there.**
- HTML Mirror:  [https://roxanneardary.com/helixplan-specification/](https://roxanneardary.com/helixplan-specification/)  

---

HelixPlan is an open-source spatial intelligence specification designed to reconstruct detailed architectural floorplans and three-dimensional property models from ordinary video walkthroughs and minimal dimensional inputs. By combining computer vision, spatial mapping, depth estimation, temporal analysis, and AI-driven architectural reasoning, HelixPlan transforms visual recordings of real-world interiors into structured, measurable, and editable representations of physical spaces.

The specification establishes a modular system capable of identifying rooms, walls, doors, windows, closets, hallways, stairs, fixtures, and other architectural features. It uses basic property dimensions, such as overall length and width, to establish scale and can incorporate additional measurements, reference objects, and sensor data to improve reconstruction accuracy.

HelixPlan is designed to serve homeowners, renters, real estate professionals, architects, interior designers, contractors, property managers, accessibility specialists, and developers. Its outputs support floorplan creation, property marketing, renovation planning, interior design, spatial analysis, and digital property documentation.

The system maintains a distinction between directly observed, user-supplied, calculated, inferred, and AI-estimated information. Every reconstruction must communicate measurement confidence, uncertainty, and potential discrepancies rather than presenting uncertain geometry as verified fact.

## Core Objectives

- Reconstruct detailed architectural floorplans from ordinary video walkthroughs.
- Generate accurate, editable two-dimensional floorplans and optional three-dimensional property models.
- Establish real-world scale using basic property dimensions and optional reference measurements.
- Identify and classify architectural structures, rooms, openings, fixtures, and spatial relationships.
- Maintain geometric consistency across video frames and reconstructed spaces.
- Apply architectural constraints to identify impossible, inconsistent, or implausible geometry.
- Automatically calculate and verify room dimensions, wall lengths, areas, and structural measurements.
- Support single-floor, multi-floor, and multi-building properties.
- Provide interactive editing and correction capabilities.
- Generate property marketing materials from verified spatial reconstructions.
- Support renovation, interior design, furniture planning, accessibility analysis, and property documentation.
- Preserve the distinction between measured property characteristics and AI-generated presentation enhancements.
- Support local processing, encrypted data storage, and user-controlled information retention.
- Provide an extensible architecture for additional spatial intelligence capabilities.

---

## Core System Modules

### Video Acquisition and Processing Module

Provides the initial video ingestion and preparation capabilities required to reconstruct physical spaces from recorded walkthroughs.

- Import video recordings from mobile devices, cameras, and supported recording sources.
- Support common video formats and variable recording resolutions.
- Extract individual frames and identify useful reconstruction frames.
- Perform automated keyframe selection to reduce redundant processing.
- Analyze camera movement, orientation, rotation, and translation.
- Detect motion blur, poor lighting, compression artifacts, and insufficient visual coverage.
- Stabilize video sequences where possible.
- Identify duplicated, obstructed, or unusable frames.
- Track recording continuity and identify transitions between rooms.
- Detect potential walkthrough gaps and areas requiring additional footage.
- Evaluate video quality and provide recommendations for improving reconstruction.
- Preserve source video metadata where available.
- Support multiple video segments representing different areas or floors of the same property.

### Dimensional Input and Calibration Module

Establishes the relationship between visual reconstruction and real-world physical measurements.

- Accept basic property dimensions, including overall length and width.
- Support optional ceiling heights, room dimensions, wall measurements, and doorway measurements.
- Allow users to provide known reference object dimensions.
- Identify potential scale references within video footage.
- Normalize reconstructed geometry against supplied measurements.
- Calibrate camera movement and spatial scale.
- Account for perspective distortion and camera positioning.
- Detect inconsistencies between supplied dimensions and reconstructed geometry.
- Support metric and imperial measurement systems.
- Maintain measurement provenance.
- Distinguish user-supplied dimensions from automatically calculated and AI-estimated measurements.
- Allow additional measurements to refine existing reconstructions.
- Report scale confidence and calibration uncertainty.

### Computer Vision and Scene Understanding Module

Analyzes video frames to identify architectural structures, objects, and spatial features.

- Detect walls, floors, ceilings, doors, windows, and structural openings.
- Identify rooms, closets, hallways, walkways, and connecting spaces.
- Recognize stairs, landings, and changes in floor elevation.
- Detect architectural fixtures and permanent installations.
- Identify furniture, appliances, and movable objects.
- Distinguish structural elements from temporary objects and visual obstructions.
- Recognize wall intersections, corners, edges, and boundaries.
- Estimate room boundaries and spatial relationships.
- Identify door and window positions and approximate dimensions.
- Detect partially visible architectural features.
- Recognize open-plan spaces and connected rooms.
- Track identified structures across multiple video frames.
- Assign confidence values to detected objects and architectural features.
- Preserve uncertainty when visual evidence is incomplete.

### Three-Dimensional Reconstruction and Spatial Mapping Module

Transforms visual observations into a coherent representation of the property's physical geometry.

- Generate spatial maps from video walkthroughs.
- Support Structure-from-Motion reconstruction.
- Support simultaneous localization and mapping.
- Estimate camera trajectories and relative camera positions.
- Generate point clouds and depth maps.
- Reconstruct surfaces, walls, floors, and ceilings.
- Generate three-dimensional architectural meshes.
- Align spatial observations collected from different camera positions.
- Detect overlapping and duplicated geometry.
- Correct spatial drift and alignment errors.
- Reconcile visual reconstruction with supplied property dimensions.
- Support multiple connected rooms and architectural spaces.
- Support multi-floor and multi-building spatial relationships.
- Maintain coordinate systems and consistent spatial references.
- Preserve reconstruction confidence and geometric uncertainty.

### Spatial Graph and Relationship Module

Maintains a unified representation of the property's geometry, architectural elements, and spatial relationships.

- Represent rooms, walls, doors, windows, stairs, closets, and hallways as connected spatial entities.
- Maintain relationships between rooms and architectural boundaries.
- Represent navigable paths and room connectivity.
- Track openings and access points between spaces.
- Maintain vertical relationships between floors and staircases.
- Associate measurements and confidence values with individual spatial elements.
- Maintain a shared spatial model used by floorplan, three-dimensional visualization, measurement, and marketing modules.
- Propagate approved corrections across dependent representations.
- Preserve relationships when individual elements are edited.
- Track changes and maintain revision history.
- Support multiple representations of the same underlying property.
- Provide a consistent source of spatial information for all downstream modules.

### Structural Constraint and Architectural Reasoning Module

Applies architectural and geometric reasoning to identify structural inconsistencies and impossible spatial relationships.

- Verify that doors connect appropriate spaces.
- Validate room enclosure and open-plan relationships.
- Evaluate hallway and walkway dimensions.
- Check wall continuity and intersections.
- Validate window placement relative to walls and exterior boundaries.
- Check stair alignment between floors.
- Evaluate stair rise, run, landing, and vertical continuity where measurements permit.
- Detect overlapping walls, disconnected structures, and impossible intersections.
- Identify doors or windows positioned outside plausible structural boundaries.
- Detect conflicting room dimensions and inconsistent floor elevations.
- Evaluate architectural relationships without assuming that every property follows conventional layouts.
- Identify potential structural anomalies.
- Suggest corrections without silently changing measured geometry.
- Distinguish architectural plausibility from verified building-code compliance.

### Temporal Consistency and Video Stability Module

Maintains consistent architectural reconstruction across multiple frames and camera positions.

- Analyze optical flow and cross-frame visual alignment.
- Track architectural features throughout video sequences.
- Maintain stable identification of walls, doors, windows, and other permanent structures.
- Detect changes caused by camera movement and perspective.
- Reduce inconsistent measurements between frames.
- Fuse observations from multiple frames using confidence-weighted geometry.
- Correct accumulated spatial drift.
- Identify temporary occlusions and partial visibility.
- Reconcile conflicting observations from different camera positions.
- Detect reconstruction instability and low-confidence regions.
- Preserve temporal relationships between observations.
- Prevent transient objects and visual artifacts from being incorrectly interpreted as permanent architectural structures.

### Floorplan Generation Module

Generates detailed architectural floorplans from the reconstructed spatial model.

- Generate editable two-dimensional floorplans.
- Generate optional three-dimensional architectural representations.
- Identify and draw room boundaries.
- Represent walls, wall thickness, corners, and structural intersections.
- Position doors and display door swings.
- Position windows and represent their dimensions.
- Include closets, hallways, walkways, and connecting spaces.
- Represent staircases, landings, and floor transitions.
- Generate room labels and architectural annotations.
- Calculate room dimensions and floor areas.
- Display overall property dimensions.
- Support open-plan layouts and irregularly shaped rooms.
- Preserve architectural relationships and spatial connectivity.
- Support individual room views and complete property layouts.
- Generate floor-specific and combined multi-floor plans.
- Provide editable dimensions, labels, and structural elements.
- Identify missing information and uncertain boundaries.
- Maintain consistency between two-dimensional and three-dimensional representations.

### Room Recognition and Classification Module

Identifies individual spaces and assigns meaningful classifications.

- Recognize bedrooms, bathrooms, kitchens, living rooms, dining rooms, offices, laundry rooms, storage rooms, and other common spaces.
- Identify closets, pantries, utility areas, and walk-in storage.
- Distinguish enclosed rooms from open-plan areas.
- Identify transitional spaces, hallways, entrances, and connecting areas.
- Recognize rooms based on visual characteristics, fixtures, and spatial relationships.
- Support user-defined room categories.
- Allow users to correct room classifications.
- Calculate room dimensions and usable floor area.
- Identify potentially incomplete or partially reconstructed rooms.
- Maintain room classification confidence.
- Support multiple possible classifications when visual evidence is ambiguous.

### Automated Measurement Verification Module

Validates measurements and identifies discrepancies throughout the reconstruction process.

- Calculate room lengths, widths, areas, and perimeter measurements.
- Calculate wall lengths and approximate wall thicknesses where supported.
- Estimate door and window dimensions.
- Measure closet, hallway, and walkway dimensions.
- Calculate stair dimensions and vertical relationships where sufficient data exists.
- Verify reconstructed dimensions against user-supplied measurements.
- Detect scale drift and accumulated measurement errors.
- Identify conflicting dimensions between connected rooms.
- Compare measurements against architectural plausibility constraints.
- Report measurement confidence and uncertainty ranges.
- Flag discrepancies and incomplete measurements.
- Recommend additional measurements when necessary.
- Distinguish observed, user-supplied, calculated, inferred, and AI-estimated values.
- Maintain measurement provenance and revision history.
- Never present an estimate as a verified measurement.

### AI Spatial Reasoning and Refinement Module

Uses contextual spatial analysis to improve reconstruction quality while preserving the distinction between evidence and inference.

- Analyze incomplete or partially obscured architectural features.
- Infer likely room boundaries when direct visual evidence is limited.
- Identify probable wall continuations and structural alignments.
- Resolve competing geometric interpretations using available evidence.
- Evaluate room adjacency and navigability.
- Refine floorplan geometry using architectural relationships.
- Identify potential missing doors, windows, and connecting spaces.
- Suggest corrections for inconsistent geometry.
- Use confidence-weighted refinement.
- Preserve original observations and user-supplied measurements.
- Record AI-generated modifications and their supporting evidence.
- Allow users to approve, reject, or modify suggested corrections.
- Avoid silently replacing verified measurements with inferred values.

### Multi-Floor and Multi-Structure Module

Supports properties containing multiple levels, separate structures, and interconnected buildings.

- Reconstruct individual floors independently.
- Align floorplans using staircases, structural walls, and known reference points.
- Identify staircases, landings, and vertical circulation.
- Maintain floor-to-floor relationships.
- Support basements, attics, mezzanines, and partial levels.
- Reconstruct detached garages, guest houses, and accessory structures.
- Represent connecting walkways and covered transitions.
- Combine individual structures into a unified property model.
- Generate individual floorplans and combined property views.
- Maintain separate dimensions and measurements for each structure.
- Identify inconsistencies between vertically aligned architectural features.

### Interactive Editing and Correction Module

Provides users with direct control over reconstructed geometry and architectural information.

- Allow manual adjustment of walls, rooms, doors, and windows.
- Add, remove, and reposition architectural elements.
- Correct room boundaries and classifications.
- Edit labels, dimensions, and annotations.
- Adjust wall thickness and other geometric properties.
- Merge or divide rooms.
- Correct room connectivity and navigable paths.
- Modify staircases and floor relationships.
- Compare original reconstruction with edited versions.
- Display confidence and uncertainty information during editing.
- Preserve original observations separately from user corrections.
- Maintain revision history and change attribution.
- Allow users to accept or reject AI-generated suggestions.
- Recalculate dependent measurements and spatial relationships after approved edits.
- Support collaborative review and correction workflows.

### Three-Dimensional Visualization and Virtual Property Module

Provides interactive visualization of reconstructed properties.

- Render reconstructed interiors and architectural structures.
- Generate navigable three-dimensional property models.
- Display walls, floors, ceilings, doors, windows, stairs, and permanent fixtures.
- Support adjustable camera positions and viewing angles.
- Provide room-by-room navigation.
- Display floor-specific and complete property views.
- Allow users to inspect measurements and architectural details.
- Synchronize approved changes with the shared spatial model.
- Support optional furniture and interior presentation layers.
- Provide visual comparison between reconstructed and edited geometry.
- Support immersive property presentations where compatible.
- Clearly distinguish reconstructed property geometry from decorative visualization elements.

### Real Estate Marketing Module

Transforms verified spatial reconstructions into professional property marketing materials while preserving factual accuracy.

- Generate marketing-ready two-dimensional floorplans.
- Generate optional three-dimensional property layouts.
- Create room-by-room property presentations.
- Produce property layout summaries and spatial highlights.
- Generate listing descriptions using verified property information.
- Create marketing copy based on room counts, dimensions, layout, and property features.
- Generate property brochures and presentation materials.
- Create visual floorplan variations suitable for listing platforms and marketing campaigns.
- Generate interactive floorplan presentations.
- Produce virtual property walkthrough experiences from reconstructed models.
- Support optional virtual staging and furniture placement.
- Support optional interior style variations and decorative presentation.
- Generate property photography enhancement workflows where supported.
- Create social media and digital advertising assets.
- Support real estate agent, broker, property manager, and owner branding.
- Support customizable templates and presentation styles.
- Export marketing materials in common document and image formats.
- Generate property-specific marketing packages.
- Support multiple listing presentation formats.
- Allow users to compare staged and unstaged visualizations.
- Clearly identify AI-generated staging, decorative enhancements, and simulated furnishings.
- Never represent virtual staging or generated imagery as actual property conditions.
- Never alter verified room dimensions or structural geometry for marketing purposes.
- Preserve the distinction between factual property information and promotional descriptions.
- Require user review and approval before publishing generated listing content.
- Maintain source information and measurement provenance for published floorplans.

### Renovation and Interior Design Module

Uses reconstructed spatial information to support property improvements and design planning.

- Provide editable room layouts for renovation planning.
- Support wall, doorway, and window modification proposals.
- Compare existing and proposed floorplans.
- Identify available wall and floor space.
- Support kitchen, bathroom, bedroom, and living-area redesign.
- Allow users to explore alternative room configurations.
- Generate conceptual renovation layouts.
- Support interior design planning and visualization.
- Identify potential conflicts between proposed changes and existing structures.
- Estimate affected room dimensions and usable floor area.
- Support material and finish visualization.
- Maintain separate existing-condition and proposed-design models.
- Clearly distinguish conceptual design suggestions from engineering or construction documentation.

### Furniture and Space Optimization Module

Analyzes available space and supports practical furniture arrangement.

- Identify available floor space and room dimensions.
- Support furniture placement and rearrangement.
- Evaluate furniture fit within reconstructed rooms.
- Calculate clearance around furniture and fixtures.
- Analyze circulation paths and access areas.
- Identify potential obstructions.
- Suggest alternative furniture arrangements.
- Support user-defined furniture dimensions.
- Provide optional furniture libraries.
- Generate staged and furnished room visualizations.
- Compare furnished and unfurnished layouts.
- Preserve verified architectural geometry while modifying presentation layers.

### Accessibility and Mobility Analysis Module

Evaluates reconstructed spaces for accessibility and practical movement.

- Analyze doorway widths and passage dimensions where measurable.
- Identify potential navigation barriers.
- Evaluate hallway and walkway clearances.
- Analyze room access and circulation paths.
- Identify stairways and changes in elevation.
- Evaluate potential wheelchair and mobility-device access limitations.
- Identify restricted turning and maneuvering areas.
- Support user-defined accessibility criteria.
- Generate accessibility observations and measurement reports.
- Highlight uncertain or unmeasured accessibility characteristics.
- Support comparisons between existing and proposed layouts.
- Avoid representing automated observations as formal accessibility certification or code compliance.

### Building Documentation and Digital Twin Module

Maintains a structured digital representation of a property's reconstructed physical layout.

- Maintain property-level spatial records.
- Store architectural geometry and room relationships.
- Associate measurements with individual building elements.
- Maintain floor-specific and structure-specific documentation.
- Record user corrections and approved revisions.
- Support updated walkthroughs and reconstruction comparisons.
- Identify changes between property scans.
- Maintain historical floorplan versions.
- Support property condition documentation.
- Provide structured spatial data for compatible property management systems.
- Maintain links between visual evidence and reconstructed elements.
- Support long-term property documentation and digital twin development.
- Clearly identify the date and source of each reconstruction.

### Dataset Generation and Model Training Module

Supports the creation of structured datasets for improving spatial reconstruction capabilities.

- Convert approved walkthrough videos into structured training examples.
- Generate video, frame, point cloud, depth map, and floorplan training pairs.
- Associate semantic labels with architectural elements.
- Preserve room, wall, door, window, and structural annotations.
- Generate synthetic properties using procedural architectural layouts.
- Vary lighting, camera movement, perspective, occlusion, and recording conditions.
- Support synthetic multi-floor and irregular property layouts.
- Incorporate approved user corrections as training feedback.
- Validate dataset quality and annotation consistency.
- Track dataset provenance and licensing.
- Maintain separation between public, private, and restricted datasets.
- Require explicit user consent before using contributed recordings, property models, or corrections for training.
- Provide dataset contribution controls and withdrawal procedures where applicable.
- Prevent private property recordings from becoming training data without authorization.

### Privacy, Security, and Data Ownership Module

Protects user recordings, property information, and reconstructed spatial data.

- Support local and offline processing.
- Provide encrypted storage for videos, images, measurements, and reconstructed property models.
- Protect data during transmission and synchronization.
- Provide user-controlled data retention and deletion.
- Allow users to control access to property models and recordings.
- Support private projects and restricted sharing.
- Provide optional redaction of sensitive visual information.
- Support removal or obscuring of personal items and identifying details.
- Separate identity information from public property presentations where applicable.
- Maintain access and modification records.
- Require explicit consent for dataset contributions and model training.
- Prevent unauthorized use of private property data.
- Provide transparent data handling and processing controls.
- Ensure privacy and security capabilities are available across all supported configurations.

### Export and Interoperability Module

Provides access to reconstructed property information through reusable and compatible formats.

- Export editable two-dimensional floorplans.
- Export three-dimensional property models.
- Export point clouds, meshes, and spatial maps where supported.
- Export room dimensions, wall measurements, and architectural annotations.
- Export property summaries and measurement reports.
- Support common architectural, image, and three-dimensional exchange formats.
- Provide structured spatial data exports.
- Preserve coordinate systems, units, and measurement provenance.
- Support individual floor and complete property exports.
- Support marketing-ready floorplan and presentation exports.
- Maintain consistency between exported files and the approved spatial model.
- Provide interoperability with compatible design, construction, real estate, and property management applications.

### API and Developer Integration Module

Provides controlled access to HelixPlan capabilities for external applications and services.

- Expose supported video ingestion and reconstruction capabilities.
- Provide access to spatial models and floorplan data.
- Support structured measurement and room information retrieval.
- Provide access to approved reconstruction and editing operations.
- Support property model import and export workflows.
- Provide integration capabilities for real estate platforms.
- Support compatible architectural and design applications.
- Provide access controls and authentication.
- Support permission-based access to private property data.
- Provide versioned interfaces and documented integration requirements.
- Maintain data validation and error reporting.
- Support event-based updates when approved property models change.

---

## Optional Plugin Modules

Optional plugins extend HelixPlan without making specialized capabilities mandatory for the core reconstruction system. Plugins must use documented interfaces, respect the shared spatial model, and preserve the system's privacy, security, provenance, and measurement integrity requirements.

### Advanced Sensor Integration Plugin

- Integrate supported depth sensors and depth cameras.
- Incorporate LiDAR scans and point cloud recordings.
- Import compatible laser measurement data.
- Incorporate inertial measurement unit data.
- Integrate supported distance and environmental sensors.
- Fuse sensor observations with video-based reconstruction.
- Improve scale calibration and geometric confidence.

### Advanced Architectural Analysis Plugin

- Provide expanded architectural relationship analysis.
- Support additional building geometry constraints.
- Analyze rooflines, ceiling structures, and complex interior transitions where data permits.
- Evaluate structural layout consistency.
- Provide advanced architectural anomaly detection.
- Support specialized architectural documentation workflows.
- Distinguish analytical observations from professional structural assessments.

### Building Code Reference Plugin

- Compare supported measurements and spatial features against selected building code references.
- Support jurisdiction-specific reference libraries.
- Identify potential dimensional and accessibility concerns.
- Provide source references and applicable code versions.
- Highlight areas requiring professional review.
- Clearly distinguish automated screening from official code interpretation, inspection, or compliance certification.

### Advanced Real Estate Listing Integration Plugin

- Connect to compatible real estate listing services.
- Prepare property marketing packages for supported platforms.
- Map approved property information to listing fields.
- Support listing image and floorplan preparation.
- Generate platform-specific marketing formats.
- Allow users to review and approve content before submission.
- Respect individual platform requirements and access permissions.

### Virtual Staging and Interior Style Plugin

- Generate optional furnished property visualizations.
- Apply selected interior design styles.
- Replace or modify decorative elements in presentation layers.
- Generate alternative furniture arrangements.
- Compare multiple staging concepts.
- Preserve the original reconstructed property geometry.
- Clearly identify generated and simulated elements.

### Advanced Virtual Reality and Immersive Presentation Plugin

- Convert reconstructed properties into immersive viewing experiences.
- Support compatible virtual reality and augmented reality devices.
- Provide interactive room navigation.
- Support spatial inspection and measurement overlays.
- Enable immersive property presentations.
- Synchronize approved changes with the underlying spatial model.

### Renovation Cost Estimation Plugin

- Associate proposed renovations with configurable material and labor estimates.
- Support user-defined regional pricing information.
- Estimate quantities using reconstructed measurements.
- Compare alternative renovation scenarios.
- Generate preliminary project cost summaries.
- Identify assumptions and missing information.
- Clearly distinguish preliminary estimates from contractor quotations and verified costs.

### Furniture Catalog and Retail Integration Plugin

- Connect to compatible furniture and furnishing catalogs.
- Import product dimensions and spatial requirements.
- Test furniture placement against reconstructed room geometry.
- Generate alternative furnishing arrangements.
- Provide optional product and catalog references.
- Support compatible purchasing and product information integrations.

### Property Management Integration Plugin

- Connect to compatible property management platforms.
- Associate floorplans with property records.
- Maintain property-level documentation.
- Support unit and building identification.
- Provide approved measurement and spatial data.
- Track changes between property reconstructions.

### Construction and Building Information Modeling Plugin

- Export compatible architectural and building information models.
- Support construction planning workflows.
- Associate spatial elements with additional building information.
- Support design coordination and model exchange.
- Provide existing-condition documentation.
- Distinguish reconstructed geometry from professionally verified construction measurements.

### Advanced Survey and Measurement Plugin

- Integrate compatible surveying and measurement instruments.
- Support reference point alignment.
- Improve dimensional calibration.
- Compare independent measurement sources.
- Generate detailed measurement discrepancy reports.
- Preserve measurement source and accuracy information.

### Outdoor and Site Mapping Plugin

- Extend spatial reconstruction to exterior property areas.
- Map yards, patios, driveways, walkways, and outdoor structures.
- Support property boundary references supplied by authorized sources.
- Incorporate compatible aerial imagery and site measurements.
- Generate combined interior and exterior property models.
- Distinguish estimated visual boundaries from surveyed property boundaries.

### Collaborative Review Plugin

- Support multiple authorized reviewers.
- Allow shared inspection and correction workflows.
- Provide comments and annotations.
- Track contributor changes.
- Support approval workflows for reconstructed and published property information.
- Maintain revision history and user permissions.

### Advanced Analytics and Reporting Plugin

- Generate detailed property measurement reports.
- Compare room dimensions and property layouts.
- Identify spatial utilization patterns.
- Analyze property layout characteristics.
- Generate customized reporting formats.
- Support portfolio-level property comparisons where authorized.

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/helixplan/](https://roxanneardary.com/helixplan/)  

---

## License & Notice Requirements

HelixPlan is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- HelixPlan specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
https://gitlab.com/Roxanne_Ardary/open-arsenal-specs

**Catalog**  
[Open Arsenal](https://roxanneardary.com/)  
[Specification Index](https://roxanneardary.com/wp-content/uploads/spec-index/specification-index.html)
