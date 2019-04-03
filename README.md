# cordova-plugin-IFlyspeech
科大讯飞的语音听说读写的cordova插件 
### Supported Platforms

- iOS
- android

## Installation

一、sdk替换 

1、在科大讯飞官网创建完应用后，下载ios、android不同版本的sdk到本地。

ios目录：cordova-plugin-IFlyspeech-master/src/ios 
android目录：cordova-plugin-IFlyspeech-master/src/android/libs 

然后将讯飞上面下载的sdk 
ios路径：lib/iflyMSC.framework 
android路径：libs分别替换到github插件解压的文件夹里面

二、配置appid修改 

1、Android：修改 cordova-plugin-IFlyspeech-master/plugin.xml文 件内容， 搜索【android:name=”IFLYTEK_APPKEY”】， 将对应的android:value=”改为申请的android版本的appid”

2、Android：修改 cordova-plugin-IFlyspeech-master/src/android/res/values/strings.xml文件内容 搜索【app_id】将对应的值改为申请的android版本的appid

3、ios：修改 cordova-plugin-IFlyspeech-master/src/ios/CDVSpeech.m文件内容 搜索【#define SPEECH_APP_ID】，将对应的值改为申请的ios版本的appid

完成后再执行cordova添加插件命令即可： cordova plugin add 插件（cordova-plugin-IFlyspeech-master）本地路径

