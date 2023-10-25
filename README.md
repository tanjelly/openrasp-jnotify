# openrasp-jnotify

一个改造过的 jnotify 版本

改造点，

1. 补全linux inotify 事件监听，使监听事件更全面
2. 支持更低版本的 linux内核
3. 支持32位linux

# BUILD

## libjnotify

以 Linux aarch64 为例。

```
cd jni/linux/Release/
make

mv libjnotify.so ../../../src/main/resources/libjnotify_arm64.so

```
**<arch> 对应关系：**
- `arm64` - Aarch64
- `64bit` - X86_64
- `32bit` - i686

## jnotify

```
mvn install
```

# NOTES

## 1.1.0

支持 Linux aarch64 架构，（注：不确定是否影响其它架构）。
