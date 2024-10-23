### 2.3.1 Absorption

The parameter value for  `Specific intestinal permeability`  was set to 0 to not include intestinal reabsorption. The solubility was obtained from DrugBank (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data))

The synthesis rate was modelled as a zero-order infusion over one year ([Mochizuki 2022](#5-references)). 

### 2.3.2 Distribution

Coproporphyrin-I is highly bound to plasma proteins (>99 %) (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)). A value of 0.66% was used in this PBPK model for `Fraction unbound (plasma, reference value)`. The major binding partner was set to albumin (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).

An important parameter influencing the resulting volume of distribution is lipophilicity. The reported logP value were 2.53 (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)) which was used in this model.

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim standard`.

### 2.3.3 Metabolism and Elimination

Two transport protein was implemented into the model via Michaelis-Menten kinetics 

* OATP1B1

The OATP1B1 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2013](#5-references)). Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

* BCRP

The BCRP expression profiles isbased on high-sensitive real-time RT-PCR ([Nishimura 2003](#5-references)). The reference concentration for OATP1B1 was measured by liquid chromatography tandem mass spectroscopy ([Prasad 2014](#5-references)). Transporter activity was described as saturable process following Michaelis-Menten kinetics, were the `Km` was taken from literature and the `kcat` was optimized based on clinical data (see [Section 2.3.4](#234-automated-parameter-identification)).

Additionally, renal clearance was set to 1 according to literature (see [Section 2.2.1](#221-in-vitro-and-physicochemical-data)).


### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter                | 
| ------------------------------ | 
| `kcat` (OATP1B1)               | 
| `kcat` (BCRP)                  | 



 