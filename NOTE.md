

dataUrl:'192.168.0.200'

db:factory_dljfdc

//图谱文档：

自定义plugins：
	1.bar
	2.line3d
	3.linet
	4.overview(汇总)
	5.polar(极坐标图)


	show tag values from "MACHINE_38101" with key = "IdCh"

	$influx -import -path=datarrr.txt -precision=s
	curl -i -XPOST 'http://localhost:8086/write?db=mydb' --data-binary @file_name.txt