创建container

~~~
docker run -it --gpus all --name test_gpu xxx
~~~



~~~
apt-get update
~~~



~~~
apt-get install software-properties-common
~~~

由第三方维护的PPA软件源来方便的安装所需要的Python版本

~~~
add-apt-repository ppa:deadsnakes/ppa
~~~

安装上面两个之后可以安装python，否则报错

~~~
apt-get update
apt-get install python3.6
~~~



修改python3.6为优先使用 优先级为1

~~~
update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 1
~~~



安装python3.6-dev

~~~
apt-get install python3.6-dev
~~~

安装pip

~~~
apt-get install python3-pip
~~~



~~~
pip3 install numpy==1.10.1 -i https://pypi.tuna.tsinghua.edu.cn/simple
~~~

下载pytorch

~~~
pip3 install torch==1.5.0 torchvision==0.6.0 -i https://pypi.tuna.tsinghua.edu.cn/simple
~~~

