# Lab 1: GHDL and GTKWave

I downloaded the GHDL and GTKWave .zip files shown below.

![zip files](https://user-images.githubusercontent.com/94701716/226140849-16927b29-d542-49fb-9fb6-91a39d257f4c.png)

After extracting both and setting the correct Path environment variables, we can test the installation using the Hello, World example:

## Hello, World
```
ghdl -h
ghdl -v
ghdl -a hello.vhdl
ghdl -e hello_world
ghdl -r hello_world
```

<!-- ![image](https://user-images.githubusercontent.com/94701716/226142468-e88fbcc4-070d-4367-92e7-46ef358b476e.png)
![image](https://user-images.githubusercontent.com/94701716/226142494-379a887a-14c3-488c-9bf7-06843fa2ad4f.png)
![image](https://user-images.githubusercontent.com/94701716/226142525-b5874d55-2e6d-437d-b7d7-6942c2c90b10.png)
![image](https://user-images.githubusercontent.com/94701716/226142573-899b6626-155a-4e8d-9e0b-be7d313fb106.png)

![image](https://user-images.githubusercontent.com/94701716/226142582-dcc2e93c-ae69-419c-8e50-eb66753bc80b.png) -->
![image](https://user-images.githubusercontent.com/94701716/226142613-aae8290e-29bc-4241-aa8f-b51a70cbf501.png)

## Half Adder
```
ghdl -a ha.vhdl
ghdl -a ha_tb.vhdl
ghdl -e ha_tb
ghdl -r ha_tb --vcd=ha.vcd
gtkwave ha.vcd
```
![image](https://user-images.githubusercontent.com/94701716/226143183-3883db2f-ca79-4191-a38c-ddf860c413a8.png)

## Full Adder
```
ghdl -a adder.vhdl
ghdl -a adder_tb.vhdl
ghdl -e adder_tb
ghdl -r adder_tb --vcd=adder.vcd
gtkwave adder.vcd
```
![image](https://user-images.githubusercontent.com/94701716/226143344-9a9453a0-a9cb-4789-99c2-ab6589821335.png)

## D Flip-flop
```
ghdl -a dff.vhdl
ghdl -a dff_tb.vhdl
ghdl -e dff_tb
ghdl -r dff_tb --vcd=dff.vcd
gtkwave dff.vcd
```
![image](https://user-images.githubusercontent.com/94701716/226143651-4d2f1855-1042-489d-a6b5-c89cd21382ec.png)

## 4-to-1 Multiplexer
```
ghdl -a mux.vhdl
ghdl -a mux_tb.vhdl
ghdl -e mux_tb
ghdl -r mux_tb --vcd=mux.vcd
gtkwave mux.vcd
```
![image](https://user-images.githubusercontent.com/94701716/226143761-86d1fb75-6759-46b6-963f-8390541ab74a.png)
