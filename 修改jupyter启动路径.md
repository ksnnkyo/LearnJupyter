#修改anaconda jypyter启动路径
##1.修改anaconda安装路径/etc/jupyter/jupyter_notebook_config.json,在NotebookApp其中添加配置项："notebook_dir":"D:/JupyterCode"

##2.修改用户目录下.jupyter/jupyter_notebook_config.json,在NotebookApp其中添加配置项："notebook_dir":"D:/JupyterCode"

##3.使用命令行执行命令jupyter notebook --generate-config，在生成的jupyter_notebook_config.py中修改c.NotebookApp.notebook_dir = 'D:/JupyterCode'，去掉最开头的#号

##4.修改jupyter的快捷方式，在开始位置指定为D:/JupyterCode

#如果以上修改均未生效，查看jupyter的会计方式的启动参数中是不是带有%USERPROFILE%，有的话就去掉，则上面四种配置方式都会生效