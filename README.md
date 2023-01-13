其它语言:

- [简体中文](README.md)(README.md)
- [English](README.en.md)

-----
=============

版本
--------

speedpower curl


安装
------------

~~~~~~~~~~~~~~~~~~~
    curl -o speedpower https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py
    chmod +x speedpower
~~~~~~~~~~~~~~~~~~~



使用
-----
~~~~~~~~~~~~~~~~~~~

    $ speedpower -h
    usage: speedtest-cli [-h] [--amount] [--up_amount] [--city]
                         [--filesize] [--up_filesize]
                         [--thread] [--upthread]
                         [--ipv6] [--onlyup] [--onlydown]
                         [--version]

    Command line interface for testing internet bandwidth using speedtest.net.
    --------------------------------------------------------------------------
    https://github.com/sivel/speedtest-cli

    optional arguments:
      -h,  --help               显示帮助
      -a,  --amount             下载数量    [40]
      -ua, --up_amount          上传数量    [8]
      -c,  --city			    服务器节点  [gz]
      -f,  --filesize		    下载文件大小 [20]Mb 
      -uf, --up_filesize        上传文件大小 [20]Mb
      -t,  --thread             下载线程数  [4]
      -ut, --upthread           上传线程数  [2]
      -6,  --ipv6			    仅支持东北大学ipv6节点
      -od, --onlydown		    仅下载		
      -ou, --onlyup		        仅上传	
      -V,  --version            显示版本
~~~~~~~~~~~~~~~~~~~

例子
-------------

1. 指定广州节点，下载99次，下载线程数8，指定文件大小1M，仅下载不上传
~~~~~~~~~~~~~~~~~~~
    ./speedpower --city gz --amount 99 --thread 8 --filesize 1 --onlydown
~~~~~~~~~~~~~~~~~~~

2. ipv6协议，下载101次，上传20次，上传线程数2，指定上传文件50M
~~~~~~~~~~~~~~~~~~~
    bash speedpower --ipv6 gz --amount 101 --up_amount 20 --upthread 2 --up_filesize 50
~~~~~~~~~~~~~~~~~~~
   
