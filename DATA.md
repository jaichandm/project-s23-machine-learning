# Data info:
columns
Company: company/manufacturer name
TypeName: laptop type
Inches: size of screen
ScreenResolution: screen resolution
Cpu: laptop cpu name
Ram: size of ram in GB
Memory: memory types
Gpu: gpu name
OpSys: operating system


### Features

1. Features to consider for predicting the laptop price are Company,TypeName,Ram,Weight,Price,Touchscreen,Ips,ppi,Cpu brand,HDD,SSD,Gpu brand,os.

2. I choose Ram, SSD, ppi(pixel count), CPU brand to improve accuracy of model.

3. I have cleaned the data by removing unnecessary data like umpires information which would not be helpful in my predictions. Below are some steps I performed on raw data:
* The "Ram" and "Weight" columns are cleaned by removing the units and converting them to numeric types.
* The "Touchscreen" and "Ips" columns are created based on the presence of certain keywords in the "ScreenResolution" column.
* The "X_res" and "Y_res" columns are extracted from the "ScreenResolution" column and cleaned by removing commas and converting them to numeric types.
* The "ppi" column is created by calculating the pixel density of the screen based on the "X_res", "Y_res", and "Inches" columns.
* The "Cpu brand" column is created based on the processor brand in the "Cpu" column.
* The "Memory" column is cleaned by removing the units and converting them to numeric types.
* The "Layer1HDD", "Layer1SSD", "Layer1Hybrid", and "Layer1Flash_Storage" columns are created based on the presence of certain keywords in the "Memory" column.
* The "Layer2HDD", "Layer2SSD", and "Layer2Hybrid" columns are created based on the presence of certain keywords in the second layer of the "Memory" column.

[Intial Expolaration](initial_exploration.ipynb)