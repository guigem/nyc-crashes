# Data preprocessing - NYC Motor Vehicle Crashes

![Texte alternatif](https://media.cntraveler.com/photos/5a9d825ad363c34048b3639a/16:9/w_2560%2Cc_limit/GettyImages-640006562.jpg)

#### BeCode challenge: from 08/12/20 to 11/12/20

#### Contributors: Guillaume

## Aim of this project

The goal of this project is to clean a [dataset](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95 "Title"), which represents crashes that occured in New York City, in order to run machine learning algorihtms. This task requires a certain number of steps that will be exposed and explained below.
The end result should not contain any missing values, no dupplicates and data formats should be correct. Moreover, the dataset should be optimized in order to, on the one hand, be statistically correct and, on the other hand, be as informative as possible.

## Repository content

- The raw data as well as the cleaned data for 100,000 and 1,000,000 rows.
- Two jupyter notebooks for the 100,000 and the 1,000,000 rows datasets that contain the steps performed to reach the cleaned dataset mentionned above.
- Two profile reports created thanks to [pandas_profiling](https://pandas-profiling.github.io/pandas-profiling/docs/master/rtd/ "Title").

## Libraries used in Python

- [Pandas](https://pandas.pydata.org/ "Title")
- [Pandas_profiling](https://pandas-profiling.github.io/pandas-profiling/docs/master/rtd/ "Title")


## Steps 

### Handling missing values

The following graph shows the number of missing values of our initial dataset. In order to simplify our approach, we will only present the 100,000 rows dataset.

As one can notice, some of the columns are massively empty. We can cite *cross_street_name*, *off_street_name*, *contributing_factor_vehicle_3*, *contributing_factor_vehicle_4*, *contributing_factor_vehicle_5*, *vehicle_type_code_3*, *vehicle_type_code_4*, *vehicle_type_code_5*. 
Therefore, we decided to simply remove these columns as it becomes almost impossible to fill them with values without biaising our analysis.



