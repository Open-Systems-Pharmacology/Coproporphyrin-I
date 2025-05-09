# Coproporphyrin-I-Model
Whole-body PBPK model of the endogenous compound Coproporphyrin-I.

<img src="https://upload.wikimedia.org/wikipedia/commons/8/85/Coproporphyrinogen_I.svg" alt="File:Coproporphyrinogen_I.svg" style="zoom:50%;" />





This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation-plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found [here](../../releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found [here](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**



This Coproporphyrin-I model is intended to be used as a victim endogenous marker in OATP1B1-mediated drug-drug interactions (DDI).

This whole-body PBPK model of Coproporphyrin-I has been developed using published pharmacokinetic clinical data by Mori 2020 [[1](#references)], Takehara 2018 [[2](#references)], Lai 2016 [[3](#references)] and Zhang 2020 [[4](#references)]. 
The model has then been evaluated by simulating clinical studies and comparing with respective observed data. 

The presented model includes the following features:

- transport by OATP1B1/B3,
- transport by MRP2
- renal clearance by glomerular filtration,
- intracellular liver synthesis modeled as a zero-order infusion.


## Code of conduct

Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution

We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License

The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References

[1] [D Mori, E Kimoto, B Rago, Y Kondo, A King‐Ahmad, R Ramanathan, LS Wood, JG Johnson, VH Le, M Vourvahis, A David Rodrigues. Dose‐dependent inhibition of OATP1B by rifampicin in healthy volunteers: comprehensive evaluation of candidate biomarkers and OATP1B probe drugs. Clinical Pharmacology & Therapeutics, Apr;107(4):1004-13, 2020.](https://pubmed.ncbi.nlm.nih.gov/31628668/)

[2] [I Takehara, T Yoshikado, K Ishigame, D Mori, KI Furihata, N Watanabe, O Ando, K Maeda, Y Sugiyama, H Kusuhara. Comparative study of the dose-dependence of OATP1B inhibition by rifampicin using probe drugs and endogenous substrates in healthy volunteers. Pharmaceutical research, Jul;35:1-3, 2018.](https://pubmed.ncbi.nlm.nih.gov/29748935/)

[3]  [Lai Y, Mandlekar S, Shen H, Holenarsipur VK, Langish R, Rajanna P, Murugesan S, Gaud N, Selvam S, Date O, Cheng Y.  Coproporphyrins in plasma and urine can be appropriate clinical biomarkers to recapitulate drug-drug interactions mediated by organic anion transporting polypeptide inhibition. Journal of Pharmacology and Experimental Therapeutics, Sep 1;358(3):397-404, 2016.](https://pubmed.ncbi.nlm.nih.gov/27317801/)

[4] [Zhang Y, Holenarsipur VK, Kandoussi H, Zeng J, Mariappan TT, Sinz M, Shen H. Detection of Weak Organic Anion-Transporting Polypeptide 1B Inhibition by Probenecid with Plasma-Based Coproporphyrin in Humans. Drug Metab Dispos. 2020 Oct;48(10):841-848.](https://pubmed.ncbi.nlm.nih.gov/32723847/)




