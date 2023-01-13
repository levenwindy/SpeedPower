Other languages:

- [Chinese Simplified](README.md)(README.md)
- [English](README.en.md)

-----
=============

Versions
--------

speedpower works with curl


Installation
------------

~~~~~~~~~~~~~~~~~~~
    curl -o speedpower https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py
    chmod +x speedpower
~~~~~~~~~~~~~~~~~~~



Usage
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
      -h, --help            show this help message and exit
      --amount              Number of Downloads [40]
      --up_amount           Number of uploads   [8]
      --city			    Select your server  [gz]
      --filesize		    Download File Size  [20]Mb 
      --up_filesize         Upload File Size    [20]Mb
      --thread              Download threads    [4]
      --upthread            Upload threads      [2]
      --ipv6			    Only Support N.U Server
      --onlyup		        Just Download Test	
      --onlydown		    Just Upload Test		
      --version             Show the version number and exit
~~~~~~~~~~~~~~~~~~~


Example
-------------

1. 指定广州节点，下载99次，下载线程数8，指定文件大小1M，仅下载不上传
~~~~~~~~~~~~~~~~~~~
    ./speedpower --city gz --amount 99 --thread 8 --filesize 1 --onlydown
~~~~~~~~~~~~~~~~~~~

2. ipv6协议，下载101次，上传20次，上传线程数2，指定上传文件50M
~~~~~~~~~~~~~~~~~~~
    bash speedpower --ipv6 gz --amount 101 --up_amount 20 --upthread 2 --up_filesize 50
~~~~~~~~~~~~~~~~~~~
