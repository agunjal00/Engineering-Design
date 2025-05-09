
# Lab 1

For this lab I went to the DSD repository and clicked on the GHDL folder. After installing GHDL and GTKWave, I ran the following commands on terminal.



## Half Adder


```bash
$ ghdl -a ha.vhdl
$ ghdl -a ha_tb.vhdl
$ ghdl -e ha_tb
$ ghdl -r ha_tb --vcd=ha.vcd
ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test
$ gtkwave ha.vcd
```

    
![App Screenshot](https://github.com/user-attachments/assets/a6cc42b1-af3e-4418-94b5-11cd4865e489)


## 4to1 Multiplexer

```bash
$ ghdl -a mux.vhdl
$ ghdl -a mux_tb.vhdl
$ ghdl -e mux_tb
$ ghdl -r mux_tb --vcd=mux.vcd
$ gtkwave mux.vcd
```

    
![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)
