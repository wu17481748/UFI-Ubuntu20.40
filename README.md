# UFI-Ubuntu20.04


随身wifi-Ubuntu20.04系统

刷入方法:

windows系统

fastboot一键刷入.bat

linux系统

./flash.sh

登录:

ssh root@192.168.68.1

密码:1313144



切卡:


nano /usr/lib/systemd/system/openstick-sim-changer.service

修改:Environment="SIM_ENABLED=xxxx"
例如:Environment="SIM_ENABLED=sim:sel"

可选槽位xxxx
(sim:sel  sim:sel2  sim:en  sim:en2)

通常sim:sel为卡槽:sim:sel2为esim


切换usb主机模式
echo host > /sys/kernel/debug/usb/ci_hdrc.0/role

