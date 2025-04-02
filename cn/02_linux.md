# Linux
看显卡/cpu状况 \
nvidia-smi \
htop  # 查看系统资源使用情况 \
top   # 查看进程资源占用 \
 \
查看进程 \
ps aux | grep python \
ps -ef | grep python  # 另一种查看方式 \
 \
正在运行的进程： \
    查看 jobs \
    暂停 cmd/ctrl Z \
    删除 kill %1   或者ctrl C \
    后台运行 cmd & \
    切换到前台 fg %1 \
 \
删除jobs \
kill %i \
删除所有jobs \
jobs -l, 或者 jobs -p \
for job in $(jobs -p); do kill -9 %$job; done \
 \
重启命令行 \
source ~/.bashrc  # 重新加载配置文件 \
 \
文件操作 \
ls -la  # 查看当前目录下所有文件(包括隐藏文件) \
cd /path/to/dir  # 切换目录  \
pwd  # 显示当前目录 
