

```sh
# Upload the files and folder to Server through SSH
rsync -avu --progress /Users/Coyawa/Downloads/test/ congyang@urban.cs.wpi.edu:/urbanshare/k-project/sampleData/
```

<https://www.linode.com/docs/tools-reference/modify-file-permissions-with-chmod>

\# Modify File Permissions with chmod

```sh

```

Links:

SSH Tutorial - How to Use SSH

Linux SSH远程文件传输命令scp - VPS侦探

SSH原理与运用（一）：远程登录 - 阮一峰的网络日志



```sh
Tips-Shell

Shell
ssh user@192.168.1.1 -p 222
sudo -i

%sh
today_date=$(date '+%Y-%m-%d')
echo $today_date
yesterday=$(date -d '7 days ago' +%Y-%m-%d)

# Rename the file
mv aa.csv bb.csv
mv xx yy

Rm -rf

autoenv  source bin/activate
./**.sh

ssh yzhao7@ace.wpi.edu login with ssh pub key

ls -l /tmp/congyang/


ssh congyang@urban.cs.wpi.edu
PW: 
rabbit=Liver4Cider
/home/guanxiong/AttentionModel/geo_summer/

How to find the size of a directory in Linux - OSTechNix
du -h ProcessedData/
du -sh

apt-get  // check the server description

Cd ..

cd /home/guanxiong/AttentionModel/geo_summer

scp -ra /Users/Coyawa/Git/geo_attention congyang@urban.cs.wpi.edu:/home/guanxiong/AttentionModel/geo_summer

scp -r /Users/Coyawa/Git/geo_attention  congyang@urban.cs.wpi.edu:、home/guanxiong/AttentionModel/geo_summer

Learn How to Search in Your Files and Folders via SSH Tutorial

For example, to search for a file called myFile.txt under the current folder (and all subfolders), you would need to use the following command:

find . -name myFile.txt

Give execute permission to your script:
chmod +x /path/to/yourscript.sh
And to run your script:
/path/to/yourscript.sh
Since . refers to the current directory: if yourscript.sh is in the current directory, you can simplify this to:
./yourscript.sh

Lshw get the server info


```



```sh
# chown command changes the user and/or group ownership of for given file. The syntax is:

chown owner-user file 
chown owner-user:owner-group file
chown owner-user:owner-group directory
chown options owner-user:owner-group file
```













