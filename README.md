# Loan-default-forecast

以预测用户贷款是否违约为任务

https://tianchi.aliyun.com/competition/entrance/531830/introduction

一、baseline

1、数据清理

只清理了非数字格式的字段

1）共5个，'issueDate'，'grade'，’subGrade‘，'employmentLength'

'issueDate'将数据转换为时长

'grade',’subGrade‘转换为定顺数据，未进一步处理

'employmentLength'转换为数字，10年以上的转换为15，1年以下转换0.5

2）删除指标，’id','issueDate','policyCode','n2.2','n2.3'

2、建模

选用lightgbm,catboost，xgboost 合成预测结果


