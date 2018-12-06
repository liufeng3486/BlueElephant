BlueTest
====================

测试工程师使用的标准测试库。包含接口、压力、UI测试相关一站式解决方案

要求
------------
* `Python`_ 3.5.3+
* `Request`_ 2.0.0+

Python下载路径``https://www.python.org/downloads/``
Request下载路径``https://pypi.org/project/requests/`` or 使用pip命令 ``pip install requests``

安装
------------
最简单的安装方式就是使用``pip``命令，作为一个pythoner,``pip``是必备工具之一

.. code-block:: html

    pip install BlueTest 
    pip3 install BlueTest # 双python环境 python3 pip   

**试一下，傻瓜式的Demo**

.. code-block:: python

    >>>import BlueTest
    >>>BlueTest.test()        #接口基础测试DEMO
    >>>BlueTest.presstest()   #接口压测DEMO
    - INFO: 测试数据生成 .//srcdata//test.json.postman_collection
    - INFO: postman转csv成功:./srcdata/test.csv
    - DEBUG: CSV文件内容序列化成功:[{'Lv': '', 'Cname': '', ...
    - INFO: log exceptionCheck: 普通请求 ...
    - INFO: log exceptionCheck: ['date']为空 ...
    - INFO: log exceptionCheck: ['date']不传 ...

-------------------
至此，你已经完成了自动化测试从0-1的壮举。

Table of Contents
-----------------
.. toctree::
   ApiTest 
   Markup
   methods
   events
   keyboard
   i18n
