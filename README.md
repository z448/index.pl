##jsonweb
- backup/restore html and css files into index.json 

##SYNOPSIS

- push lines of html/css files in array and encode it into json file which can be restored back into single html file

##INSTALLATION
- clone repository

```bash
git clone https://github.com/z448/jsonweb
cd jsonweb
# install JSON dependency using carton
carton install
```

- set enviroment

```bash
. ./env.sh
```

##GIF

![jsonweb](https://raw.githubusercontent.com/z448/jsonweb/master/jsonweb.gif)

##EXAMPLES

- backup my.html index.html and style.css

```bash
jsonweb -j my.html index.html style.css

# makes index.json containing objects my, index and style which contains lines of html file. 
```

- restore index.json into single index.html
```bash
jsonweb -h
# or specify name of your .json
jsonweb -h my.json
```




