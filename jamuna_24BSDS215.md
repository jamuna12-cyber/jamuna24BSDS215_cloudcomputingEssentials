mkdir data_etl
mkdir -p data_etl/{January,February,March,April,May,June,July,August,September,october,November,December}
touch data_etl/January/extract_sales_data.py
touch data_etl/January/transform_customer_data.py
touch data_etl/January/load_order-data.py
mv data_etl/March/transform_customer_data.py ./data_etl/May/
mv data_etl/May/transform_customer_data.py data_etl/May/new_transform_customer_data.py
cd data_etl/
ls
touch sensitive_data_load.sh
chmod 700 sensitive_data_load.sh
ls -l sensitive_data_load.sh
mkdir backup
cp sensitive_data_load.sh backup/
rm March/load_order-data.py
rm March/extract_sales_data.py 
rmdir March
nano sensitive_data_load.sh 
./sensitive_data_load.sh 
history |tail -20
history | grep 'extract'
uptime
chmod 700 sensitive_data_load.sh
ping -c 4 example.com
find data_etl/ -name "extract_sales_data.py"
grep "for" sensitive_data_load.sh 
mkdir -p data_etl/{data_analyst,etl_admin,data_engineer}
chmod 700 data_etl/data_analyst/
chmod 700 data_etl/data_engineer/
chmod 700 data_etl/etl_admin/
find data_etl/ -type d -empty -delete 
ls -lt
ls -ls
find data_etl/ -type f -name "*.py"
tar -cvf data_etl_backup.tar.gz data_etl/
tar -tvf data_etl_backup.tar.gz
