---
title: '编译'
date: 2018-11-28T15:14:39+10:00
weight: 4
---


### Linux
```bash
apt-get update
apt-get install -y g++

export PATH=$PATH:~/depot_tools

cd ~/webrtc/src

./build/install-build-deps.sh

gn gen out/Release "--args=is_debug=false"

ninja -C out/Release

```

### Android
```bash
# 安装依赖
apt-get install -y software-properties-common
add-apt-repository -y ppa:openjdk-r/ppa

./build/install-build-deps-android.sh


# 添加安卓平台
cd ~/webrtc

#echo "target_os = [ 'android' ]" >>.gclient


# 同步
export PATH=$PATH:~/depot_tools
export CDS_CLANG_BUCKET_OVERRIDE=http://120.92.49.206:3232/chromiumsrc/commondatastorage/raw/master/public/chromium-browser-clang

cd ~/webrtc && gclient sync\
 --patch-ref=https://chromium.googlesource.com/chromium/src/build.git@gitlab


# 编译
cd ~/webrtc/src

gn gen android/Release "--args=is_debug=false target_os=\"android\" target_cpu=\"arm64\""

ninja -C android/Release
```

### iOS
```bash
export PATH=$PATH:~/depot_tools

export CDS_CLANG_BUCKET_OVERRIDE=https://chromiumsrc.gitlab.io/commondatastorage/chromium-browser-clang
git.sh

# 安装depot_tools
cd ~
rm -rf depot_tools && git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git depot_tools

cd ~/depot_tools && git checkout gitlab
chmod +x ~/depot_tools/cipd


cd ~
rm -rf ~/webrtc && mkdir ~/webrtc

cd ~/webrtc && \
gclient config --name src https://chromium.googlesource.com/external/webrtc.git@gitlab

cd ~/webrtc && \
gclient sync\
 --patch-ref=https://chromium.googlesource.com/chromium/src/build.git@gitlab


sudo xcode-select -s /Applications/Xcode.app/Contents/Developer


cd ~/webrtc/src && \
gn gen out/Release "--args=is_debug=false"

cd ~/webrtc/src && \
ninja -C out/Release

```