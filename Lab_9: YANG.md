# Lab 9: YANG

## Install pyang and PlantUML:
```
$ sudo apt install libxml2-dev libxslt1-dev
$ sudo pip3 install -U lxml pyang
```
![1](https://user-images.githubusercontent.com/94701716/236365674-b454c19e-f550-46c3-9f76-e979f06402c8.png)



## Copy ~/iot/lesson9/intrusiondetection.yang to ~/demo
```
$ mkdir demo
```


```
$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
```


```
$ cd ~/demo
```


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
