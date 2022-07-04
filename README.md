# YYS_ASSIST
###### 近日来，一款名为阴阳师的游戏引诱了我，自此我沉迷于此，宵衣旰食。日渐消瘦的我，荒废了时日，忘记了身为社会主义接班人的使命，忘记了构建人类命运共同体的伟大抱负。为了挽救我美好的青春，我必须从虚拟的世界中走出来，重新回到光明的社会中去。
###### 天下苦阴阳师久矣，枯燥的重复点击操作早已使人爱恨交加，解放双手迫在眉睫。手点? 找代肝? ，要钱还是要时间？小孩子才做选择，我都要。不如浅肝亿点点写个脚本吧？哦，不对，是代肝，代肝而已。
###### 首先，我想到的是用Python自带的pyautogui来写，至于为什么是Python呢，因为简单啊，开发效率高啊。然而，想象总是美好的，现实却很残酷，实测过程苦不堪言，通过像素点识别不仅容易乱点，还非常的浪费资源。为了更加高效的进行游戏，为社会的进步添砖Java(加瓦)。经过我深思熟虑，我决定尝试OpenCV进行图像识别，这次效果还不错，御魂觉醒之类的都可以正常进行，稳定性也不错。但是，探索副本却不尽人意。这大大阻碍了我追求梦想的脚步。
###### 最终，经过多次骚扰度娘，终于让我找到了一个图色识别利器:大漠插件。铺垫了这么多，终于可以步入正题了。干就完事了。
## 阴阳师自动化助手，防止头秃，珍爱生命，人人有责 QQ交流群：753472503
### 辅助是通过识图比色代替枯燥的重复点击操作，绝无任何修改游戏内存与游戏数据而影响游戏平衡的的操作。
#### 基于C++结合MFC开发的阴阳师辅助，结合大漠插件的图色识别函数，进行模拟人手点击操作，脚本中使用大量的随机延迟函数和随即延迟点击，
#### 并且游戏是在模拟器中运行，脚本在电脑环境运行，环境分离，只要操作得当，让脚本的行为像人一样，被检测到的几率几乎为0.
### 脚本示意图
![tags](imgs/desc.jpg)
![tags](imgs/desc2.jpg)
# 一、简单的使用方法 
###### ①点击左上角tags
![tags](imgs/点击tags.png)

###### ②选择一个发行版本进入下载相应exe
![enter](imgs/Enter.png)
###### ③选择对应屏幕缩放(100%或125%)的脚本下载即可(不同缩放的脚本只是显示效果不同，功能无任何区别)
![download](imgs/download.png)
# 二、自己编译运行
###### 1.下载源码或者通过git拉取，使用VS2017及以上版本（最好是2017）打开项目，修改YYS_AssistDlg.cpp中的大漠插件注册（有相应注释），找到代码g_dm->Reg(_T(""),_T(""));在两个_T("")中填入自己买的或找的大漠注册码和附加码。
###### 2.使用大漠图色工具（百度一大堆分享的）自己截取游戏不同场景的图片（应该挺多的，可能会有亿点点工作量哈，不想截图就用现成的exe支持一下作者哟§(*￣▽￣*)§）放在项目的pic_font文件夹（桌面端也适用，不过得自己在代码中调各个场景识别范围），
######   模拟器默认分辨率[960*540 160dpi](照着这个分辨率只需截图，不用考虑识别区域坐标)
###### 3.将项目解决方案配置改为debug或release  解决方案平台选x86  （注意：必须为x86,大漠64位需自己定制）
###### 4.CTRL + F5即可开始运行脚本
# 三、主要开发文档见文件夹：主要接口介绍文档->接口介绍.cpp
# 四、QQ交流群：753472503
# 五、自己截图说明
# 百度上可以搜到大漠综合工具，使用此工具抓图保存(需为bmp格式)，下面是抓的图示例。
![示例1](imgs/截图示例1.png)
![示例2](imgs/截图示例2.png)
![示例3](imgs/截图示例3.png)
![示例4](imgs/截图示例4.png)
![示例5](imgs/截图示例5.png)
