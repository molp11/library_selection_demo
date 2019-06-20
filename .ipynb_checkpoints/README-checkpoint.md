# library_selection_demo

## Click here to run the code yourself and view additional libraries in the 'data' directory [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/molp11/library_selection_demo/master)

# 2D descriptors:
## [a common school of thought](http://practicalfragments.blogspot.com/2011/11/pushing-rule-of-3.html) holds that fragment libraries should contain molecules with the following attributes:
- Molecular Weight $\lt$ 300 g/mol
- ClogP $\le$ 3
- Number of hydrogen bond donors $\le$ 3
- Number of hydrogen bond acceptors $\le$ 3
- Number of rotatable bonds $\le$ 3
- Polar surface area $\le$ 60 Å


    HBox(children=(IntProgress(value=0, description='calculating...', max=500, style=ProgressStyle(description_wid…


    
    


![png](page_files/page_4_2.png)


# [3-dimensionality (vs. flat structures) as a strategy to increase library diversity](https://blogs.sciencemag.org/pipeline/archives/2013/08/08/the_3d_fragment_consortium)
## Plots quantifying molecule 3D character depicted below
- [2-dimensional normalized ratios of principle moments of inertia](https://pubs.acs.org/doi/full/10.1021/ci025599w)
- [Plane of best fit (PBF) score versus sum of NPRs](https://pubs.acs.org/doi/pdfplus/10.1021/ci300293f)


    HBox(children=(IntProgress(value=0, description='calculating...', max=1200, style=ProgressStyle(description_wi…



![png](page_files/page_7_1.png)


# [Fingerprinting and molecular similarity](https://www.rdkit.org/docs/GettingStartedInPython.html#fingerprinting-and-molecular-similarity)
## [click here for a more detailed explanation of the theory behind fingerprints](https://www.daylight.com/dayhtml/doc/theory/theory.finger.html)
- in general, molecular substructures are converted into bitmaps that can be compared mathematically for similarity

## Comparing nearest-neighbor similarity between two libraries
- Example use case: would combining two different compound libraries lead to substantial redundancy? 
- In the example shown below, each compound fingerprint in one library is compared to each compound fingerprint in another and the highest pair-wise similarity score is recorded for each molecule
- Here, scoring ranges from 0.0 (no similarity) to 1.0 (structurally identical)
- E.g. if a compound is associated with a score of 1.0, this means the same compound exists in both libraries


    HBox(children=(IntProgress(value=0, description='calculating 1...', max=500, style=ProgressStyle(description_w…



    HBox(children=(IntProgress(value=0, description='calculating 2...', max=1500, style=ProgressStyle(description_…



![png](page_files/page_10_2.png)


# 2D depictions of molecular fingerprints:
- The dimensionality of fingerprint bitmaps (here we used 2048-bit [Morgan fingerprints](https://www.rdkit.org/docs/GettingStartedInPython.html#morgan-fingerprints-circular-fingerprints)) can be reduced using statistical techniques like [Principle component analysis (PCA)](https://en.wikipedia.org/wiki/Principal_component_analysis) to allow for visualization and comparison of library diversity.
- Here we fit a [pca model](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.IncrementalPCA.html) on a set of \~348 million fragments (MW $\le$ 350 g/mol) downloaded from the [ZINC database](http://zinc15.docking.org/tranches/home/#)
- The model (loaded here as 'ipca.pkl') is then used to project 2048 bit [Morgan fingerprints](https://www.rdkit.org/docs/GettingStartedInPython.html#morgan-fingerprints-circular-fingerprints) calculated from compound libraries onto two dimensions for visual comparison of diversity.


![png](page_files/page_13_0.png)

