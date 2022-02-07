# domoticz2influxdb - Convert offline domoticz database to influxdb line format

`domoticz2influxdb.py` takes a domoticz database and converts this data to the
influxdb line format, which can subsequently be loaded as bulk data into 
influxdb through e.g. `curl` using 

    curl -i -XPOST "http://localhost:8086/write?db=mydb" --data-binary @data.txt

See https://docs.influxdata.com/influxdb/v1.7/tools/api#examples-6

