# APolQ
Supporting Information for the publication "A Simple Method for Including Polarization Effects in Solvation Free Energy Calculations When Using  Fixed--Charge Force Fields: Alchemically Polarized Charges." by Braden D. Kelly and William R. Smith, 2020 

Currently available on chemRxiv https://doi.org/10.26434/chemrxiv.11522133.v1 

This Repository has the topology files for all partial charge sets on an all 45 molecules studied in the above mentioned manuscript.

For each molecule there should be, frankly, alot of topology files. For each molecule there should be a topology for the polarized charge set(one per water model) and the vaccuum set as well. There should also be the vacuum derived charge set. This should also be done ffor both MP2/cc-pVTZ and MP2/aug-cc-pVTZ. This is further done for both MBIS and RESP. Although, RESP is only 1 water model. Lastly, there should be topologies for the AM1-BCC charge sets. All GAFF parameters are version 2.11.

Due to the vast number of topology files this is the format:

NAME_CM_QM_BASIS_PCM_GMX_averaged.top

NAME = name of the solute\
CM = charge method i.e., mbis, resp bcc\
QM = QM theory, should only be MP2\
BASIS = basis set used, should be cc-pVTZ or aug-cc-pVTZ\
PCM = continuum or vacuum i.e., True means continuum was used, false mean vacuum calculation was done\
averaged = averaged - it means the MBIS partial charges had their charges averaged out just like RESP and AM1-BCC do
