# android-bp-guide

A centralized documentation repository for Android.bp and Soong Blueprint.

## Start Here

If you are new to this repository, start with [soong_build.html](soong_build.html). It is the main Soong modules reference index and links each package to its available Android.bp module types.

These files are static generated HTML references. You can open any `.html` file directly in a browser; no build step or local server is required.

Recommended reading path:

1. Open [soong_build.html](soong_build.html) to find the module type you care about.
2. Jump to the linked package page, such as [cc.html](cc.html), [java.html](java.html), or [android.html](android.html).
3. Use the module anchors for direct links, for example [cc_library](cc.html#cc_library), [android_app](java.html#android_app), or [filegroup](android.html#filegroup).
4. For a specific property, use browser search in the module page or jump to anchors like [cc_library.srcs](cc.html#cc_library.srcs).

Helpful search files:

- [keywords.txt](keywords.txt): module type to property keyword map. Use it when you know a property name but not the module page.
- Browser search (`Ctrl+F` / `Cmd+F`): fastest way to find a module type or property inside a large HTML page.

Common entry points:

- Main index: [soong_build.html](soong_build.html).
- Common Android modules: [android.html](android.html), including `filegroup`, `license`, `package`, and `soong_namespace`.
- Native code: [cc.html](cc.html), [rust.html](rust.html), [bpf.html](bpf.html), and [clang.html](clang.html).
- Java and apps: [java.html](java.html), [robolectric.html](robolectric.html), and [sdk.html](sdk.html).
- Generated code and scripts: [genrule.html](genrule.html), [codegen.html](codegen.html), [python.html](python.html), [golang.html](golang.html), and [sh.html](sh.html).
- Interfaces and platform metadata: [aidl.html](aidl.html), [aidl_library.html](aidl_library.html), [hidl.html](hidl.html), [sysprop.html](sysprop.html), [vintf.html](vintf.html), and [selinux.html](selinux.html).
- Images, partitions, and prebuilts: [filesystem.html](filesystem.html), [etc.html](etc.html), [apex.html](apex.html), and [android_sdk.html](android_sdk.html).
- Vendor or MediaTek-specific modules: files named with `mtk*`, `Lib*`, `mediatek*`, or other vendor component names.

Notes:

- This repository is a reference map for module types and properties, not a step-by-step Android build tutorial.
- Module pages can be large because they include common properties, target-specific properties, and product variable variants.
- When in doubt, use [soong_build.html](soong_build.html) as the source of truth for which page owns a module type.

## 阅读入口

第一次查看这个仓库时，建议先从 [soong_build.html](soong_build.html) 开始。它是主要的 Soong 模块参考索引，可以按 package 找到对应的 Android.bp 模块类型文档。

这些文件是静态生成的 HTML 参考文档。可以直接用浏览器打开任意 `.html` 文件，不需要构建，也不需要启动本地服务。

推荐阅读路径：

1. 打开 [soong_build.html](soong_build.html)，先找到你关心的模块类型。
2. 跳到对应的 package 页面，例如 [cc.html](cc.html)、[java.html](java.html)、[android.html](android.html)。
3. 使用模块锚点直接定位，例如 [cc_library](cc.html#cc_library)、[android_app](java.html#android_app)、[filegroup](android.html#filegroup)。
4. 如果要查具体属性，可以在模块页面里用浏览器搜索，也可以直接访问类似 [cc_library.srcs](cc.html#cc_library.srcs) 这样的属性锚点。

辅助检索：

- [keywords.txt](keywords.txt)：模块类型到属性关键字的映射。知道属性名但不知道在哪个页面时，可以先查这里。
- 浏览器搜索（`Ctrl+F` / `Cmd+F`）：大页面里查模块名或属性名最快。

常用入口：

- 主索引：[soong_build.html](soong_build.html)。
- Android 通用模块：[android.html](android.html)，包括 `filegroup`、`license`、`package`、`soong_namespace` 等。
- Native 代码：[cc.html](cc.html)、[rust.html](rust.html)、[bpf.html](bpf.html)、[clang.html](clang.html)。
- Java 和应用：[java.html](java.html)、[robolectric.html](robolectric.html)、[sdk.html](sdk.html)。
- 代码生成和脚本：[genrule.html](genrule.html)、[codegen.html](codegen.html)、[python.html](python.html)、[golang.html](golang.html)、[sh.html](sh.html)。
- 接口和平台元数据：[aidl.html](aidl.html)、[aidl_library.html](aidl_library.html)、[hidl.html](hidl.html)、[sysprop.html](sysprop.html)、[vintf.html](vintf.html)、[selinux.html](selinux.html)。
- 镜像、分区和预编译文件：[filesystem.html](filesystem.html)、[etc.html](etc.html)、[apex.html](apex.html)、[android_sdk.html](android_sdk.html)。
- 厂商或 MediaTek 相关模块：文件名包含 `mtk*`、`Lib*`、`mediatek*`，或其他厂商组件名的页面。

说明：

- 这个仓库更适合作为模块类型和属性的参考地图，不是一步一步的 Android 构建教程。
- 单个模块页面可能很大，因为里面同时包含通用属性、target 相关属性和 product variable 变体。
- 不确定某个模块属于哪个页面时，优先回到 [soong_build.html](soong_build.html) 查，它是模块归属关系的总入口。
