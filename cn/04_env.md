# 环境配置
## Conda
### 安装：
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

conda和pip的关系:简单的来说可以理解为 （建议在conda环境中先用conda，无法解决的话用pip安装一些conda中没有的lib）

### 是否在conda环境：   
anaconda的安装和自动启动，相关脚本在： `~/.bashrc ` , \ 
如果输出是空白，则不在conda环境中： `echo $CONDA_DEFAULT_ENV  `   

### 常用conda命令: 
把{env_name}替换成真实环境名 
```bash
conda create -n {env_name} python=3.8  # 创建 
conda activate {env_name}              # 激活 
conda deactivate                       # 退出环境 
conda env list                         # 查看所有环境 
conda list                             # 查看当前环境安装的libs 
conda env remove --name {env_name}     # 删除环境 
```
