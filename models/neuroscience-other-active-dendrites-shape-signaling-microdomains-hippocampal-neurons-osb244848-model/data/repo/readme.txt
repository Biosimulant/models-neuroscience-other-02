The files in this directory incorporate calcium handling mechanisms involved in the Ca – Calmodulin – CaMKII – PP1 pathway in a conductance-based neuronal CA1 pyramidal model developed in Rathour and Narayanan, PNAS, 2014. The simulation environment is NEURON.  The model contains Na, KDR, KA, h, CaT and CaR currents, and employs GHK-based implementations of AMPA and NMDA receptors. Fig13.hoc helps recreate Fig 13 of the following paper:

Basak R, Narayanan R. Active dendrites regulate the spatiotemporal spread of signaling microdomains; Plos Comp Biol (in Press).

Running Fig13.hoc will create files that will contain .txt files storing the values of various species (Ca, Calmodulin, phosphorylated CaMKII etc.) as they evolve with time at various spatial locations, specifically the 100 µm length around the spine-containing synapse in the oblique containing the calcium handling mechanisms. The default number of spines in the oblique in the .hoc file is 1000. Example output was obtained by running the defaultgrad_Dependent() function. This shows the example data generated for the Calcium species for 100 ms of simulation time at the central location of the oblique and is provided in the Sample_output_Calcium.txt file in this directory. The calcium handling mechanisms were incorporated in the file modcamechs.mod, which is modified from Ashhad and Narayanan; Journal of physiology; 2013

Implemented by Reshma Basak and Rishikesh Narayanan. Contact reshmab at iisc.ac.in .

If you need more help running this model please see:
https://senselab.med.yale.edu/ModelDB/NEURON_DwnldGuide.cshtml


20181008 A correction from Reshma Basak for a shell volume scaling bug
in modcamechs.mod and an updated sample calcium .txt file. The bug
resulted in quantitative but not qualitative changes.

20220523 Updated MOD files to contain valid C++ and be compatible with
the upcoming versions 8.2 and 9.0 of NEURON.
