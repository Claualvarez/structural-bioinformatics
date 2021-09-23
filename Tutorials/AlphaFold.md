# Structure prediction using Colab notebooks

For this tutorial we will use a [Colab notebook](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) that provides a basic AlphaFold functionality. To use advances features follow this [link](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/AlphaFold2_advanced.ipynb).
The Colab notebook that we will use was created by Sergey Ovchinnikov, Milot Mirdita and Martin Steinegger.

## Before we start ...
**1. What is AlphaFold**
> AlphaFold is an artificial intelligence (AI) program developed by Google's DeepMind which performs predictions of protein structure.
> 
> [Quote from Wikipedia](https://en.wikipedia.org/wiki/AlphaFold)

**2. What is a Colab notebook?** 
> *“Colab” is a product from Google Research. \
> Colab allows anybody to write and execute arbitrary python code through the browser [...] More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs.* 
>
> [Quote from Colab FAQ](https://research.google.com/colaboratory/faq.html)

## Getting started
For this tutorial you will need an amino acid sequence. (Just the sequence, without a sequence header). \
     Here is an example:  \
     `KGKEGKVLKVDPKKGRVVVEGVNGEVEVPIHPSHVRKGDTVKVIAGNKGKEGKVLKVDPKK`
     
Open the following [link](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) in a new tab.

![AlphaFoldColab](https://github.com/Claualvarez/structural-bioinformatics/blob/main/Tutorials/Figures/AlphaFoldColab1.png)

To run a code in Colab you will need to sign in to a google account. \
If you  have a Google account, click on the Sign in button on the upper sight corner of the screen.

### Settings 
**query_sequence:**  Copy and paste your sequence for this exercise here. \
**jobname:** It is highly recommended to use a short and descriptive jobname. 
**msa_model:** The options here allow you to select the database to construct an input Multiple Sequence Alignment. \
    - If your sequence is from a natural protein, use `UniRef+Envirnmental`. \
    - If your sequence is a de novo engineered sequence, use the `single sequence` option.
**num_models:** For this exercise, we will calculate only one model. 
**use amber:** This will allow you to refine the peptide bond geeometry with the AMBER force field.
**use_templates:** select this option if you expect your protein to have homologs with a solved structure in the PDB.

![Settings](https://github.com/Claualvarez/structural-bioinformatics/blob/main/Tutorials/Figures/AlphaFoldColabSettings.png)

