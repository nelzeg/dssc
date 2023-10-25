# Digital Standard Cell Characterizer (DSCC)  

### ⚠️ Important:
1. **The tool only characterizes combinational cells for nodes greater that or equal to 130nm because it is based on the Non linear delay model (NLDM) for timing characterization. The support for sequential cells will be added in the future.**  
2. **I still have to refactor the code, task I will be doing while I study my courses on Software Development on Coursera.**  
<br>

## Demo
### 📌 Instructions:
- **The layout file must have the extension `.mag` associated with [Magic Layout Tool](http://opencircuitdesign.com/magic/).**
- **If you installed the PDK in the default path `/usr/local`, it is not necessary to use the argument `--sky130-root`.**
- **The output loads are in picofarads [pF] and the transition times in nanoseconds [ns].**

~~~ bash
python3 dscc.py thesis_aoi211.mag \\
--sky130-root="/home/nelson/cad" \\
--output-loads="0.05, 0.1" \\
--slew-rates="0.1, 0.2"
~~~

<div align="center"><video src="https://github.com/ledzeg/dscc/assets/107968926/7c6d5b47-cb7b-424a-942b-abe0cdf93e18"></video></div>

## Slides
**In these slides you will find an explanation on how the tool was developed, that is, the algorithms to characterize the cells and to identify the logical function of them. This tool was developed to be used in the main project of [Open-Source Standard Cell Design Methodology](https://github.com/ledzeg/stdcell-methodology)**
<br>
<div align="center"><b >👇🏼 Click on the image to watch the slides</b></div>
<br>
<div align="center"><a href="https://docs.google.com/presentation/d/e/2PACX-1vSiSyyyWhbehkQ2xNrCZK2VOh_s4KmKSZHU7BYJNZw7zeUBU8BMkgzOVHIq0tX81F9O7TQF6yfjhio4/pub?start=false&loop=false&delayms=60000"><img src="slides_cover.png" target="_blank" frameborder="0" width="680" height="400" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></a></div>


