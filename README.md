# factoryplus-cds-smarttools


The Common Data Structure (CDS) for Smart Tools in JSON format.

The CDS is a common order and format of variables taken from different devices to ensure data/metadata is gathered in a consistent format when stored on the Factory+ network.

This initial draft was created based on the Open Protocol Specification from Atlas Copco.

List of datatypes used for the variables in this CDS:

- String
- Boolean
- UInt

These datatypes are what is currently being used. Any other Sparkplug compliant datatype can be used for "User_Defined" variables.

Example variable: the last service date of the tool would be under "Smart_Tools/Bosch_Nexo_Nutrunner_1/Tool_Info/Last_Service_Date".

## Future work
Can potentially upload a tag structure diagram to this repository to be able to better visualise the hierarchy. This would need to be kept upto date as the CDS structure is updated in future merges - may be worth doing programmatically in the future; automatically generate a diagram as edits are made to the JSON file?


## Notes/changes:

06/01/2021
- Updated names to use `Title Case` convention
- Added top-level folder of "Smart Tools" which will be the DeviceType for this dataset when used in an Origin Map.

11/01/2021
- changed from Title Case to Pascal_Snake_Case to be consistent with the rest of Factory+ naming (as there were issues with spaces in the group id of the topic structure).

22/01/2021
- added PSET number select as one of the commands

25/01/2021
- removed `Metric Name` as the top level item
- put `User_Defined` as a folder under the `Smart_Tools/<Smart_Tool_Name>/` folder structure. This is now consistent with all CDSs
