1. 虚拟机连接使用桥接网络模式

2. 查看ip 地址

   ifconfig | grep inet

   ![avatar](../assets/ifconfig.jpg)
   
3. ubuntu desktop 默认不安装ssh

       sudo apt-get install ssh

4. 修改ssh配置文件

        sudo vim /etc/ssh/sshd_config

        :set nu (显示行号)

        查找PermitRootLogin 该为yes

5. 重启ssh

        sudo service ssh restart

        查看状态

        sudo service ssh status

   ![avatar](../assets/ssh-status.jpg)

6. 连接

   ![avatar](../assets/ssh.jpg)
   ![avatar](../assets/success-ssh.jpg)

7. 命令连接ssh

      ssh -p 22 li@10.0.2.15

      -p ： 端口号
      li: 用户名
      