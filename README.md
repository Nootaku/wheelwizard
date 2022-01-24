# <img src="https://raw.githubusercontent.com/Nootaku/wheelwizard/main/resources/img/title.png" style="zoom:33%;" />

## Download and install on Android

1. Download the `.apk` : [wheel_wizard_0.0.2](foo)
2. Transfer the `.apk` to your phone
3. Install the `.apk` on your phone

_Note: As I don't have an Android Developer Account, you might get security warnings when installing the app. Feel free to look at the code before installing the app if you don't trust me. I would strongly encourage this endeavor as I believe it is something important to do for all applications._

## Install dependency

```shell
pip install kivy
pip install kivymd
pip install ffpyplayer
pip install buildozer
```

## Create an Android APK

**_Step 1: Edit the `buildozer.spec` file_**

Open `buildozer.spec`.

- on line 15:

```
# (list) Source files to include (let empty to include all the files)
source.include_exts = py,png,jpg,kv,atlas,otf,mp4
```

- on line 37:

```
# (list) Application requirements
# comma separated e.g. requirements = sqlite3,kivy
requirements = python3,kivy,ffpyplayer,ffmpeg,kivymd
```

**_Step 2: Run buildozer_**

```shell
cd wheel_wizard
buildozer init
buildozer android debug run
```

## Problems to be tackled

Add videos to the list without putting them on GitHub
