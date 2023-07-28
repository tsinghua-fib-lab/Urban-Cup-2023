# Carbon 
- **Carbon/odiac_carbon_mainland_us.npy**
  - Record the 1kmx1km monthly CO2 emission statistics from the ODIAC database (https://odiac.org/data-product.html) in a NPY file. ODIAC is an open-data inventory that pioneered the combined use of nighttime lights data and point source data to achieve its global 1x1km resolution emission field.
  - You can use following codes to load the data:​
```
import numpy as np
odiac_values=np.load(‘odiac_carbon_mainland_us.npy’, allow_pickle=True).item()
```
where odiac_values is a dict form of the monthly odiac values of the 1km*1km points in Mainland USA.
Take an example, to request the odiac values of the March of 2021, just type odiac_values['21'][3].
The key is the location tuple for the point (latitude, longitude), and the value is the monthly carbon emission in units of Megatonne.​

  **Data Preview:**  
