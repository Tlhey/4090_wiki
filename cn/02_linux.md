# Linux
SSH 连接服务器
`ssh {yourname}@10.200.13.23 #{yourname}` 替换成你的用户名


资源占用
```
nvidia-smi #看显卡/cpu状况  
htop       # 查看系统资源使用情况 
top        # 查看进程资源占用 
```
 
查看进程 
```
ps aux | grep python 
ps -ef | grep python  # 另一种查看方式 
```

正在运行的进程： \
    查看 `jobs` \
    暂停 `cmd/ctrl + Z` (keyboard shortcut) \
    删除 `kill %1`   或者`ctrl C`(keyboard shortcut) \
    后台运行 `cmd &` \
    切换到前台 `fg %1` \
 \

关于进程的操作:
```
jobs -l         # 查看任务列表（带 PID）
jobs -p         # 只显示任务的 PID
kill %i         # 删除指定编号的任务
for job in $(jobs -p); do kill -9 %$job; done  # 删除所有后台任务（慎用！）
```


重启命令行 \
`source ~/.bashrc`  # 重新加载配置文件 \
 \


文件操作
```
ls -la                # 列出当前目录下的所有文件（包括隐藏文件）
cd /path/to/dir       # 进入你想去的目录
pwd                   # 显示你当前所在的目录
```

