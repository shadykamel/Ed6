# Lab 9: YANG

## Install pyang and PlantUML:
```
$ pip install pyang plantuml
```
![image](https://user-images.githubusercontent.com/94701716/235489513-e50f8ae5-7cb0-4d2a-bb88-9d762b73d681.png)

## Copy ~/iot/lesson9/intrusiondetection.yang to ~/demo
```
$ mkdir demo
```
![image](https://user-images.githubusercontent.com/94701716/235511256-983578e3-069a-4122-ba01-f4945a4861a2.png)

```
$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
```
![image](https://user-images.githubusercontent.com/94701716/235516519-eb743568-719b-4d8b-b84a-19afc3c3517d.png)
![image](https://user-images.githubusercontent.com/94701716/235516565-f34adeaf-e20d-4e4a-b9c0-32d7df438f84.png)

```
$ cd ~/demo
```
![image](https://user-images.githubusercontent.com/94701716/235516738-18cb48a0-eba9-4fc6-b5c7-81ef405c22ce.png)

## Run pyang to generate intrusiondetection.yin and intrusiondetection.uml
```
$ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
```

```
$ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
```

## Run PlantUML to generate intrusiondetection.png
```
$ python3 -m plantuml intrusiondetection.uml
```
