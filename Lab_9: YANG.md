# Lab 9: YANG

## Install pyang and PlantUML:
```
$ pip install pyang plantuml
```


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
