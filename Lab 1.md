# Lab 1: GHDL and GTKWave
For this lab, I will install and use GHDL and GTKWave to run an example of a half adder and 4-to-1 multiplexer. However, due to software issues, I was not able to use GTKwave, so I will use Fliplot instead. 

Download guide: [Fliplot](https://github.com/raczben/fliplot) and [GHDL](https://github.com/ghdl/ghdl/releases)

---
## Half-adder
This is my final product after running the half-adder. I used the following commands to complete the task:
- `ghdl -a ha.vhdl`
- `ghdl -a ha_tb.vhdl`
- `ghdl -e ha_tb`
- `ghdl -r ha_tb --vcd=ha.vcd`
- `ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test`
- `gtkwave ha.vcd`

---
## 4-to-1 multiplexer  
This is my final product after running 4-to-1 multiplexer. I used the following commands to complete the task:
- `ghdl -a mux.vhdl`
- `ghdl -a mux_tb.vhdl`
- `ghdl -e mux_tb`
- `ghdl -r mux_tb --vcd=mux.vcd`
- `gtkwave mux.vcd`
