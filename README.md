[Aurora主题](https://github.com/krsunm/Aurora)作者已经免费开放,

本人已将其经过简单修改支持前后端分离部署。

# 特性
## 原版教程 ：https://kun-pehs-organization.gitbook.io/aurora-for-v2board/
## 该版本特性：
### 前后端分离部署
### 可以独立部署到您的服务器，修改配置后将public文件夹上传到您的服务器即可
### 可以部署到cloudflare worker-site，连服务器都可以白嫖cloudflare
# 独立部署
修改index.html 配置项,配置项说明参看config.json,虽然该文件已无实际用途
```shell
  window.EnvConfig = {
    serverUrl: 'https://fkgfw.com',
    landPage: 'index',
    showRegInvite: 'show',
    appTheme: 'auto',
    appColor: 'default',
    appName: '免费机场',
    appDesc: `免费机场支持白嫖,若追求更高的品质请付费支持`,
    // appLogo: '{{ $logo }}',
    appVersion: '2.0',
    clientIOS: 'https://fkgfw.com'
    clientAndroid: 'https://fkgfw.com'
    clientWindows: 'https://fkgfw.com'
    clientMacOS: 'https://fkgfw.com'
    clientOpenwrt: 'https://fkgfw.com'
    clientLinux: 'https://fkgfw.com'
    staticUrl: '/static',
  }
```
# 部署到cloudflare worker-site
同独立部署一样修改配置项，安装wrangler

编辑wrangler.toml配置

然后
```shell
wrangler publish
```
[wrangler详细文档](https://developers.cloudflare.com/workers/wrangler/)

成果归原作者，请尊重劳动成果。

欢迎来我的[Telegram Group](https://t.me/clashcross) 闲聊