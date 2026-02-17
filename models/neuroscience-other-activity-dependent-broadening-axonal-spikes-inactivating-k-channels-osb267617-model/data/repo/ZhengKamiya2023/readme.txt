This is the readme for the simulation showing the properties of Na, K channels (hhmfb.mod replacing K conductance with KIn.nod, inactivating K model; hhmfb.mod, non-inactivating K model) and Ca channels of P/Q, N, R type (mfbpqca.mod, mfbnca.mod, mfbrca.mod) at hippocampal mossy fiber terminals.   
We also tested single shocks, 10, 20, and 50Hz train stimuli 50 times for showing use-dependent action potential broadening, accumulation of K channel inactivation, and enhancement of Ca entry during AP train.
For 20 Hz 50 stimulus, K conductance was changed by 0.5, 1, and 10 times to vary the action potential duration to see if it changes the rate of K channel inactivation during the train stimulus.
The responses at the en passant boutons and the effect of KV7 M-type K channels (kmb.mod) were also tested.

To run the simulations, follow these steps:
Compile the mod files using nrnivmodl under Mac OS X and Linux, or mknrndll under Windows.
Run mosinit.hoc in NEURON.
Click the buttons in the panel "Demo" and click "Init & Run" in the "RunControl" panel to run simulations.

Questions about this model should be directed to kamiya@med.hokudai.ac.jp.



