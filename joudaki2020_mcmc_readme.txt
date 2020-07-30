We provide MCMC chains in CosmoMC format (.txt, .paramnames, .ranges files)

These are the central chains for the analysis of KV450 + DESY1 in Joudaki et al. (2020). 

i) "kv450" refers to KiDS+VIKING-450 (KV450).

ii) "desy1_orignz" refers to Dark Energy Survey Year 1 (DES-Y1) with KiDS analysis setup and 
original redshift distributions. 

iii) "desy1" refers to DES-Y1 with KiDS analysis setup and spectroscopic calibration of the 
redshift distributions. 

iv) "kv450desy1" refers to the combined analysis of KV450 and DES-Y1 considering a KiDS 
analysis setup and spectroscopic calibration of the redshift distributions.

Note that the chains contain the pre-burn phase. In order to remove the burn-in phase of 
the MCMC, the first 30% of the lines should not be considered. The chains are provided in 
the "_N.txt" ascii files, with N = 1..8. For {KV450, DES-Y1, KV450 + DES-Y1}, they 
respectively contain a total of {61, 62, 72} primary and derived parameters for the MCMC 
samples [along with ln(likelihood x prior) and χ2 values]. They are compatible with CosmoMC 
and its plotting utility, GetDist. The format of each line in these files is as follows:

Column 1: weight of the point

Column 2: -ln(likelihood x prior)

Columns 3 and beyond: a list of primary and derived parameters as specified in 
the ".paramnames" files and the prior ranges are given in the ".ranges" files.

Note that it is important to propagate the weight of each point in the calculation of 
posterior probability distributions!
