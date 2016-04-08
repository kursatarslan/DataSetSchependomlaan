**Dataset Schependomlaan**

This document contains information about the data set regarding the construction project Schependomlaan. All involved parties have given permission to use the data for scientific and academic purposes. The data is gathered during the master thesis project of Stijn van Schaijk. In collaboration with Hendriks Bouw en Ontwikkeling[1], ROOT[2], TNO[3] and RAAMAC[4] the data is collected. General information about the project can be found at the website http://www.schependomlaan.nl/ .

The dataset contains the following elements:
- Design model in .IFC
-  Subcontractor models in .IFC and .DWG
	   - Flooring
	   - Walls
	   - Stairs
	   - Fencing
	   - Steel
	   - Roofs
	   - Prefab
- Coordination models in .TBP (Tekla BIMsight Package)
- Schedule/Planning in .pdf and .xml
- As-planned models in .IFC and Synchro file format.
- As-built models in point cloud formats .ASCII and .PLY
- Results comparison as-planned and as-built models in .xls
- As-planned Event log in .xlsx and .csv
- As-built Event log in .xlsx and .csv
- Event log with actors in .xlsx and .csv

*Some files contain some errors and therefore have to be treated carefully.*

**Design model**
The design model IFC Schependomlaan.ifc is made in Archicad by ROOT bv. They modelled the project by order of Hendriks Bouw en Ontwikkeling. The project was originally drawn in 2D cad formats and was translated into a high quality BIM model. The design model is used as a reference during the engineering phase in collaboration with the subcontractors.

**Coordination model and Subcontractor models**
The models delivered by the subcontractors are coordinated in the file: Schependomlaan Nijmegen.tbp. This file can be opened using Tekla BIMsight5 and contains all the subcontractor models. Some subcontractors couldn’t deliver their products in BIM/.IFC. Those designs are aligned with the BIM using .DWG formats.

**Planning and as-planned models**
As-planned models are created by use of Synchro[6] software. The design IFC is connected by use of the .XML planning. The native Synchro file is available Synchro project Schependomlaan.sp . From Synchro as-planned models are exported to .IFC. A model containing all the planning information is exported called: IFC Schependomlaan incl planningsdata.ifc. As part of the study also as-planned models on specific dates had to be exported. So the following models have been made:
- Week 26 26 june IFC Schependomlaan incl planningsdata.ifc
- Week 27 3 july IFC Schependomlaan incl planningsdata.ifc
- Week 28 10 july IFC Schependomlaan incl planningsdata.ifc
- Week 29 17 july IFC Schependomlaan incl planningsdata.ifc
- Week 30 24 july IFC Schependomlaan incl planningsdata.ifc
- Week 37 11 sept IFC Schependomlaan incl planningsdata.ifc
Note that at the moment of writing Synchro does not have optimal IFC exporting options, as a result the data structure in IFC is changed during export. The elevation tree is changed and the property sets are changed. As can be seen in the figures below. One has to take this into account when working with this dataset.

**As-built Point clouds**
The construction site is filmed with drones over days during the project. The movies can be seen at the Youtube chanel of the drone pilot:
https://www.youtube.com/channel/UCHsKVCxqYaZn39JNZH7v9LQ
Movies of week 26, 27 , 28, 29 and 30 are used to create as-built point clouds using structure from motion techniques. The point clouds are available in .PLY, .ASCII and some in .LAS files. The point clouds are created by RAAMAC.

**Comparison as-planned as-built**
The as-built point clouds are compared with the as-planned IFC using a matlab algorithm by RAAMAC. As a result a comparison sheet is created. See the file: comparison_all weeks.xlsx

**Event logs**
Part of the research was to enable construction process mining. In order to do so event logs had to be created. Those files can be analysed in process mining tools. The as-planned event log is in the file eventlog IFC schependomlaan.csv . The event log containing as-built information is the file: Schependomlaan eventlog as planned data incl as built data.csv .
As part of an experiment also actors are added to an event log. Those actors are fake and not realistic. But to proof that social network analytics can be done with those data structures this file is made: Schependomlaan eventlog as planned data incl as built data incl Actors FAKE.csv .


[1] http://www.hendriksbouwenontwikkeling.nl/

[2] http://www.root-bv.nl/

[3] https://www.tno.nl/en/

[4] http://raamac.cee.illinois.edu/

[5] https://www.teklabimsight.com/

[6] https://synchroltd.com/
