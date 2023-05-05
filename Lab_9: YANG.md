# Lab 9: YANG

## Install pyang and PlantUML:
```
$ sudo apt install libxml2-dev libxslt1-dev
$ sudo pip3 install -U lxml pyang
```
![1](https://user-images.githubusercontent.com/94701716/236365674-b454c19e-f550-46c3-9f76-e979f06402c8.png)
![2](https://user-images.githubusercontent.com/94701716/236366320-5ffb9446-1b66-4a80-8632-59567e9bd49f.png)
![5](https://user-images.githubusercontent.com/94701716/236369136-5832f9e6-8905-4723-af86-2c01ae6a2ab2.png)

## Copy ~/iot/lesson9/intrusiondetection.yang to ~/demo
```
$ mkdir demo
```
![3](https://user-images.githubusercontent.com/94701716/236367237-b81f5ebc-b29b-4b3c-976c-ac706c5a5759.png)

```
$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
```
![4](https://user-images.githubusercontent.com/94701716/236368958-0220a465-d70c-4619-98e7-50b5df5764e1.png)

```
$ cd ~/demo
```
![6](https://user-images.githubusercontent.com/94701716/236369388-624edb32-1133-44fd-bd76-def2c2e27f11.png)

## Run pyang to generate intrusiondetection.yin and intrusiondetection.uml
```
$ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
```


```
$ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
```


## Run PlantUML to generate intrusiondetection.png
```
$ py -m plantuml intrusiondetection.uml
```
