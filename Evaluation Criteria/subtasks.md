# Detailed Evaluation Criteria

| Index | Criteria | Description|
| :--- | :--- | :--- |
| 1 |Instructional Alignment | The response reflects an understanding of SAP methodology, procedural rules, and equations.|
| 2 |Factual Precision | The response makes use of numerical inputs that remain within 10% variance.|
| 3 |Source Attribution,The accuracy and appropriateness of referencing official SAP guidance or documentation.|
| 4 |Logical Coherence,"The clarity, completeness, and internal consistency of calculations and justifications.|





This table outlines the specific verification targets used to evaluate the LLM's performance for each module and subtask, based on the SAP 10.2 standard.

| Module | Subtask | Verification Target | Index |
| :--- | :--- | :--- | :--- |
| **Geometry** | Wall Area | Consider only external wall, and extract the opening area | 1 |
| | | Give the right area | 2 |
| | | Use the prompt-given dimension | 3 |
| | | Give step-by-step calculation | 4 |
| | **Floor Area** | Consider only ground floor | 1 |
| | | Use the right dimension | 2 |
| | | Use the prompt-given dimension | 3 |
| | | Give step-by-step calculation | 4 |
| | **Roof Area** | Consider slope roof, and extract the opening area | 1 |
| | | Use the right dimension | 2 |
| | | Use the prompt-given dimension | 3 |
| | | Give step-by-step calculation | 4 |
| | **Window Area** | Consider orientation | 1 |
| | | Use the right dimension | 2 |
| | | Use the prompt-given dimension | 3 |
| | | Give step-by-step calculation | 4 |
| | **TFA** | Consider correct floors | 1 |
| | | Use the right dimension | 2 |
| | | Use the prompt-given dimension | 3 |
| | | Give step-by-step calculation | 4 |
| **Heat loss calculation** | Fabric heat loss | Consider all the component (Wall, roof, floor, window, door) | 1 |
| | | Give the right U-value for each component | 2 |
| | | Calculate the right heat loss for each component | 3 |
| | | Give the right total heat loss | 4 |
| | | Give step-by-step calculation | 5 |
| **Ventilation loss calculation** | Infiltration | Identify the right infiltration rate based on the building type | 1 |
| | | Identify the right number of side sheltered | 2 |
| | | Consider the floor level | 3 |
| | | Calculate the right infiltration | 4 |
| | | Give step-by-step calculation | 5 |
| | **Ventilation** | Identify the right ventilation type | 1 |
| | | Calculate the right ventilation loss | 2 |
| | | Give step-by-step calculation | 3 |
| **Total heat loss parameter** | HLP | Calculate the right total heat loss parameter | 1 |
| | | Use the right floor area | 2 |
| | | Give step-by-step calculation | 3 |
| **Water heating demand** | Hot water usage | Calculate the right annual hot water usage | 1 |
| | | Consider the number of occupants | 2 |
| | | Give step-by-step calculation | 3 |
| **Calculate the internal gain** | Internal gain | Calculate the right internal gain for each category | 1 |
| | | Consider all the categories (Metabolic, Lighting, Appliances, Cooking, etc.) | 2 |
| | | Give the right total internal gain | 3 |
| | | Give step-by-step calculation | 4 |
| **Calculate the solar gain** | Solar gain | Calculate the right solar gain for each window/rooflight | 1 |
| | | Consider the orientation and shading | 2 |
| | | Give the right total solar gain | 3 |
| | | Give step-by-step calculation | 4 |
| **Utilisation factor** | Utilisation factor | Calculate the right utilisation factor | 1 |
| | | Consider the thermal mass | 2 |
| | | Give step-by-step calculation | 3 |
| **Internal temperatrue** | Internal temperature | Calculate the right mean internal temperature | 1 |
| | | Consider the heating period and controls | 2 |
| | | Give step-by-step calculation | 3 |
| **Space heating demand** | Space heating | Calculate the right space heating demand | 1 |
| | | Give step-by-step calculation | 2 |
| **Lighting electricity** | Lighting | Calculate the right lighting electricity | 1 |
| | | Consider the efficacy of the lamps | 2 |
| | | Give step-by-step calculation | 3 |
| **auxiliary electricity** | Auxiliary | Calculate the right auxiliary electricity | 1 |
| | | Consider pumps and fans | 2 |
| | | Give step-by-step calculation | 3 |
| **Renewable generation** | PV generation | Calculate the right PV generation | 1 |
| | | Consider the orientation and tilt | 2 |
| | | Give step-by-step calculation | 3 |
| **Delivered Energy** | Total energy | Calculate the right total delivered energy | 1 |
| | | Give step-by-step calculation | 2 |
| **Emission calculation** | CO2 Emission | Calculate the final CO2 emissions | 1 |
| | | Use the right emission factors | 2 |
| | | **TER** | Calculate the right Target Emission Rate | 3 |
