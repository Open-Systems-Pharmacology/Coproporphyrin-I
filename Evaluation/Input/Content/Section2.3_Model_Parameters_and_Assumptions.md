### 2.3.1 Absorption

The parameter value for  `Specific intestinal permeability`  was set to 0 to not include intestinal reabsorption. This was informed by non-successful parameter identification's going to very low values and fixing the parameter to the calculated one resulted in unreasonable fits and the fraction excreted to feces was not consistent with literature ([Section 2.2.1](#221-in-vitro-and-physicochemical-data)). The solubility was obtained from DrugBank (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

The synthesis rate was modelled as a zero-order infusion over one year into intracellularly in the liver. This was informed by first modelling a synthesis rate in MoBi according to the value stated in literature and then translating it into a zero-order infusion in PK-Sim ([Mochizuki 2022](#5-references)). 

### 2.3.2 Distribution

Coproporphyrin-I is highly bound to plasma proteins (>99 %) (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)). A value of 0.66% was used in this PBPK model for `Fraction unbound (plasma, reference value)`. The major binding partner was set to albumin (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

An important parameter influencing the resulting volume of distribution is lipophilicity. The reported logP value of  2.53 (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)) is used in this model.

The partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim standard` was selected as distribution calculation methods.

### 2.3.3 Metabolism and Elimination

Two transport proteins were implemented into the model via Michaelis-Menten kinetics - OATP1B1 and MRP2.

* OATP1B1

The OATP1B1 expression profile is based on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2013](#5-references)), i.e not according to the default implementation in PK-Sim. Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

* MRP2

The MRP2 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for MRP2 was measured by liquid chromatography tandem mass spectroscopy ([Deo 2012](#5-references)), i.e not according to the default implementation in PK-Sim. Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

Additionally, glomerular filtration rate fraction was set to 1 as this describes the observed renal clearance rate in accordance to literature (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).


### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter                | 
| ------------------------------ | 
| `kcat` (OATP1B1)               | 
| `kcat` (MRP2)                   | 



 
