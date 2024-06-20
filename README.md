# AI摄像头在线文档仓库
https://aicamera-v831-documentation.readthedocs.io/zh/latest/

## AI摄像头在线文档

git remote add origin https://github.com/labplus-cn/AICamera-v831-documentation.git
## 编译步骤

git clone https://github.com/labplus-cn/AICamera-v831-documentation.git

python3环境安装依赖库

    pip3 install -r requirements.txt

本地编译

    cd documentation
    make html

如果成功，构建的文件将位于其中documentation/_build 文件夹，
HTML 页面保存在 _build/html 目录。

## 文件结构

_static 静态文件

example 示例

faq 常见问题解答，帮助支持

hardware_introduction AI摄像头介绍

programming_mode 编程工具介绍

tutorials 教程

_build 编译文件目录

## readthedocs在线文档管理
https://readthedocs.org/projects/aicamera-v831-documentation/