系统的整体结构如下图所示
graph L
MainWindow--包含-->PaintBoard
MainWindow--包含-->MyGLWidget
MainWindow-.使用资源.->icon.qrc
其中MainWindow为主窗口，实现主界面并提供主界面到各种功能之间的连接。

PaintBoard为画板类，实现所有与二维图形有关的功能，包括输入、填充、变换、裁剪等。

MyGLWidget为三维窗体类，实现与三维模型有关的功能，基本功能包括三维模型显示，还拓展了三维模型的旋转（随鼠标运动）和三维模型的缩放（鼠标滚轮控制）。

icon.qrc用于管理与系统有关的所有资源文件，主要包括各种图标。
