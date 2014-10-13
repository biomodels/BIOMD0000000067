

# A Synthetic Gene-Metabolic Oscillator

**Reference:** [ _Fung et al; Nature (2005) 435:118-122_ ](http://www.nature.com/nature/journal/v435/n7038/abs/nature03508.html)   
Name of kinetic law | Reaction  
---|---  
Glycolytic flux, V_gly: | nil -> AcCoA;  
Flux to TCA cycle/ETOH, V_TCA: | AcCoA -> TCA/EtOH;  
HOAc ex/import,reversible, V_out: | HOAc -> HOAc_E  
V_Pta: | AcCoA + Pi -> AcP + CoA  
reversible, V_Ack: | AcP + ADP -> OAc + ATP  
V_Acs: | OAC + ATP -> AcCoA +PPi  
Acetic acid-base equillibrium, reversible, V_Ace: | OAC + H -> HOAc  
Expression of LacI, R_LacI: | nil -> LacI  
Expression of Acs, R_Acs: | nil -> Acs  
Expression of Pta, R_Pta: | nil -> Pta  
LacI degradation, R_dLacI: | LacI -> nil  
Acs degradation, R_dAcs: | Acs -> nil  
Pta degradation, R_dPta: | Pta -> nil  
  
For this model the differential equation for V_Ace was changed from:  
C*(AcP*H-K_eq*OAC) with C = 100 in the supplemental material  
to C*(OAc*H-K_eq*HOAc) with C = 100, as in [ _Bulter et. al;
PNAS(2004),101,2299-2304_
](http://www.pnas.org/cgi/content/abstract/101/8/2299) , and a value for K_eq
of 5*10^-4 after communication with the authors.

translated to SBML by:  
Lukas Endler(luen at tbi.univie.ac.at), Christoph Flamm (xtof at
tbi.univie.ac.at)

_Biomodels Curation_ The model reproduces 3a of the paper for glycolytic flux
Vgly = 0.5. The authors have agreed that the values on Y-axis are marked wrong
and hence there is a discrepancy between model simulation results and the
figure. Also, note that the values of concentration and time are in
dimensionless units. The model was successfully tested on MathSBML and Jarnac.

