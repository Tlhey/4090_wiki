# Mamba
## Download
如果遇到了陈年的老仓库（python<=3.10, torch=1.x，用conda装环境会变得非常困难。Mamba是一个很好的替代。~~~比如我刚刚就成功的装了一个奇怪的环境~~~

mamba下载教程(4090机器):
```wget -4 "https://mirrors.tuna.tsinghua.edu.cn/github-release/conda-forge/miniforge/LatestRelease/Miniforge3-24.11.3-2-Linux-x86_64.sh" ```
安装即可。

使用方法,和conda基本一致，只是把`conda`换成`micromamba`即可。

## env.yaml
对于env.yaml文件：
```micromamba env create -f env.yml (-y) > install_log.txt 2>&1 &```
即可成功生成环境。

小技巧1：如果遇到了不兼容，可以挑出比较关键的包（含有torch）的保留版本号，剩下的包都去掉版本号。亲测有效。

小技巧2: 将下面代码加入env.yaml文件:

```
- pip:
    - -i https://pypi.tuna.tsinghua.edu.cn/simple               # (1)换清华源加速下载（可以加速）
    - --extra-index-url https://download.pytorch.org/whl/cu116  # (2)下常用的旧版本(记得改cuda编号) ,可以解决很多库旧版本pip无法找到的问题
```