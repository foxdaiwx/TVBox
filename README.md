**所有资源均来自于各路大神无私分享，仅用于个人学习使用，严禁商用，如有侵权请联系删除。**

# Content
1. TVBOX
2. 接口源：点播接口源（多仓、单仓、单线）、直播接口源
3. TVBOX壳及魔改app（仅本人使用及市场常用和好用的）
4. Github加速网站
   
# 四、Github加速代理网站
1、镜像站与直链加速  
• <https://github.hscsec.cn/>：将 github.com 替换为该域名后可浏览与下载，适合临时访问受限或加速浏览;  
• <https://githubfast.com/>：同构镜像，用法同上，替换域名即可;  
• <https://kkgithub.com/>：镜像站，适合浏览与直链下载;  
• <https://521github.com/>：镜像站，适合浏览与直链下载;  
• <https://gitclone.com/>：支持“加速 clone”，见下文用法;  
 使用要点：在原 GitHub 链接中将域名部分替换为上述镜像域名，路径保持不变；部分站点可能不支持登录或个别功能受限。限使用Git.  

2. Git 克隆与下载加速  
• GitClone 代理克隆：将仓库地址前缀替换为 <https://gitclone.com/github.com/> 后执行克隆；首次代理克隆后会异步缓存，后续速度更快，适合 git clone 场景。  
  示例：<git clone https://gitclone.com/github.com/OWNER/REPO.git>  
• GitHub 文件/Release 加速（压缩包直下）：使用 Cloudflare Workers 反代，示例服务：<https://gh.api.99988866.xyz>、<https://g.ioiox.com>。用法：将浏览器地址栏或下载工具中的github.com 链接替换为对应反代域名即可加速 Release/Archive/项目文件 下载。  

3. Hosts 与静态资源加速
• 动态更新 Hosts：  
  • <https://hosts.gitcdn.top/>（Fetch GitHub Hosts）    
  • <https://gitlab.com/ineo6/hosts/-/raw/master/hosts>    
  将解析结果追加到本机 hosts 文件，可改善 github.com 与相关域名的连通性与速度。  
• Raw 文件加速：将 <raw.githubusercontent.com> 替换为 <raw.staticdn.net>，可加速 Raw 文件访问（适合 Markdown 中的图片、文档等）。  
• Jsdelivr CDN：适合加速 GitHub Releases 与 项目静态资源（如 JS/CSS/图片）；注意通常不提供 Release 附加的 .exe/.dmg 等二进制直链下载。   

4. 使用建议与注意事项  
• 镜像与登录限制：部分镜像站仅支持浏览/下载，无法登录 GitHub 账号（如 <hub.fastgit.org>），涉及 PR/Issue/Gist 等操作请直接使用官方站点或 Git 操作。  
• 安全性：优先使用 HTTPS；第三方镜像与反代服务可能随时变更或下线，谨慎提交账号口令与 Token，必要时使用一次性 Token 或短期凭证。  
• 稳定性：若镜像访问异常，优先切换至其他镜像或改用 Hosts/代理/GitHub CLI 等方式；下载类需求可优先用 GitClone/Release 反代。  

# 三、TVBOX壳及魔改app
1. **TVBOX** 原版、白壳、黑壳  
2. **TVBOX壳**：影视仓，公众号=派大星开发；OK影视（OK影视Pro 带弹幕功能）：公众号=OK猫开发；（其他：Fongmi影视（蜂蜜影视）、天光云影、）；    
3. **带源TVBOX app**：小苹果影视；欧歌影视；月光宝盒（Box、Max、Plus）...；  
4. **播放器**：小猫影视（全平台）；  
5. **直播**：我的电视、酷9直播、HTV直播、电视家、全网通电视、宽带直播、.....太多了，待验证；  

# 二、接口源（2025.11.11大部分内含直播接口源，但需测试期有效性）
## 1. 点播接口源：
   讴歌 或 欧歌，原始接口源：http://tv.nxog.top/m/ （单仓多线，含直播源），官网：https://欧.我爱你 （中文域名） 或 https://xn--dkw.xn--6qq986b3xl/ （中文域名对应的Punycode编码格式的ASCII码域名），包含 多仓、单仓多线路、单线路，且其接口源动态更新；内含多个工具；公众号：装歌APP，小程序：装歌API。缺点就是要看视频广告 和 不提供接口源最原始地址的链接。
### 🌹多仓
💃欧歌API：通过其接口自动链接到指定的线路（如肥猫、饭太硬、王二小放牛娃等，线路中有多个源，并可以装B个性化修改域名名字，比如“狐狸”），下文中“狐狸”为自定义的名字；  
a. [欧歌多仓，狐狸多仓]<https://xn--e5x6c.v.nxog.top/apia?id=1>，狐狸=e5x6c，字母a，序号1，（PunyCode编码，中文域名 转 ASCII码域名），  
b. [欧歌单仓，狐狸单仓]<https://xn--e5x6c.v.nxog.top/apia?id=2>，注意序号2，api后面的字母为a，  
c. [欧歌单线，单线多源]<https://xn--e5x6c.v.nxog.top/apib?id=1>，注意字母b，api后面的字母为b，  
解读：装歌APP/装歌API接口源的组成规律：装歌线路1\~装歌线路6,1=v、2=y、3=u、4=h、5=e、6=u，字母连起来=vyuheu，如上面的URL；  
多仓,apia,id=1;  单仓，apia,id=2； 单线，apib，id=1~22 (序号对应的线路如下表，只有单线才有变动的序号id），  
【序号与线路对应表】，常用id：1=饭太硬、4=肥猫、8=王二小、10=毒盒、17=巧技；  
1=饭太硬，2=光哥云盘，3=盒子迷，4=肥猫，5=潇洒改版，6=PG，7=小米，8=王二小，9=花生，10=毒盒（直播源多），11=OK，12=多多改版，13=短剧，14=老虎，15=真心，16=莱妮丝，17=巧技，18=驸马，19=VOX，20=南风，21=杰哥学习，22=网络收集不分排名；

### 🌹单仓多线
a. [欧歌单仓多线（狐狸）]<https://xn--e5x6c.v.nxog.top/apia?id=2>，（注意序号2,见前述）  
b. [茄子库]<https://700sjro44343.vicp.fun/eggp/qzku/tv.json>

### 🌹单线路（下翻，见多个大佬的列表及对应的链接URL）
a. 欧歌/装歌单线多源，原始地址：<http://tv.nxog.top/m/>，内含直播；  
b. 欧歌/装歌单线多源，装B地址URL：<https://xn--e5x6c.v.nxog.top/apib?id=1>， 饭太硬（注意api后跟字母b，序号线路对应表，狐狸=e5x6c，不支持比如🦊图标）。

🌹以下为不包含在装歌API清单中，序号也不是欧歌的ID：
1) 骚零：https://100km.top/0  （❌）
2) 摸鱼儿：http://我不是.摸鱼儿.com
3) one： https://gh-proxy.com/https:/raw.githubusercontent.com/leevi0709/one/main/jsm.json
4) 香雅情： https://gh-proxy.com/https://raw.githubusercontent.com/xyq254245/xyqonlinerule/main/XYQTVBox.json
5) 优选含2k4k: https://gitee.com/senno/tvbox/raw/master/api.json
6) 霜辉月明py：https://999740.xyz/raw.githubusercontent.com/lm317379829/PyramidStore/pyramid/py.json
7) CS含18禁：https://objectstorage.ap-melbourne-1.oraclecloud.com/n/axvdhhe2hcmn/b/tv-bucket-20250804-1124/o/cs.json
8) JJZX含18禁：https://objectstorage.ap-melbourne-1.oraclecloud.com/n/axvdhhe2hcmn/b/tv-bucket-20250804-1124/o/jjzx.json
9) 少儿教育： https://jihulab.com/ymz1231/xymz/-/raw/main/ymshaoer

## 2.直播接口源
1) 榴莲电视：<http://106.53.99.30/2025.txt>，永久免费接口，影视仓 和 OK影视，都适用；  
2) 冰茶体育：<https://bc.188766.xyz/?url=https://live.188766.xyz&mishitong=true&mima=bingchawusifengxian&haiwai=true>  （密码更新"冰茶无私奉献"，OK影视专用，影视仓 能导入但是无效）,（TG冰茶群或频道关注后，从群中获取冰茶体育密码和直播源链接），包括咪咕 咪视通 冰茶体育；区分冰茶普通链接和冰茶体育专用链接，差异为是否带“haiwai=true”，目前导入后两者无差异；  
3) Develop202：<https://gh.llkk.cc/https://raw.githubusercontent.com/develop202/migu_video/refs/heads/main/interface.txt> ，咪咕，此处使用了代理；  
4) 装歌：从装歌原始单线多远接口源 <http://tv.nxog.top/m/> 中，动态更新，获取后经常失效，不如直接适用 原始点播接口源而由其自动更新直播源；

## 3.影视壳和app、魔改、接口源、资源
1) 核心仓库，<https://github.com/CatVodTVOfficial/TVBoxOSC>, 失效；备选<https://github.com/lizhe0326/tvbox>
2) 影视仓接口源：<https://github.com/noimank/tvbox>，APK下载集合<https://github.com/youhunwl/TVAPP>，自用tvbox源分享，影视仓多仓源分享，tvbox相关资源记录：
3) APK下载集合：<https://github.com/youhunwl/TVAPP>, 收集全网 Android TV电视盒子应用，涵盖影视、直播、K歌、工具、游戏等类型，整理优质APK资源，支持便捷下载与自动更新。提供安全验证、分类索引与兼容性标注，助力用户打造家庭影音娱乐中心！ ✅ TVBox/影视仓等影音壳接口配置源

# 一、TVBox
1. 全版本介绍：
（1）https://zhuanlan.zhihu.com/p/608959171 
（2）https://github.com/pymond/tvbox/blob/main/README.md
2. 下载链接 夸克网盘： https://pan.quark.cn/s/cf81a27a7439  （更新日期：2023.8.17）
3. 再介绍：
（1）https://uzbox.com/app/tvbox.html， 
（2）https://uzbox.com/tech/tvbox-jiekou.html，
（3）https://raw.liucn.cc/box/

5. 纯净版q215613905：Q版、俊版、简洁版本 
6. 美化版takagen99：下载地址https://github.com/o0HalfLife0o/TVBoxOSC/releases，出处：takagen99
7. 多仓版：影视仓，寻找同名的微信公众号，作者：安卓开发哥，V3支持低版本的Android4.0
8. 手机版：竖版EasyBox

9. 接口：
（1）https://www.lige.fit/ ，
（2）https://raw.liucn.cc/box/dm.txt
（3）https://www.juwanhezi.com/other/jsonlist （聚玩盒子，单仓、多仓、数据源平台）

11. 几个魔改版的公众号：影视仓、码上放生、时光机、安卓开发哥等 
