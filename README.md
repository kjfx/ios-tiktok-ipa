# ios tiktok ipa抓包下载，tiktok 21.1.0 ipa 旧版本历史版本下载，免拔卡解锁

### 1、下载旧版的TikTok

软件代码下载：https://kjfx.lanzoui.com/ifft01huzs1i
<br>
备用下载地址：https://github.com/kjfx/tiktok-ios-ipa/releases/download/TikTokIOS/TikTok-IOS.zip
<br><br>
美区 Apple ID 申请方法：https://github.com/kjfx/AppleID<br>
我使用的机场网址：http://www.txyun.xyz/

iTunes下载地址：[64位版下载>>](https://www.apple.com/itunes/download/win64) | [32位版下载>>](https://www.apple.com/itunes/download/win32)

<br><br><br>
<img src="https://raw.githubusercontent.com/kjfx/ios-tiktok-ipa/main/%E6%8A%93%E5%8C%85%E4%B8%8B%E8%BD%BD-%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98.jpg" />

### 2、下载 Shadowrocket<br>

### 3、在 Shadowrocket 添加配置
打开Shadowrocket → 配置 → default.conf → 编辑配置 → HTTPS解密 → 开启HTTPS解密 → 生成新的CA订书 → 生成新的CA订书 → 安装证书 → 允许 → 打开设置 → 已下载描述文件 → 安装 → 安装 → 安装 → 完成 → 通用 → 关于本机 → 证书信任设置 → 开启信任Shadowrocket证书 → 继续 → 打开Shadowrocket → 关闭 → √ → √ → 配置 → default.conf → 编辑纯文本 → 滚动条拉到最下面 <br>
在最下面粘贴以下代码：

    [URL Rewrite]
    (?<=_region=)CN(?=&) JP 307
    (?<=&mcc_mnc=)4 2 307
    ^(https?:\/\/(tnc|dm)[\w-]+\.\w+\.com\/.+)(\?)(.+) $1$3 302
    (^https?:\/\/*\.\w{4}okv.com\/.+&.+)(\d{2}\.3\.\d)(.+) $118.0$3 302

    [MITM]
    hostname = *.tiktokv.com,*.byteoversea.com,*.tik-tokapi.com
    
再点击保存。

### 4、在Shadowrocket添加节点，开启科学上网。<br>

### 5、打开TikTok App 即可实现免拔卡看，可以登录，评论。

### 如何更改国家：
默认是日本区，可以更改这行代码中的JP 【(?<=_region=)CN(?=&) JP 307】<br>
美国示例： (?<=_region=)CN(?=&) US 307<br>
英文简写 JP（日本）｜KR（韩国）｜UK（英国）｜US（美国）｜TW（中国台湾）

