
# Logic Orchestration integrated with OpenROAD

This project is providing the integration between customized ABC with OpenROAD. Specifically, we implement a new logic optimization method **Orchestration** in ABC, where multiple logic optimization methods (rw, rs, rf) are orchestrated in the single traversal of the AIG. To evaluate the logic optimization in the end-to-end fashion, we integrate the algorithm with OpenROAD. 

### Note 1
This repo only provides the customized ABC and the integration part, where we omit the installation of OpenROAD. Thus, users are required to install the OpenROAD before evaluating this repo.

### How to link an external ABC implementation in OpenROAD-flow-scripts
#### 1. Change the makefile in Yosys
We can change the ABCREV to direct the compilation to the customized ABC in OpenROAD-flow-scripts/tools/yosys/Makefile (or ABCEXTERNAL for a new download link).

#### 2. Change the script for the design flow
In OpenROAD-flow-scripts/flow/scripts/synth.tcl, we can change the command for logic optimization with ABC and change the running script for logic optimization where we define the optimization operations.

The script is in OpenROAD-flow-scripts/flow/scripts.
