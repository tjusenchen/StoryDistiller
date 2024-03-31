# New Versions

* March 31, 2024: We will release a new version soon to extract storyboards with more UI scenarios compared with SceneDroid, StoryDistiller, and StoryDroid for Android apps!

* We developed an extended version of StoryDroid/StoryDistiller to explore more scenes of GUI pages, named [SceneDroid](https://github.com/SceneDroid/SceneDroid).

# StoryDroid/StoryDistiller
We have made the source code publicly available. We hope this project can benefit other researchers or practitioners in the field of analysis of Android apps. Please contact us (senchen@tju.edu.cn) if you have any questions or issues. We will continue to maintain this project. Thanks for your feedback.

## Environment Configuration
* Ubuntu/Macbook
* Python: 2.7
* APKTool: 2.6.1 (Please use the newest version of APKTool)
* Android emulator：X86, Android 7.1.1, Google APIs, 1920 * 1080
* Android environment: adb, aapt
* Java environment (jdk): jdk1.8.0_45
* pip install opencv-python==3.4.3.18
* IC3: https://github.com/siis/ic3, please take the tool into the path /StoryDroid/main-folder/
* jadx: https://github.com/skylot/jadx, please take the tool into the path /StoryDroid/main-folder/
* libs support: Please take the android.jar files of all the different platform versions (android-3~android-32) into the path /StoryDroid/main-folder/config/libs/android-platforms/
* Open ~/.bashrc and configure the path of JDK and SDK (Replace by your own paths):
```
export JAVA_HOME=/usr/lib/jvm/jdk1.8.0_45
export JAVA_BIN=/usr/lib/jvm/jdk1.8.0_45/bin
export CLASSPATH=.:${JAVA_HOME}/lib/dt.jar:${JAVA_HOME}/lib/tools.jar
export PATH=$PATH:${JAVA_HOME}/bin
export PATH=$PATH:/home/dell/Android/Sdk/tools
export PATH=$PATH:/home/dell/Android/Sdk/platform-tools
export PATH=$PATH:/home/dell/Android/Sdk/emulator
export JAVA_HOME JAVA_BIN CLASSPATH PATH 
```

## StoryDroid/StoryDistiller Usage
* If you want to use the full function of StoryDroid, please use the following command: 
```
python2.7 main_full.py
```

* If you want to use the function of atg (Activity transition graph) generation, please the following command: 
```
python2.7 main_partial.py
```

# StoryDroid+
StoryDroid+ provides an operation-friendly platform for using storyboards and helps different stakeholders (e.g., designers, package managers, developers) explore and understand apps from different perspectives through rich visual pages.
<img width="1408" alt="overview" src="https://user-images.githubusercontent.com/23289910/203773727-dbb7ffb2-69d6-4ba2-8185-5db0868d14f5.png">

## Configuration
* The ***Environment Configuration*** of StoryDroid+ is the same as that of StoryDroid/StoryDistiller.
* StoryDroid+ uses ***Flask*** framework to build an offline website, a lightweight customizable framework, written in Python, which is more flexible and secure. So:
```
pip install flask
```

## StoryDroid+ Usage
The folder ***"code-for-web-v2.0"*** is the latest version of StoryDroid+, in which the folder ***"templates"*** contains the front-end code of StoryDroid+, and the folder ***"static"*** contains the resource files of StoryDroid+. If you want to use the full function of StoryDroid+, please use the following command:
```
python2.7 test.py
```

## Contact
[Sen Chen](https://sen-chen.github.io/) All Copyright Reserved.
