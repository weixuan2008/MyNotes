### 管理conda自身

# 查看conda版本
- conda --version

# 查看conda的环境配置
- conda config --show

# 更新conda
- conda update conda

# 更新Anaconda整体
- conda update Anaconda

# 查询某个命令的帮助
- conda create --help

### 管理环境
# 创建虚拟环境
- conda create -n env_name python=3.13
- 创建后，env_name文件可以在Anaconda安装目录envs文件下找到


# 查看有哪些虚拟环境
- conda info -e
- conda info --envs

# 激活虚拟环境
- conda activate env_name
- 在4.6版本以前需要使用如下命令：
- Linux:  source activate your_env_name
- Windows: activate your_env_name

# 退出虚拟环境
- conda activate
- conda deactivate


# 删除虚拟环境
- conda remove --name env_name --all


