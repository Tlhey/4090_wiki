# 网络问题
因为是国内的地址，所以时候会连不上外国网站/下载(pip)很慢...

装很长的环境； nohup micromamba env create -f env.yml (-y) > install_log.txt 2>&1 &

1 换清华源加速下载 2 下常用的旧版本(记得改cuda)
```  
- pip:
    - -i https://pypi.tuna.tsinghua.edu.cn/simple 
    - --extra-index-url https://download.pytorch.org/whl/cu116
```
小技巧1：github用ssh可以成功clone
小技巧2: 换个时间说不定就pip通了...这是玄学