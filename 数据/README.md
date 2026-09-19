# 数据说明

## 数据来源

- 数据集名称：直播电商数据集
- 来源平台：阿里云天池实验室
- 数据集页面：https://tianchi.aliyun.com/dataset/124814
- 使用目的：个人数据分析学习与求职作品集展示

## 数据规模

- 原始记录：5,630条
- 唯一用户：5,630位
- 原始字段：19个
- 分析粒度：每行代表一位用户

## 核心字段

| 字段 | 含义 |
|---|---|
| CustomerID | 用户编号 |
| Churn | 是否流失 |
| Tenure | 用户生命周期 |
| PreferredLoginDevice | 常用登录设备 |
| CityTier | 城市等级 |
| OrderCount | 订单数量 |
| DaySinceLastOrder | 距最近一次下单天数 |
| PreferedOrderCat | 偏好品类 |
| NumberOfStreamerFollowed | 关注主播数量 |
| SatisfactionScore | 满意度评分 |
| Complain | 是否投诉 |
| CouponUsed | 优惠券使用数量 |
| DiscountAmount | 优惠金额 |

## 目录说明

- `原始数据/`：从天池数据集页面获得的原始数据。
- `处理后数据/`：由Notebook生成的统计结果、用户分层和Tableau数据文件。

## 数据处理

项目对原始数据执行了以下处理：

1. 字段类型与取值范围检查；
2. 缺失值检查与中位数填充；
3. 重复用户检查；
4. 文本类别标准化；
5. 业务规则与潜在异常值检查；
6. RFG、Persona、Risk Level和策略字段生成。

## 许可说明

本仓库中的分析代码和原创文档可按照仓库的软件许可证使用。

原始数据及其相关权利归原数据发布方所有，不包含在本仓库的软件许可证授权范围内。使用者应前往阿里云天池数据集页面查看并遵守适用的数据使用条款。