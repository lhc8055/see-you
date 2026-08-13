# 第3次构建 - 2026-08-13

## 改动内容
内置18条影视/动漫规则，APP首次启动自动加载，无需手动安装

## 内置规则列表

### 影视规则 (9条)
1. 剧集屋 - jjwu9.com
2. 爱你影视 - ainivod.com
3. 蘑菇网影视 - moguvodw.com
4. 热播之家 - rebozj.pro
5. 兔陶网影视 - tutaow.com
6. 开心影院 - kxyytv.com (含验证码)
7. 太乙影视 - ww66.taiee.lol
8. 八号影视 - bahaotv.com
9. 937影视 - 937tv.vip

### 动漫规则 (9条)
1. 完美动漫 - wmdm.cc
2. 天使动漫 - tsdm.cc
3. 电影人生 - dyrsok.com
4. E站弹幕网 - ezdmw.site
5. mutedm - 91mute.com (含验证码)
6. 打驴动漫 - dalvdm.cc (含验证码)
7. 橘子动漫 - mgnacg.com (含验证码)
8. 囧次元 - jcydm.net
9. omomfun - omofun01.xyz

### 原有内置规则 (2条)
- 7sefun
- DM84

### 已排除的失效规则
- 真狼影视 (已失效)
- 影视工厂 (失效)
- 花子动漫 (失效)
- 嗷呜动漫 (失效)
- 西瓜卡通 (失效)

## 技术实现
规则文件放置在 `assets/plugins/` 目录下，APP首次启动时通过
`PluginsController.copyPluginsToExternalDirectory()` 自动加载到
`plugins.json`，用户无需手动安装任何规则。

## APK下载
- Release版 (推荐): app-release.apk (70 MB)
- Debug版: app-debug.apk (130 MB)
- GitHub Release: https://github.com/lhc8055/fy/releases/tag/v3.0

## 文件说明
- source/ - 未编译的原始源码
- apk/ - 编译好的APK安装包
  - app-release.apk - Release签名版 (推荐安装)
  - app-debug.apk - Debug调试版
