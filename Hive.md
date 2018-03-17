Hive学习之创建、删除、Truncate表\_Hive\_IThao123 - IT行业第一站

<http://www.ithao123.cn/content-578181.html>

```sql
DROP TABLE sas_billingplan;
CREATE EXTERNAL TABLE sas_billingplan
	 (
		Description_Of_Rule_Of_Billing_O STRING,
		Billing_Value STRING,
		Sold_To_Party STRING,
		Material_Number STRING,
		Material_Description STRING,
		Sales_Document STRING,
		Rule_For_Origin_Of_Next_Billing STRING,
		Billing_Value0, STRING,
		Company_Code STRING,
		Sales_Document_Item STRING,
		Billing_Date STRING
	 )
ROW FORMAT DELIMITED
FIELDS TERMINATED BY ','
LINES TERMINATED BY '\n'
STORED AS INPUTFORMAT
'org.apache.hadoop.mapred.TextInputFormat'
OUTPUTFORMAT
'org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat'
LOCATION
's3://pbdl-bda-xbec/staging/sharedworkspace/congyang_pipeline/sas_billingplan/'
tblproperties ("skip.header.line.count"="1")
```



























