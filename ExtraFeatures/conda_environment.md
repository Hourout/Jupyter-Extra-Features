# 创建conda虚拟环境


| 命令 | 解释 |
| --- | --- |
| conda list | 查看安装了哪些包 |
| conda info -e | 查看系统中存在的虚拟环境 |
| conda update conda | 检测更新 |
| conda create -n xxx python=3.6.9 | 创建虚拟环境需要制定新建的虚拟环境的名称以及python的版本 |
| conda activate xxx | 激活进入新建的虚拟环境 |
| conda deactivate | 关闭退出当前的虚拟环境 |
| conda remove -n xxx --all | 删除虚拟环境 |

创建一个你需要的虚拟环境，在base环境下安装包nb_conda，用来jupyter访问虚拟环境
```
conda install nb_conda
```
注意，jupyter服务必须在base环境下启动，并且所有的环境都必须安装jupyter
