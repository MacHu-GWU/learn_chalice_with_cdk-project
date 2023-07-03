Learn Chalice with CDK
==============================================================================
AWS Chalice 确实方便了很多部署 Lambda App 的工作. 它于 2021 年推出了 CDKv2 的支持, 但是文档很不完善. 而且很多 Configuration 都不知道在哪里调. 我个人觉得目前为止 2023-06 还不推荐使用 CDKv2 来部署 Chalice. 我目前选择用 CDK 部署 infra, 然后让经典的 Chalice 部署方式来部署 App.

.. code-block:: bash

    virtualenv -p python3.8 .venv

.. code-block:: bash

    source .venv/bin/activate

.. code-block:: bash

    pip install chalice

.. code-block:: bash

    pip install "chalice[cdkv2]"

.. code-block:: bash

    cdk deploy

.. code-block:: bash

    cdk destroy
