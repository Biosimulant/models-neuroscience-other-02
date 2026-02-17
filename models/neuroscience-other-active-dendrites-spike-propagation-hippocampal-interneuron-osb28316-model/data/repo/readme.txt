README for the models associated with the paper:

	Saraga F, Wu CP, Zhang L, Skinner FK. Active Dendrites and Spike Propagation 
	in Multi-compartment Models of Oriens-Lacunosum/Moleculare Hippocampal Interneurons.
	J Physiol. 2003 Aug 15

Summary:

It is well known that interneurons are heterogeneous in their morphologies, biophysical 
properties, pharmacological sensitivities and electrophysiological responses, but it is 
unknown how best to understand this diversity. Given their critical roles in shaping brain 
output, it is important to try to understand the functionality of their computational 
characteristics. To do this, we focus on specific interneuron subtypes. In particular, it 
has recently been shown that long-term potentiation is induced specifically on 
oriens-lacunosum/moleculare (O-LM) interneurons in hippocampus CA1 and that the same cells 
contain the highest density of dendritic sodium and potassium conductances measured to date. 
We create multi-compartment models of an O-LM hippocampal interneuron using passive 
properties, channel kinetics, densities and distributions specific to this cell type, and 
explore its signaling characteristics. We find that spike initiation depends on both 
location and amount of input, as well as the intrinsic properties of the interneuron. Distal
 synaptic input always produces strong back-propagating spikes whereas proximal input could 
produce both forward and back-propagating spikes depending on the input strength. We 
speculate that the highly active dendrites of these interneurons endow them with a 
specialized function within the hippocampal circuitry by allowing them to regulate direct 
and indirect signaling pathways within the hippocampus.

------------------------------------------------
This model can be auto-launched from modeldb or run by starting the mosinit.hoc with:
nrngui mosinit.hoc
or double clicking on the mosinit.hoc file 
after the mod files have been compiled (nrnivmodl compiles in unix, mknrndll in mswin, mac)

Select a figure by clicking on a figure name.

Fernanda.Saraga@UToronto.ca

20150416 Note from the ModelDB administrator: A bug noted by Mohamed
Sherif and fix provided by Ted Carnevale updates the IA.mod file so
that the a,b states change.

20160830 Note from the ModelDB administrator: A bug noted by Andras
Ecker and communicated by Marianne Bezaire was that IAprox.mod
neglected to call the rates function.  The previous fix (20150416)
required slight changes (see below) in the IClamp current (adjustable
in the Point Process Manager window which becomes available when you
run the simulation with mosinit.hoc) for some of the generated figures
to be similar to those in the paper: 1) for 20150416 version in the 8B
Long case the current needed to be increased from 0.2 to 0.27 however
with this subsequent version (20160830) this is no longer
necessary. For other cases 2) the 8 B Short current needs to be
increased from 13 to 14 and 3) the 9A Case 2 current needs to be
changed from -.05 to -0.04 for the generated graphs to be similar to
the paper figures in both this updated version and in the 20150416
version.
