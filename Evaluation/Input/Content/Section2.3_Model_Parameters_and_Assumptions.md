### 2.3.1 Absorption

Intestinal permeability was fitted to po data. Formulation of ethinylestradiol tablet was modeled with Weibull-function and parameters `Dissolution time (50% dissolved)` and `Lag time` fitted to po data.

### 2.3.2 Distribution

Physico-chemical parameters were set to the reported values (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)). It was assumed that the major binding partner in plasma is albumin. The value of lipophilicity was estimated by fitting the model to iv and po data.

After testing the available organ-plasma partition coefficient and cell permeability calculation methods available in PK-Sim, observed clinical data were best described by choosing the partition coefficient calculation by `Berezhkovskiy` and cellular permeability calculation by `PK-Sim Standard`.

### 2.3.3 Metabolism and Elimination

Following metabolization processes have been implemented based on [Ezuruike 2018](#5-References):

- Linear CYP1A2 CL
- Linear CYP2C8 CL
- Linear CYP2C9 CL
- Linear CYP3A4 CL
- Saturable UGT1A1
- Unspecific liver metabolization

Renal plasma clearance is modeled with `Plasma clearance` set to 2.079 l/h reported in literature ([Stanczyk 2013](#5-References)). The value was normalized to body weight by dividing by 70 kg.

### 2.3.4 Enzyme Inhibition

Simulations of co-administration of ethinylestradiol with tizanidine (see [CYP1A2 DDI Qualification report](link)) indicate that the reported competitive inhibition of CYP1A2 by ethinylestradiol ([Karjalainen 2008](#5-References)) is not sufficient to describe the increased concentrations of tizanidine after multiple days administration. Therefore, it was decided to fit a time-dependent inhibition (TDI) function to the CYP1A2 enzyme system. The parameters `Kinact` and `K_kinact_half` were estimated by fitting the model to concentration-time profiles of tizanidine ([Granfors 2005](#5-References)).

### 2.3.5 Automated Parameter Identification

Following parameter values were estimated for the model:

- `Lipophilicity`
- `Specific intestinal permeability`
- `Dissolution time (50% dissolved)` (Weibull formulation)
- `Lag time` (Weibull formulation)
- `Kinact` (CYP1A2 TDI)
- `K_kinact_half` (CYP1A2 TDI)
