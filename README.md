# 12306
1230查询，采集

列车
[列车](https://kyfw.12306.cn/otn/leftTicket/queryO?leftTicketDTO.train_date=2018-03-20&leftTicketDTO.from_station=BJP&leftTicketDTO.to_station=SHH&purpose_codes=ADULT)

查询 途径站
[查询](https://kyfw.12306.cn/otn/czxx/queryByTrainNo?train_no=240000G1010D&from_station_telecode=VNP&to_station_telecode=AOH&depart_date=2018-03-30)
    

# 参数说明

名称 | 描述
---|---
train_no | 车次
train_sn | 查询 途径站 使用此编号
from_station | 出发站
to_station | 到达站
start_time | 出发时间
arrive_time | 到达时间
time_fucked_up | 历时 总耗时
arrive_type	| 到达类型 Y:当日 N:次日
first_seat | 一等座
second_seat | 二等座
business_seat | 商务特等座
soft_sleep | 软铺
hard_sleep | 硬卧
business_sleep | 高级软卧
hard_seat | 硬座
no_seat | 无座


# 使用
```
train = Train()

#查询列车
res = train.run('2018-03-30 北京 上海')
print(res)

# 查询 途径站点
# tems = train.channel(res[0])
# print(tems

```
