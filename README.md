# cos-dev-cheatsheet

# import and compile the any COS project from repo
1. Download the repo. 
2. Run in standard termninal:
```
do $System.OBJ.ImportDir("c:\path\to\project","*.xml;*.cls;*.mac;*.int;*.inc;*.dfi","ck",,1)
```
# compile classes 

`do $System.OBJ.Compile("Package*")`

# export classes from Package to one file in InterSystems/mgr/namespace
```
do $System.OBJ.Export("Package.*.CLS","release.xml")
```

# Delete all instances in class
`w ##class(HR.Person).%DeleteExtent()`

# Build Cube
`$System.DeepSee.BuildCube("Cube")`

