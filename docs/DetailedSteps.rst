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

这样我们就获得了最原始的数据 ``test.json.postman_collection`` 名字很长，这是postman规定的，请暂时忍受一下。

由于这个文件的可读性比较差，而且不利于维护和使用，所以需要生成一个中间文件，在这里选用的是 ``csv`` 格式。

  ``csv`` 作为 `BlueTest` 的标准数据文件，为了支持这一实现方式。
  
  还提供了 ``postman`` 文件, 标准 ``swagger`` ，标准 ``YAPI`` 一键转换为 ``csv`` 的功能
  
  而且不用担心，如果你的数据源不是以上格式，在后面的详细介绍中，会有 ``csv`` 文件格式的详细说明。可根据说明，编写自己的测试数据一键转换功能。

.. code-block:: python

    BlueTest.initPostMan(name,result_path = "")
    
**initPostMan**
    




