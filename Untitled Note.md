```sh
#Upload the file to ccc
rsync -avu --progress /Users/Coyawa/Downloads/osram_total_update.sql cwang8@ccc.wpi.edu:/home/cwang8/data/osram_total_update.sql

rsync -avu --progress /Users/Coyawa/Downloads/write_new.sql cwang8@ccc.wpi.edu:/home/cwang8/data/write_new.sql


#write csv into sql table
 load data local infile '/home/cwang8/data/osram_total_update.csv' into table osram_total_update
 fields terminated by ','
 enclosed by '"'
 lines terminated by '\n';
 
 
 mysql -hmysql.wpi.edu -ucwang8 -p2FXyug osram  
 source /home/cwang8/data/osram_total_update.sql
```