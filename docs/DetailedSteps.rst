DetailedSteps
=======
在这里介绍如何使用 `bluetest` 一步一步完成工作。

首先让我们看下 `bluetest` 里的主要 ``.py`` 文件
    
   * ``logInit.py`` 日志相关
   * ``parm.py`` 配置参数
   * ``press.py`` 压测相关
   * ``toolbox.py`` 工具箱
   * ``dome_test.py`` 范例
   * ``core.py`` 接口基础测试相关
 

准备数据 
------
我们从第一步开始，准备数据。
按照我们的约定，做接口测试的源数据可以是 ``postman`` 里download下来的数据。如下图所示：

.. figure:: _static/screenshots/dtailedsteps_postman.png
    :align: center
    
def initPostMan(name,result_path = "")
