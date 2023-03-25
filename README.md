# UFI-Ubuntu20.40


随身wifi-Ubuntu20.40系统

切卡
nano /sbin/openstick-sim-changer

修改
Environment="SIM_ENABLED=xxxx"

可选槽位xxxx
sim:sel  sim:sel2  sim:en  sim:en2

通常sim:sel为卡槽sim:sel2为esim


刷入方法:

windows系统
fastboot一键刷入.bat

linux系统
./flsh.sh


ssh root@192.168.68.1

passwd=1313144
