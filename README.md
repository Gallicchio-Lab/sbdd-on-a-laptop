# Structure-Based Drug Design on a Laptop: a Hands-On Workshop

A series of Jupyter notebooks and notes for a 3-day hands-on workshop held at Brooklyn College in January 2026.

## Learning Objectives

The goal of the workshop was to build familiarity with free or online computational modeling tools for structure-based drug design that are available to all on small computers, such as laptops. In addition to the Google Colab computational environment, we used molecular viewers and molecular editors (Mol*, Maestro Viewer).

Some of the things we learned about:

- The Google Colab computational environment.
- Elements of the Python programming language.
- The preparation of the structure of chemical compounds with RDKit. 
- The structure prediction tools for protein and protein-ligand complexes (Boltz-2).
- Structural refinement and binding energy scoring of protein-ligand complexes (MM/GBSA).
- Molecular dynamics of protein-ligand complexes (OpenMM).
- Binding free energy scoring of protein-ligand complexes with alchemical transfer (AToM-OpenMM).

## Case Study

We followed the paper [Identification of Potent Reverse Indazole Inhibitors for HPK1](https://doi.org/10.1021/acsmedchemlett.0c00672) by Elsie C. Yu and a team at Merck (Boston).

Each student was tasked with modeling a pair of related compounds to confirm the energetic and structural characteristics that informed the team of medicinal chemists at Merck. Their work was structure-based, but for the most part, it did not involve advanced molecular modeling.

## The Jupyter Notebooks

Navigate to the [notebooks](notebooks/) folder and open each notebook in sequence. They are numbered from 1 to 6.

1. [Prerequisites and Setup](notebooks/1_Prerequisites_and_Setup.ipynb), contains some course information and the steps to set up the Google Colab and other software.
2. [Paper Overview Compound SMILES](notebooks/2_Paper_Overview_Compound_SMILES.ipynb) goes through the steps to recover the ligands' information from CHEMBL and generate their 2D structures.
3. [Structure Prediction and Preparation](notebooks/3_Structure_Prediction_and_Preparation.ipynb) uses Boltz-2 to generate a structural model of the complex using the protein sequence and the SMILES of the compounds as inputs.
4. The fourth notebook, [Structure Refinement and Binding Energy Scoring](notebooks/4_Structure_Refinement_and_Binding_Energy_Scoring.ipynb), goes through the steps of energy-minimizing the Boltz-predicted structures and computing their binding energies in implicit solvent using OpenMM.
5. [Protein-Ligand MD Analysis](notebooks/5_protein_ligand_md_analysis.ipynb) performs MD of the complex and some structural analysis.
6. Finally, [Alchemical Relative Binding Free Energy](notebooks/6_Alchemical_Relative_Binding_Free_Energy.ipynb) introduces the calculation of the Relative Binding Free Energy of a pair of compounds using the Alchemical Transfer Method (ATM) and the [AToM-OpenMM](https://github.com/Gallicchio-Lab/AToM-OpenMM) software.

## Credits

Developers: Emilio Gallicchio and Joe Z. Wu. Additional credits in each notebook.

Instructor: Emilio Gallicchio

Teaching Assistant: Joe Z. Wu

Coordinators: Maria Contel and Ana Bartolome

Funding: the National Cancer Society

Hosting and Support: the Brooklyn College Cancer Center


