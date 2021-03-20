### 登陆集群

-   在校园网or跳板机环境，使用分配给各位同学的用户名和密码，使用ssh登陆

    ```bash
    ssh <user_name>@<ip>
    ```

-   登陆之后使用bash命令行（有余力的同学也可以给自己配置zsh提升开发体验）
-   下面是测试账号登陆的的实况截图，从跳板机进行登陆
-   `/home/<user_name>`是各位同学自己的用户目录，用户目录之外的文件夹请不要访问，以免影响机器环境
-   安装python库时，建议通过`pip3 install <pkg_name> --user`命令安装

![](/thuacv/Screen Shot 2021-03-19 at 20.00.38.png)

### 验证评测命令(xsubmit)可用

-   执行`xsubmit -v`命令查看版本；执行`xsubmit -h`命令查看使用帮助
-   如执行这两个命令出现和下图类似的输出，则说明评测命令正常运行

![](/Users/chenqingchen/Desktop/thuacv/Screen Shot 2021-03-19 at 20.01.10.png)

### 修改密码

-   这里有两个密码，一个是各位同学登陆集群的账号密码，一个是提交评测的账号密码，默认这两个账号密码是相同的
-   为了保证每位同学个人信息的安全，建议第一次登陆集群后修改密码（**这里指提交评测的账号密码**），具体操作方式如下图所示

![](/Users/chenqingchen/Desktop/thuacv/Screen Shot 2021-03-19 at 20.02.21.png)

### 提交评测+查看提交

-   提交评测输入使用`xsubmit submit`子命令，查看个人提交记录使用`xsubmit lookup`子命令，具体操作方式参考下列两张图
-   提交结果的状态分为pending, running, success, fail四种类别
-   每位同学每天有**两次**提交次数，超过次数的提交将被拒绝
-   为了白天尽量不占用机器资源，大部分程序将在晚上进行评测
-   提交的文件需要整体打成压缩包，必须是zip格式

![Screen Shot 2021-03-19 at 20.02.26](/Users/chenqingchen/Desktop/thuacv/Screen Shot 2021-03-19 at 20.02.26.png)

![](/Users/chenqingchen/Desktop/thuacv/Screen Shot 2021-03-19 at 20.20.07.png)

### 其他

-   每天凌晨0:00 - 8:00是例行停机维护时间，请各位同学不要进行提交。（但仍然可使用GPU训练）
-   部分功能将会在之后陆续上线，也会相应更新本文档
-   有任何问题请在微信群or邮件联系相关助教
-   不要试图hack评测机，相应文件，网络操作在后台都有记录
