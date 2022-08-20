需求分析：预计算，基于维度聚合。 指标列是总和。不存原始数据。

CK没有预聚合，也是秒级。MPP+列存。
Kylin有预聚合，也是秒级。
Druid是JSON。

分析关键计算：MPP，列存，预计算。

维度和度量。

Lambda架构：离线和实时。实时写入。

问题本质是数据建模。

数据模型非常固定。
Source->Sink数据。
OLAP需求。
MPP->列式->预计算。
聚合表。

小时-》分钟-》(实时)秒-》交互式

ES在亿级别聚合很慢。百万数据实时聚合。

分析型：TB,PB

对比Druid，KyLin，CK，Doris，GP

https://bigdata.djbook.top/#term-13