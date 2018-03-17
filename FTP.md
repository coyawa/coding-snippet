

```sh
ftp ftp-server
```

```sh
wget ftp://caris.ct.pb.com//work21/us/us_leasingcontracs.sas7bdat
```

```sh
wget -r 'ftp://bigdata:pitney1a@161.228.114.53/work21/us/us_leasingcontracs.sas7bdat'
```

wget —user=bigdata --password=pitney1a ftp://caris.ct.pb.com/work21/us/us\_leasingcontracs.sas7bdat

```sh
curl -u bigdata:pitney1a 'ftp://caris.ct.pb.com//work21/us/us_returns.sas7bdat' -o ~/us_returns.sas7bdat

curl ftp://161.228.114.53/work21/us/us_leasingcontracs.sas7bdat --user bigdata:pitney1a -o us_leasingcontracs.sas7bdat
```

ftp://caris.ct.pb.com//work21/us/us\_returns.sas7bdat

```sh
quit
```

