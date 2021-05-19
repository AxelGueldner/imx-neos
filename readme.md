# imx-neos

Command line interface to assist development of imx neos projects

## Installing

Install the cli global to gain access to it accros all dummy projects:
```
$ npm install imx-neos -g
```

## How to use

Currently there are two operations available:

### addComp - this will add a brand new component to your project
use this command pattern:
```
imx-neos addComp <project> <target>
```
the target parameter consists of the type and the name of the new to create component. Type and name are separated using an **//**

an example could look like this
```
imx-neos addComp kampenwand a/button
```
this will create a new atom named button

There is the short alias aC available for this operation
```
imx-neos aC <target>
```

### copyComp - create a copy of an existing component while renaming it
use this command pattern:
```
imx-neos copyComp <project> <source> <target>
```
Both, the source and the target parameter consist of a type and a name which have to be separated using an **//**
The source parameter will be the existing component you whish to copy.
The target parameter will be the new component that will be created.

an example could look like this
```
imx-neos copyComp kampenwand a/button m/newButton
```
this will create a new molecule named newButton using a copy of the existing atom named button

There is the short alias cC available for this operation
```
imx-neos cC <project> <source> <target>
```

## Component types

The atomicDummy framework knows 4 TPL Component Types that you want to address:
* Atoms - use **a**
* Molecules - use **m**
* Nucleus - use **n**
* Organisms - use **o**


## Authors

* **Axel Güldner@infomax**