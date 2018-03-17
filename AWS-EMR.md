

```sh
 ssh -i ~/wang.pem hadoop@ec2-34-212-233-70.us-west-2.compute.amazonaws.com 
 aws s3 cp s3://pbdl-bda-xbec/staging/sharedworkspace/congyang_pipeline/us_leasingcontracs.csv us_leasingcontracs.csv
```



```sh
-- check the EMR disk usage
-- Q: How to use the disk out of the /dev/xvda1
df -h

Filesystem      Size  Used Avail Use% Mounted on
devtmpfs        7.4G   28K  7.4G   1% /dev
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvda1      9.8G  9.3G  336M  97% /
/dev/xvdb1      5.0G   37M  5.0G   1% /emr
/dev/xvdb2       33G  649M   32G   2% /mnt
/dev/xvdc        38G  451M   38G   2% /mnt1
```



```sh
# Load the new drive in EMR
cd /mnt
cd /mnt1
```



```sql

```



```sql

```

























