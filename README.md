# keyboardbelowedittext
软键盘不遮挡EditText的输入区域
<br/>（1） 有遮挡的效果<br/>
<img src='https://raw.githubusercontent.com/supermanmwg/keyboardbelowedittext/master/pic/edittext.gif'  width="300px" />
<br/>（２）无遮挡的效果<br/>
<img src='https://raw.githubusercontent.com/supermanmwg/keyboardbelowedittext/master/pic/edittext2.gif'  width="300px" />
<br/>
主要有两个地方需要添加:<br/>
#####（１）在对应的activity的AndroidManifest.xml中添加　
android:windowSoftInputMode="adjustResize"
例如：
```xml
   <activity
    android:name=".MainActivity"
    android:windowSoftInputMode="adjustResize" >
    <intent-filter>
        <action android:name="android.intent.action.MAIN" />
        <category android:name="android.intent.category.LAUNCHER" />
    </intent-filter>
    <activity>
```
  
#####（２）在对应的layout文件中的整个layout都包含进一个ScrollView。
