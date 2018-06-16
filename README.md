#############################################################################################
                                 
                                                   AQNet Dataset

                    State Key Laboratory of Advanced Optical Communication System and Networks, Peking University
                    
#############################################################################################

# Introduction
The dataset contains both indoor and outdoor fine-grained PM<sub>2.5</sub> data monitored by low-cost wireless sensor network 
in Peking University and Xidian University. <br>
Data in Beijing were collected from March 1st, 2018 to May 15th, 2018. <br>
Data in Xian were collected from March 10th, 2018 to June 9th, 2018.<br>
Some bad data were eliminated when the data set was generated.
# Annotations
The dataset contains TWO PARTS:<br>
## file 'basic_inf.json'
Introduce the information of every sensor. <br><br>
`id`:Each sensor has an ID number ranging from 1 to 160.<br><br>
`longtitude` & `latitude`：The coordinates in the BD09 coordinate system adopted by Baidu Map.<br><br>
`location`:The place where the sensor is arranged, usually in Chinese.<br><br>
`outside`: A boolean variable. `'1'` refers to `outdoor` and `'0'` refers to `indoor`.<br><br>
`city`:Beijing(北京) or Xian(西安).<br>

## file 'beijing_outside & beijing_inside & xian_outside & xian_inside  .json'
The outdoor/indoor PM<sub>2.5</sub> and PM<sub>10</sub> data in Beijing/Xian.<br><br>
`id`:The sensor number. Its information can be further gotten in file`basic_inf.json`.<br><br>
`time`:Sampling time. The sampling frequency is every half an hour.<br><br>
`pm25` & `pm10`:PM<sub>2.5</sub> and PM<sub>10</sub> monitored by corresponding sensor at given time. The unit is μg/m<sup>3</sup>.<br>

## Questions?
Contact Zixuan Bai at zixuan.bai@pku.edu.cn

June 2018
