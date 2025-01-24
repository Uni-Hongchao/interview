
+ Drivers
 
 | Column Name | Type |
 | --------- | ------- |
 | driver_id | int |
 | driver_name | varchar |


+ Citys
 
 | Column Name | Type |
 | --------- | ------- |
 | city_id | int |
 | city_name | varchar |
 | time_zone | varchar |


+ Orders

 | Column Name | Type |
 | --------- | ------- |
 | order_id | bigint |
 | city_id | int |
 | address | varchar |
 | zipcode | varchar |
 | delivered_time | timestamp |
 | driver_id | int |


+ Drivers

 | driver_id | driver_name | 
 | --------- | ------- |
 | 10001 | Jim |
 | 10012 | Mike |
 | 10018 | Henry |
 | 10120 | Alex |

+ Citys

 | city_id | city_name | time_zone |
 | ----- | ----- | ----- |
 | 10 | Chicago | America/Chicago |
 | 11 | Phoenix | America/New_York | 

+ Orders

 | order_id | city_id | address | zipcode | delivered_time | driver_id |
 | ----- | ----- | ----- | ----- | ----- | ----- |
 | 20240830120910100001 | 10 | *** | 60007 | 2024-09-02 18:30:28.000 | 10001 |
 | 20240829141008224800 | 10 | *** | 60018 | 2024-09-02 16:23:34.010 | 10012 |
 | 20240831080803487005 | 10 | *** | 60604 | 2024-09-03 01:45:56.566 | 10012 |
 | 20240901101004746483 | 10 | *** | 60610 | 2024-09-03 00:28:21.824 | 10018 |
 | 20240901101004746483 | 11 | *** | 80003 | 2024-12-12 18:28:21.824 | 10120 |

+ Report
  
 | local_date | city_name | top1_driver_name | order_cnt | area_cnt |
 | ----- | ----- | ----- | ----- | ----- |
 | 2024-09-02 | Chicago | Mike | 2 | 2 |
 | 2024-09-02 | Phoenix | Alex | 1 | 1 |

