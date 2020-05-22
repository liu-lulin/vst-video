# Qt 全聚合影视
基于 Qt 的 QMultiMedia组件构建，目标是搭建deepin v20云播放平台。  
"vst-video"文件是已编译好的程序,适用于64位Linux系统Qt5环境,双击运行,终端运行"./install.sh"生成桌面图标。  
### 依赖  
sudo apt-get install libqt5multimedia5 libqt5multimediawidgets5 qtmultimedia5-dev

### 更新记录：

2020.05.22 发布 V2.52 正式版
主要更新：
1.更换视频输出组件,修复视频边框蓝条闪烁问题;
2.添加视频旋转功能,视频对比度调节等功能暂时失效;

2020.05.20 发布 V2.51 正式版
主要更新：
1.添加播放记录功能;
2.添加主题设置功能;
3.标题栏添加功能菜单(置顶,最大化,最小化,关闭等);

2020.05.19发布 V2.5 正式版
主要更新：
1.优化UI,标题栏添加设置按钮。
2.修复已知BUG。

2020.05.16 发布 V2.43 正式版
主要更新：
1.搜索添加右键功能菜单。
2.播放器UI更新，按钮素材全部改用矢量图。
3.修复首次播放剧集时总是第一集的BUG。

2020.05.14 发布 V2.42 正式版
主要更新：
1.浏览器添加右键功能菜单，支持调用关联程序打开。
2.加入关于对话框，去掉标题版本信息。
3.细微调整播放器UI，控制栏改为紫罗兰色

2020.05.14 发布 V2.41 正式版  
主要更新：
1.浏览器添加右键功能菜单，支持调用关联程序打开。
2.加入关于对话框，去掉标题版本信息。

2020.05.13  发布 V2.4 正式版  
主要更新：
1.优化启动速度，采用线程刷新资源;
2.添加超时设置，修复可能卡界面的BUG;
3.添加资源设置窗口，方便在软件修改资源;
4.播放器右键添加画面缩放设置;

2020.05.11  发布 V2.3 正式版  
* 播放器右键添加功能菜单，支持本地和远程文件播放;
* 增加对命令行参数的支持，现在可用作本地播放器;

2020.05.08  发布 V2.2 正式版  
*  修复已知BUG,优化操作体验;
*  以deb安装包形式发布。

2020.05.08  发布 V2.1

* 添加直播功能，配置文件为程序目录的live.txt文件，格式和资源一样。
*  修复已知BUG，优化体验。

2020.05.06

发布v2.0 测试版

*软件基本成型，欢迎测试。

2020.5.1
* 添加列表显示开关,修复BUG ;
* 添加安装脚本，现在可以安装桌面图标。

2020-04-30
*添加等待动画效果;
* 列表播放支持，剧集自动连播放;
* 添加常用快捷键，全屏下可以直接上下箭头控制音量，左右箭头控制快进快退，空格暂停/播放
*  源码采集方式更新，采用xml的DOM遍历方式，取消原来的正则搜索

故障排除：

有声音无视频:  
【 Linux】
* 报 va 相关错误  
参考：https://bugreports.qt.io/browse/QTBUG-23761  
解决：sudo apt-get remove gstreamer1.0-vaapi  

* 不报错
sudo apt-get install gst123  
下列【新】软件包将被安装：  
gst123 gstreamer1.0-pulseaudio gstreamer1.0-x  

【Windows】
* 安装 LAV Filters 解码解决。


