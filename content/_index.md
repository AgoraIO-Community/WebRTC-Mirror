---
date: 2018-11-28T15:14:39+10:00
type: docs
weight: 1
---

## 0. 简介

这是一个由 Agora.io 提供的 `WebRTC` 镜像源，你可以使用此版本代替 Google 官方版本（只读）。

## 1. 环境配置

### 运行以下脚本，替换 git 源
```bash
git config --global user.email "<your email>"
git config --global user.name "<your name>"

git config --global url.http://120.92.49.206:3232/chromiumsrc/webrtc.git.insteadOf https://chromium.googlesource.com/external/webrtc.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/base.git.insteadOf https://chromium.googlesource.com/chromium/src/base
git config --global url.http://120.92.49.206:3232/chromiumsrc/build.git.insteadOf https://chromium.googlesource.com/chromium/src/build
git config --global url.http://120.92.49.206:3232/chromiumsrc/buildtools.git.insteadOf https://chromium.googlesource.com/chromium/src/buildtools
git config --global url.http://120.92.49.206:3232/chromiumsrc/gradle.git.insteadOf https://chromium.googlesource.com/external/github.com/gradle/gradle.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/ios.git.insteadOf https://chromium.googlesource.com/chromium/src/ios.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/testing.git.insteadOf https://chromium.googlesource.com/chromium/src/testing
git config --global url.http://120.92.49.206:3232/chromiumsrc/third_party.git.insteadOf https://chromium.googlesource.com/chromium/src/third_party
git config --global url.http://120.92.49.206:3232/chromiumsrc/clang-format.git.insteadOf https://chromium.googlesource.com/chromium/llvm-project/cfe/tools/clang-format.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libcxx.git.insteadOf https://chromium.googlesource.com/chromium/llvm-project/libcxx.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libcxxabi.git.insteadOf https://chromium.googlesource.com/chromium/llvm-project/libcxxabi.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libunwind.git.insteadOf https://chromium.googlesource.com/external/llvm.org/libunwind.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/android_ndk.git.insteadOf https://chromium.googlesource.com/android_ndk.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/android_tools.git.insteadOf https://chromium.googlesource.com/android_tools.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/auto.git.insteadOf https://chromium.googlesource.com/external/github.com/google/auto.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/catapult.git.insteadOf https://chromium.googlesource.com/catapult.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/compact_enc_det.git.insteadOf https://chromium.googlesource.com/external/github.com/google/compact_enc_det.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/colorama.git.insteadOf https://chromium.googlesource.com/external/colorama.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/depot_tools.git.insteadOf https://chromium.googlesource.com/chromium/tools/depot_tools.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/errorprone.git.insteadOf https://chromium.googlesource.com/chromium/third_party/errorprone.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/ffmpeg.git.insteadOf https://chromium.googlesource.com/chromium/third_party/ffmpeg.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/findbugs.git.insteadOf https://chromium.googlesource.com/chromium/deps/findbugs.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/freetype2.git.insteadOf https://chromium.googlesource.com/chromium/src/third_party/freetype2.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/harfbuzz.git.insteadOf https://chromium.googlesource.com/external/github.com/harfbuzz/harfbuzz.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/gtest-parallel.git.insteadOf https://chromium.googlesource.com/external/github.com/google/gtest-parallel
git config --global url.http://120.92.49.206:3232/chromiumsrc/googletest.git.insteadOf https://chromium.googlesource.com/external/github.com/google/googletest.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/icu.git.insteadOf https://chromium.googlesource.com/chromium/deps/icu.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/jsr-305.git.insteadOf https://chromium.googlesource.com/external/jsr-305.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/jsoncpp.git.insteadOf https://chromium.googlesource.com/external/github.com/open-source-parsers/jsoncpp.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/junit.git.insteadOf https://chromium.googlesource.com/external/junit.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/fuzzer.git.insteadOf https://chromium.googlesource.com/chromium/llvm-project/compiler-rt/lib/fuzzer.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libjpeg_turbo.git.insteadOf https://chromium.googlesource.com/chromium/deps/libjpeg_turbo.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libsrtp.git.insteadOf https://chromium.googlesource.com/chromium/deps/libsrtp.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libvpx.git.insteadOf https://chromium.googlesource.com/webm/libvpx.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/libyuv.git.insteadOf https://chromium.googlesource.com/libyuv/libyuv.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/linux-syscall-support.git.insteadOf https://chromium.googlesource.com/linux-syscall-support.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/mockito.git.insteadOf https://chromium.googlesource.com/external/mockito/mockito.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/nasm.git.insteadOf https://chromium.googlesource.com/chromium/deps/nasm.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/openh264.git.insteadOf https://chromium.googlesource.com/external/github.com/cisco/openh264
git config --global url.http://120.92.49.206:3232/chromiumsrc/requests.git.insteadOf https://chromium.googlesource.com/external/github.com/kennethreitz/requests.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/robolectric.git.insteadOf https://chromium.googlesource.com/external/robolectric.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/ub-uiautomator.git.insteadOf https://chromium.googlesource.com/chromium/third_party/ub-uiautomator.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/usrsctp.git.insteadOf https://chromium.googlesource.com/external/github.com/sctplab/usrsctp
git config --global url.http://120.92.49.206:3232/chromiumsrc/binaries.git.insteadOf https://chromium.googlesource.com/chromium/deps/yasm/binaries.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/patched-yasm.git.insteadOf https://chromium.googlesource.com/chromium/deps/yasm/patched-yasm.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/tools.git.insteadOf https://chromium.googlesource.com/chromium/src/tools
git config --global url.http://120.92.49.206:3232/chromiumsrc/client-py.git.insteadOf https://chromium.googlesource.com/infra/luci/client-py.git
git config --global url.http://120.92.49.206:3232/chromiumsrc/boringssl.git.insteadOf https://boringssl.googlesource.com/boringssl.git

```

### 指定同步目录
```bash
#指定当前目录为同步目录，也可以指定其他路径
export WORKSPACE=`pwd`
```

### 安装depot_tools
```bash
cd $WORKSPACE
rm -rf depot_tools && git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git

cd $WORKSPACE/depot_tools && git checkout gitlab
chmod +x $WORKSPACE/depot_tools/cipd

export PATH=$PATH:$WORKSPACE/depot_tools
```

### 同步webrtc
```bash
rm -rf $WORKSPACE/webrtc && mkdir $WORKSPACE/webrtc
cd $WORKSPACE/webrtc && gclient config --name src https://chromium.googlesource.com/external/webrtc.git@gitlab

export CDS_CLANG_BUCKET_OVERRIDE=http://120.92.49.206:3232/chromiumsrc/commondatastorage/raw/master/public/chromium-browser-clang

#cd ~/depot_tools; git fetch; git reset --hard origin/gitlab; chmod +x ~/depot_tools/cipd

cd $WORKSPACE/webrtc && gclient sync --patch-ref=https://chromium.googlesource.com/chromium/src/build.git@gitlab
```

## 2. 编译

### Linux
```bash
apt-get update
apt-get install -y g++

export PATH=$PATH:$WORKSPACE/depot_tools

cd $WORKSPACE/webrtc/src

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
cd $WORKSPACE/webrtc

#echo "target_os = [ 'android' ]" >>.gclient


# 同步
export PATH=$PATH:$WORKSPACE/depot_tools
export CDS_CLANG_BUCKET_OVERRIDE=http://120.92.49.206:3232/chromiumsrc/commondatastorage/raw/master/public/chromium-browser-clang

cd $WORKSPACE/webrtc && gclient sync --patch-ref=https://chromium.googlesource.com/chromium/src/build.git@gitlab


# 编译
cd $WORKSPACE/webrtc/src

gn gen android/Release "--args=is_debug=false target_os=\"android\" target_cpu=\"arm64\""

ninja -C android/Release
```

### iOS
```bash
export PATH=$PATH:$WORKSPACE/depot_tools

export CDS_CLANG_BUCKET_OVERRIDE=https://chromiumsrc.gitlab.io/commondatastorage/chromium-browser-clang
git.sh

# 安装depot_tools
cd $WORKSPACE
rm -rf depot_tools && git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git depot_tools

cd $WORKSPACE/depot_tools && git checkout gitlab
chmod +x $WORKSPACE/depot_tools/cipd


cd $WORKSPACE
rm -rf $WORKSPACE/webrtc && mkdir $WORKSPACE/webrtc

cd $WORKSPACE/webrtc && \
gclient config --name src https://chromium.googlesource.com/external/webrtc.git@gitlab

cd $WORKSPACE/webrtc && \
gclient sync\
 --patch-ref=https://chromium.googlesource.com/chromium/src/build.git@gitlab


sudo xcode-select -s /Applications/Xcode.app/Contents/Developer


cd $WORKSPACE/webrtc/src && \
gn gen out/Release "--args=is_debug=false"

cd $WORKSPACE/webrtc/src && \
ninja -C out/Release

```

## 3. 附录-依赖及镜像列表 

### 整个开源WebRTC编译时需要下载的依赖列表  
https://chromium.googlesource.com/chromium/src/base
https://chromium.googlesource.com/chromium/src/build
https://chromium.googlesource.com/chromium/src/buildtools
https://chromium.googlesource.com/external/github.com/gradle/gradle
https://chromium.googlesource.com/chromium/src/ios
https://chromium.googlesource.com/chromium/src/testing
https://chromium.googlesource.com/chromium/src/third_party
https://chromium.googlesource.com/chromium/llvm-project/cfe/tools/clang-format
https://chromium.googlesource.com/chromium/llvm-project/libcxx
https://chromium.googlesource.com/chromium/llvm-project/libcxxabi
https://chromium.googlesource.com/external/llvm.org/libunwind
https://chromium.googlesource.com/android_ndk
https://chromium.googlesource.com/android_tools
https://chromium.googlesource.com/external/github.com/google/auto
https://chromium.googlesource.com/catapult
https://chromium.googlesource.com/external/github.com/google/compact_enc_det
https://chromium.googlesource.com/external/colorama
https://chromium.googlesource.com/chromium/tools/depot_tools
https://chromium.googlesource.com/chromium/third_party/errorprone
https://chromium.googlesource.com/chromium/third_party/ffmpeg
https://chromium.googlesource.com/chromium/deps/findbugs
https://chromium.googlesource.com/chromium/src/third_party/freetype2
https://chromium.googlesource.com/external/github.com/harfbuzz/harfbuzz
https://chromium.googlesource.com/external/github.com/google/gtest-parallel
https://chromium.googlesource.com/external/github.com/google/googletest
https://chromium.googlesource.com/chromium/deps/icu
https://chromium.googlesource.com/external/jsr-305
https://chromium.googlesource.com/external/github.com/open-source-parsers/jsoncpp
https://chromium.googlesource.com/external/junit
https://chromium.googlesource.com/chromium/llvm-project/compiler-rt/lib/fuzzer
https://chromium.googlesource.com/chromium/deps/libjpeg_turbo
https://chromium.googlesource.com/chromium/deps/libsrtp
https://chromium.googlesource.com/webm/libvpx
https://chromium.googlesource.com/libyuv/libyuv
https://chromium.googlesource.com/linux-syscall-support
https://chromium.googlesource.com/external/mockito/mockito
https://chromium.googlesource.com/chromium/deps/nasm
https://chromium.googlesource.com/external/github.com/cisco/openh264
https://chromium.googlesource.com/external/github.com/kennethreitz/requests
https://chromium.googlesource.com/external/robolectric
https://chromium.googlesource.com/chromium/third_party/ub-uiautomator
https://chromium.googlesource.com/external/github.com/sctplab/usrsctp
https://chromium.googlesource.com/chromium/deps/yasm/binaries
https://chromium.googlesource.com/chromium/deps/yasm/patched-yasm
https://chromium.googlesource.com/chromium/src/tools
https://chromium.googlesource.com/infra/luci/client-py

### 系统官方国内镜像列表  
http://mirrors.aliyun.com/ubuntu/

### 本地镜像   
https://120.92.49.206:3232/chromiumsrc/base.git
https://120.92.49.206:3232/chromiumsrc/build.git
https://120.92.49.206:3232/chromiumsrc/buildtools.git
https://120.92.49.206:3232/chromiumsrc/gradle.git
https://120.92.49.206:3232/chromiumsrc/ios.git
https://120.92.49.206:3232/chromiumsrc/testing.git
https://120.92.49.206:3232/chromiumsrc/third_party.git
https://120.92.49.206:3232/chromiumsrc/clang-format.git
https://120.92.49.206:3232/chromiumsrc/libcxx.git
https://120.92.49.206:3232/chromiumsrc/libcxxabi.git
https://120.92.49.206:3232/chromiumsrc/libunwind.git
https://120.92.49.206:3232/chromiumsrc/android_ndk.git
https://120.92.49.206:3232/chromiumsrc/android_tools.git
https://120.92.49.206:3232/chromiumsrc/auto.git
https://120.92.49.206:3232/chromiumsrc/catapult.git
https://120.92.49.206:3232/chromiumsrc/compact_enc_det.git
https://120.92.49.206:3232/chromiumsrc/colorama.git
https://120.92.49.206:3232/chromiumsrc/depot_tools.git
https://120.92.49.206:3232/chromiumsrc/errorprone.git
https://120.92.49.206:3232/chromiumsrc/ffmpeg.git
https://120.92.49.206:3232/chromiumsrc/findbugs.git
https://120.92.49.206:3232/chromiumsrc/freetype2.git
https://120.92.49.206:3232/chromiumsrc/harfbuzz.git
https://120.92.49.206:3232/chromiumsrc/gtest-parallel.git
https://120.92.49.206:3232/chromiumsrc/googletest.git
https://120.92.49.206:3232/chromiumsrc/icu.git
https://120.92.49.206:3232/chromiumsrc/jsr-305.git
https://120.92.49.206:3232/chromiumsrc/jsoncpp.git
https://120.92.49.206:3232/chromiumsrc/junit.git
https://120.92.49.206:3232/chromiumsrc/fuzzer.git
https://120.92.49.206:3232/chromiumsrc/libjpeg_turbo.git
https://120.92.49.206:3232/chromiumsrc/libsrtp.git
https://120.92.49.206:3232/chromiumsrc/libvpx.git
https://120.92.49.206:3232/chromiumsrc/libyuv.git
https://120.92.49.206:3232/chromiumsrc/linux-syscall-support.git
https://120.92.49.206:3232/chromiumsrc/mockito.git
https://120.92.49.206:3232/chromiumsrc/nasm.git
https://120.92.49.206:3232/chromiumsrc/openh264.git
https://120.92.49.206:3232/chromiumsrc/requests.git
https://120.92.49.206:3232/chromiumsrc/robolectric.git
https://120.92.49.206:3232/chromiumsrc/ub-uiautomator.git
https://120.92.49.206:3232/chromiumsrc/usrsctp.git
https://120.92.49.206:3232/chromiumsrc/binaries.git
https://120.92.49.206:3232/chromiumsrc/patched-yasm.git
https://120.92.49.206:3232/chromiumsrc/tools.git
https://120.92.49.206:3232/chromiumsrc/client-py.git