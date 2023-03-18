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

## Half Adder
```
ghdl -a adder.vhdl
ghdl -a adder_tb.vhdl
ghdl -e adder_tb
ghdl -r adder_tb --vcd=adder.vcd
gtkwave adder.vcd
```
