

### For the Pie/Dount Chart

```js
// Auto Pay
SUM([AutoPayVol])/SUM([OrdVol])

// AutoPayVol
IF ([Field1] = "Auto Pay") THEN [Value] ELSE 0 END

// Placeholder
MIN(0)

// Manual
1-(SUM([AutoPayVol])/SUM([OrdVol]))
```

Steps:

Pre:

Create the Measure: Placeholder, Autopay, Manual

0: Filter with the **autopay** & **manual**

1\. Put the Measure Names into the Placeholder (as color)

2\. Put the Measure Value into the Placeholder (as angle)

3\. Put the Autopay to the label into the Placeholder (2)

4\. Change the Placeholder size

```sh
Option 1: Convert to a Date Field
Select Analysis > Create Calculated Field.
Type the following into the Formula field, and then click OK:
  
DATE(DATEADD('second', INT([Unix Date]), #1970-01-01#))

Option 2: Convert to a Datetime Field
If the date is interpreted as a string instead of a number value, right-click the field and select Change Data Type > Number.
Select Analysis > Create Calculated Field.
Type the following into the Formula field, and then click OK:
  
DATEADD('hour',-7,(Date("1/1/1970") + ([Unix Date]/86400)))

Important: -7 will need to be  adjusted based on your timezone (Unix time corresponds to UTC, therefore -7 corresponds to Pacific Standard Time).

```







**Tips-Tableau**

[Convert a Field to a Date Field](https://onlinehelp.tableau.com/current/pro/desktop/en-us/data_dateparse.html)

[Tableau Tip: Building KPI Dashboards with Shapes - The Data School](http://www.thedataschool.co.uk/emily-chen/building-kpi-dashboards-with-shapes/)

[Tableau 201: How to Make Donut Charts | EvolyticsEvolytics | Data Analytics A full service analytics agency](http://www.evolytics.com/blog/tableau-201-how-to-make-donut-charts/)

[1 Easy Trick to get Clustered Bar Charts – VizPainter](https://vizpainter.com/1-easy-trick-for-clustered-bar-charts/)