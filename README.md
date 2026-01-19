The project is being converted to SystemVerilog, this is due to its compatability with input arrays. 
This is because FPGAs do not allow inouts on internal modules, forcing data/address busses to be defined as multiplexers where the select is determined by the relevant control signals, as each bus has a different number of inputs, they required individual modules to define them.
With array inputs, only a singular module is needed and have the number of inputs defined using parameters, simplifying the code.
