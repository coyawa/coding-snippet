```js
(SUM([Number of Records])-([BOL-Goal]/12*[Goal-MTD]))*12/[BOL-Goal]*[Goal-MTD]

(SUM([Logins])-([login-Goal]/12*[Goal-MTD]))*12/[login-Goal]*[Goal-MTD]


(SUM([supplies])-([Supplies-Goal]/12*[Goal-MTD]))*12/[Supplies-Goal]*[Goal-MTD]

(SUM([Supplies Unique Visitors])-SUM([Orders]))/SUM([Supplies Unique Visitors])/[Aband-Goal]

SUM([Orders])/SUM([Supplies Vists])/[CovRate-Goal]

SUM([Supportvisits])/[support-Goal]

SUM([Supportvisits])/[support-Goal]

(SUM([Supportvisits])-([support-Goal]/12))*12/[support-Goal]*[Goal-MTD]


ZN( SUM(
[Supportvisits]-([support-Goal]/12*[Goal-MTD])+([support-Goal]*[Goal-MTD]/12))
)


MTD2
  [dateCre] >= [StartDate] and [dateCre]<= [EndDate]
StartDate
  MAKEDATE(YEAR([MaxDate]),MONTH([MaxDate]),01)
EndDate
  [MaxDate]
MaxDate
  { FIXED:MAX([dateCre])}



Progress bar chart
WINDOW_MAX(AVG([Discount]))







```

