{"carnoinfo":"陕VM7869@~@/SGMP/snapshot/2021012616031240157/10.0.12.155_20210126160312_type1.jpg@~@/SGMP/snapshot/2021012616031768311/10.0.12.155_20210126160317_type3.jpg@~@/SGMP/snapshot/2021012616032295715/10.0.12.155_20210126160322_type0.jpg","groupId":"1","station":"RMDJ","contentType":"3"}


hkvision_dll_src=D:/apache-tomcat-8.0.37-windows-x64/apache-tomcat-8.0.37-sms/bin
#hkvision_dll_src=F:/tool/apache-tomcat-8.0.37-windows-x64/apache-tomcat-8.0.37/bin
################snapshot start#################
register_snapshot_ip=10.0.12.155
register_snapshot_port=8000
register_snapshot_username=admin
register_snapshot_password=www12345

weight_after_sampling_snapshot_ip=10.0.12.153
weight_after_sampling_snapshot_port=8000
weight_after_sampling_snapshot_username=admin
weight_after_sampling_snapshot_password=www12345

weight_out_snapshot_ip=10.0.12.151
weight_out_snapshot_port=8000
weight_out_snapshot_username=admin
weight_out_snapshot_password=www12345
################snapshot end#################

#aip.file.ip=10.1.4.148
#aip.file.port=21
#aip.file.username=sysadmin
#aip.file.password=ops@xa#16
#aip.file.http-path-prefix=http://10.1.4.148:88

####yangling ftp###
aip.file.ip=10.0.10.30
aip.file.port=21
aip.file.username=ftpuser
aip.file.password=kr@85263382
aip.file.http-path-prefix=http://10.0.10.30:88

#websocket
sgmp.websocket.url=http://10.0.10.30:8020/sgmp-websocket

#\u5C97\u4F4D \u83DC\u5355code */
inout_rmdj_gangwei=RMDJ
inout_lsgb_gangwei=LSGB
inout_lsqy_gangwei=LSQY
group_id_yl=1
##################barriergate start################
inOpen_byLaneNo=1
outOpen_byLaneNo=1
weightOpen_byLaneNo=1
##################barriergate end################

