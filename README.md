# Factory+ Smart Tool Common Data Structure

The CDS is a common order and format of variables taken from different devices to ensure data/metadata is gathered in a consistent format when stored and shared across the the Factory+ architecture.

This initial draft was created based on the Open Protocol Specification from Atlas Copco.

List of datatypes used for the variables in this CDS:
- String
- Boolean
- UInt

These datatypes are what is currently being used. Any other Sparkplug compliant datatype can be used for `User_Defined` variables.

Example variable: the last service date of the tool would be under `Smart_Tools/Bosch_Nexo_Nutrunner_1/Tool_Info/Last_Service_Date`.
