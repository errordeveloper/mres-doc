# Wishbone

  It may be appropriate to implement the DSP susb-system
  on the WB bus, more study is required to approve this.

  Considering a set of unit generators implemented on
  an FPGA and route via WB is not the most optimal
  approach, since the logic resources required for
  this are limited. Suppose a 100 of oscillators were
  to be implemneted with DSP slices + WB interconnect
  for each unit generator, then there will be a very
  large number of cells used for just the interconnect.
  This may provide great flexibility, however does not
  make the best use of the resources available.
  It may be a better idea to design a simpler bus for
  DSP interconnect.

## WB Units

  The fallowing units should be designed for practice:

   - dummy DAC
   - wevform generator
   - signal multiplier and adder
   - delay unit

 Most of this should be done in synthesiseble Verilog
 and use only FP math.
