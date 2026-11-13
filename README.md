# 文档字体库（font library）

本目录是**中文 Office 文档排版 / 转 PDF 用的字体母本库**，收集了在 Windows 与 WPS 环境下写出来的文档实际会引用到的字体，
以及缺字体时的替代方案与踩坑记录。

> 线上仓库：<https://github.com/cheenwe/fonts>，下表每个字体都带直链
> （`https://github.com/cheenwe/fonts/raw/main/<分类>/<文件名>`，文件名含空格已转义为 `%20`）。
>
> **⚠️ 声明：本项目仅为个人学习研究目的整理收集，不做任何商业用途。所有字体版权归各自版权方所有；
> 如需商业使用，请自行向版权方获取相应商业授权。**

- 共 **135 个字体文件**，约 819MB
- 分类原则：**常用程度 + 是否需要长期保留** → 核心字体放 `01/02`，扩展放 `03~06`
- 文件名沿用 Windows / WPS 原名（部分规范化），同族多版本用后缀区分，差异见「版本取舍」

```
fonts/
├── 01-cjk-core/          中文核心                             15 个 / 220MB
├── 02-latin-core/        拉丁核心（Times/Arial/Symbol/Consolas 等） 36 个 /  14MB
├── 03-wps-builtin/       WPS 自带字体（从 macOS WPS 安装目录提取）   9 个 /  33MB
├── 04-cjk-hans-extra/    HuaWen / FangZheng / Adobe 简中扩展（含公文系列）  35 个 / 348MB
├── 05-cjk-ja-ko-hant/    日文 / 韩文 / 繁中                    10 个 / 160MB
└── 06-latin-extra/       等宽 / 混合 / 商业英文字体             30 个 /  45MB
```

---

## 01-cjk-core —— 中文核心

| 文件 | 字体家族 | 大小 | 汉字数 | 说明 |
|---|---|---|---|---|
| [SimSun.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/SimSun.ttc) | 宋体 / 新宋体 | 15.3MB | 20910 | Win7 版，最通用的宋体 |
| [simsun-Win10.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/simsun-Win10.ttc) | 宋体 / 新宋体 | 18.0MB | 20992 | Win10 版，多 82 字，度量与上者一致 |
| [SimHei.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/SimHei.ttf) | 黑体 | 9.8MB | 20902 | 全量 |
| [Kaiti.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/Kaiti.ttf) | 楷体 | 11.8MB | 20902 | 全量楷体，文档写「楷体」时用它 |
| [simkai.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/simkai.ttf) | 楷体_GB2312 | 4.1MB | 6763 | 只有 GB2312，给老文档写「楷体_GB2312」兜底 |
| [simfang.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/simfang.ttf) | 仿宋 | 10.6MB | 20902 | 全量 |
| [simsunb.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/simsunb.ttf) | SimSun-ExtB | 21.9MB | 0（纯扩展区） | 生僻字后备（U+20000 起） |
| [msyh.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyh.ttc) | 微软雅黑 / 雅黑 UI | 19.7MB | 20992 | 雅黑里覆盖最全（含 36 个 ExtB 字） |
| [msyhbd.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyhbd.ttc) | 微软雅黑 Bold | 16.9MB | 20992 | |
| [msyhl.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyhl.ttc) | 微软雅黑 Light | 12.2MB | 20992 | |
| [msyh-21m.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyh-21m.ttc) | 微软雅黑 / 雅黑 UI | 21.5MB | 20910 | 另一版本，字形相同 |
| [msyh-22m.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyh-22m.ttf) | 微软雅黑 | 21.8MB | 20909 | 单字重 TTF 版 |
| [msyh-Bold.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msyh-Bold.ttf) | 微软雅黑 Bold | 14.6MB | 20909 | 单字重 TTF 版 |
| [arialuni.ttf](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/arialuni.ttf) | Arial Unicode MS | 23.3MB | 20902 | 从 Excel / Office 导出的文档里常出现 |
| [msgothic.ttc](https://github.com/cheenwe/fonts/raw/main/01-cjk-core/msgothic.ttc) | MS Gothic / MS PGothic / MS UI Gothic | 9.2MB | 12579（日文） | 日文文档常见引用 |

> `.ttc` 是字体集合，一个文件里有多款字重/字族（如 `SimSun.ttc` = 宋体 + 新宋体；`msyh.ttc` = 雅黑 + 雅黑 UI），LibreOffice 认得。

## 02-latin-core —— 拉丁核心（36 个 / 14MB）

| 家族 | 文件 | 备注 |
|---|---|---|
| Times New Roman | [Times.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Times.ttf) · [Times Bold.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Times%20Bold.ttf) · [Times Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Times%20Italic.ttf) · [Times Bold Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Times%20Bold%20Italic.ttf) | 中文文档里最高频的英文字体 |
| Arial | [Arial.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Arial.ttf) · [Arial Bold.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Arial%20Bold.ttf) · [Arial Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Arial%20Italic.ttf) · [Arial Bold Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Arial%20Bold%20Italic.ttf) | |
| Consolas | [Consolas.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Consolas.ttf) · [Consolas Bold.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Consolas%20Bold.ttf) · [Consolas Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Consolas%20Italic.ttf) · [Consolas Bold Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Consolas%20Bold%20Italic.ttf) | Windows 等宽，文档代码块 / VBA 片段常用 |
| Courier New | [Courier New.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Courier%20New.ttf) · [Courier New Bold.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Courier%20New%20Bold.ttf) · [Courier New Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Courier%20New%20Italic.ttf) · [Courier New Bold Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Courier%20New%20Bold%20Italic.ttf) | |
| Verdana | [verdana.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/verdana.ttf) · [verdanab.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/verdanab.ttf) · [verdanai.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/verdanai.ttf) · [verdanaz.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/verdanaz.ttf) | 文档里只写 family，Bold/Italic 由渲染器自行合成 |
| Tahoma | [tahoma.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/tahoma.ttf) · [tahomabd.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/tahomabd.ttf) | |
| Georgia | [georgia.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/georgia.ttf) · [georgiab.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/georgiab.ttf) · [georgiai.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/georgiai.ttf) · [georgiaz.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/georgiaz.ttf) | |
| Palatino Linotype | [Palatino Linotype.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Palatino%20Linotype.ttf) · [Palatino Linotype Bold.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Palatino%20Linotype%20Bold.ttf) · [Palatino Linotype Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Palatino%20Linotype%20Italic.ttf) · [Palatino Linotype Bold Italic.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/Palatino%20Linotype%20Bold%20Italic.ttf) | 文档里常写作 Palatino 或 Palatino Linotype |
| Symbol | [symbol.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/symbol.ttf) | 公式、希腊字母 |
| MT Extra | [mtextra.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/mtextra.ttf) | MathType 公式对象专用符号（带 MathType 公式的 doc 必备） |
| Wingdings 1/2/3 | [wingdings.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/wingdings.ttf) · [wingdings2.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/wingdings2.ttf) · [wingdings3.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/wingdings3.ttf) | **表单里的 □ / ☑ 就是 Wingdings 2 的 `£` / `R`**，缺了会乱码 |
| Webdings | [webdings.ttf](https://github.com/cheenwe/fonts/raw/main/02-latin-core/webdings.ttf) | 装饰符号字体，偶尔被文档引用 |

## 03-wps-builtin —— WPS 自带字体（9 个 / 33MB）

来源：**`/Applications/wpsoffice.app/Contents/Resources/office6/fonts/`**（macOS 版 WPS 唯一的内置字体目录，没有用户级字体缓存目录）。
这些是 WPS 为了「用户机器上没有宋体/仿宋/楷体」时自己顶上的一套替身字体，**不是**微软原字体。

| 文件 | 家族名 | 大小 | 汉字数 | 用途 |
|---|---|---|---|---|
| [FangS-SC.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/FangS-SC.ttf) | 仿宋-简 | 13.5MB | 20976 | WPS 的仿宋替身，覆盖 GBK 全 |
| [ShuS-SC.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/ShuS-SC.ttf) | 书宋-简 | 10.7MB | 20976 | WPS 的宋体替身 |
| [HYKaiTiJ.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/HYKaiTiJ.ttf) | HanYi KaiTi Jian | 5.5MB | 6763 | 只有 GB2312 |
| [HYQiHei-55J.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/HYQiHei-55J.ttf) | HanYi QiHei-55J | 2.1MB | 6763 | 只有 GB2312 |
| [HYZhongJianHeiJ.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/HYZhongJianHeiJ.ttf) | HanYi ZhongJianHei Jian | 1.7MB | 6763 | 只有 GB2312 |
| [KingsoftMath.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/KingsoftMath.ttf) | Kingsoft Math | 156KB | — | WPS 公式对象（OMML）专用字形 |
| [KingsoftSign.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/KingsoftSign.ttf) | Kingsoft Sign | 24KB | — | WPS 电子签名对象 |
| [KingsoftExtra.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/KingsoftExtra.ttf) | Kingsoft Extra | 19KB | — | WPS 私有符号区（U+F0xx） |
| [DejaVuMathTeXGyre.ttf](https://github.com/cheenwe/fonts/raw/main/03-wps-builtin/DejaVuMathTeXGyre.ttf) | DejaVu Math TeX Gyre | 578KB | — | 数学符号 |

**使用前须知：**

1. **授权**：WPS 内置字体只授权在 WPS 内使用，复制到其他软件或服务端属于转授权，有法律风险。
2. **度量不同**：仿宋-简 / 书宋-简 的字宽与真宋体、真仿宋并不一致，在 Word 文档网格（`docGrid`）下会改变每行字数 → 可能引发多一页/少一页。
3. **覆盖不足**：三个 HanYi 字体只有 6763 字（GB2312），生僻字直接缺字。

**什么时候才需要它们**：文档里把字体名**明确写成**「仿宋-简」「书宋-简」「HanYi KaiTi Jian」时（WPS 另存过的 doc 可能出现）。

## 04-cjk-hans-extra —— 简中扩展（35 个 / 348MB）

### FangZheng 公文 / 标题系列（14 个，来自 Windows 版 WPS 自带）

> ⚠️ 本系列与 `03` 节为**商业授权字体**，家族名以拼音书写（FangZheng / HuaWen / HanYi），文件与下载链接保持原名。服务端部署前请自行确认授权范围（个人桌面使用一般无碍）。
> 「仿宋_GB2312 / 黑体 / 楷体 / 书宋 / 小标宋」是**党政公文标准字体组合**，公文类文档高频引用。

| 文件 | 家族名 | 大小 | 说明 |
|---|---|---|---|
| [FZFangSong_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZFangSong_GBK.TTF) | FangZheng FangSong_GBK | 11.7MB | 公文正文标准 |
| [FZHei_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZHei_GBK.TTF) | FangZheng HeiTi_GBK | 9.5MB | 公文一级标题 |
| [FZKai_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZKai_GBK.TTF) | FangZheng KaiTi_GBK | 13.5MB | 公文二级标题 / 批示 |
| [FZShuSong_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZShuSong_GBK.TTF) | FangZheng ShuSong_GBK | 9.5MB | 正文 / 引言 |
| [FZXiaoBiaoSong_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZXiaoBiaoSong_GBK.TTF) | FangZheng XiaoBiaoSong_GBK | 13.3MB | **公文标题标准字体** |
| [FZLiShu_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZLiShu_GBK.TTF) | FangZheng LiShu_GBK | 13.2MB | |
| [FZWeiBei_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZWeiBei_GBK.TTF) | FangZheng WeiBei_GBK | 15.6MB | |
| [FZXingKai_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZXingKai_GBK.TTF) | FangZheng XingKai_GBK | 7.4MB | |
| [FZYaoTi_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZYaoTi_GBK.TTF) | FangZheng YaoTi_GBK | 6.8MB | |
| [FZChaoCuHei_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZChaoCuHei_GBK.TTF) | FangZheng ChaoCuHei_GBK | 5.7MB | 大号标题 |
| [FZXiHeiYi_GBK.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZXiHeiYi_GBK.TTF) | FangZheng XiHeiYi_GBK | 11.1MB | |
| [FZSongS-Extended.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZSongS-Extended.TTF) | FangZheng SongTi-S ChaoDaZiFuJi | 17.2MB | GB18030 全量 |
| [FZSongS-Extended-SIP.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZSongS-Extended-SIP.TTF) | FangZheng SongTi-S ChaoDaZiFuJi (SIP) | 27.8MB | 含扩展 B/C 区（SIP 平面） |

### HuaWen 系列（11 个）

| 文件 | 家族名 | 汉字数 |
|---|---|---|
| [STSong.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STSong.TTF) | HuaWen SongTi | 20902 |
| [STKaiti.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STKaiti.TTF) | HuaWen KaiTi | 20902 |
| [STFangsong.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STFangsong.TTF) | HuaWen FangSong | 20902 |
| [STXihei.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STXihei.TTF) | HuaWen XiHei | 20902 |
| [STZhongsong.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STZhongsong.ttf) / [STZhongsong-alt.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STZhongsong-alt.TTF) | HuaWen ZhongSong | 20902 |
| [STLiti.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STLiti.TTF) | HuaWen LiShu | 6763 |
| [STXingkai.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STXingkai.TTF) | HuaWen XingKai | 6763 |
| [STXinwei.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STXinwei.TTF) | HuaWen XinWei | 6763 |
| [STCaiyun.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STCaiyun.TTF) | HuaWen CaiYun | 6763 |
| [STHupo.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/STHupo.TTF) | HuaWen HuPo | 6763 |

### 其他简中

| 文件 | 家族名 | 汉字数 |
|---|---|---|
| [Lisu.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/Lisu.TTF) | LiShu | 20902 |
| [YouYuan.TTF](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/YouYuan.TTF) | YouYuan | 20902 |
| [FZQiTi-S14S.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZQiTi-S14S.ttf) | FangZheng QiTi Jian | 6763 |
| [FZSuXinShiLiuKaiS-R-GB.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZSuXinShiLiuKaiS-R-GB.ttf) | FangZheng SuXinShiLiuKai Jian | 6763 |
| [FZZhongDengXian-Z07S.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZZhongDengXian-Z07S.ttf) | FangZheng ZhongDengXian Jian | 6763 |
| [FZYingBiXingShu-S16S.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZYingBiXingShu-S16S.ttf)（简） / [FZYingBiXingShu-S16T.ttf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/FZYingBiXingShu-S16T.ttf)（繁） | FangZheng YingBiXingShu | 6763 |

### Adobe Std（OTF/CFF，4 个）

| 文件 | 家族名 | 汉字数 |
|---|---|---|
| [Adobe Song Std.otf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/Adobe%20Song%20Std.otf) | Adobe 宋体 Std | 20910 |
| [Adobe Heiti Std.otf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/Adobe%20Heiti%20Std.otf) | Adobe 黑体 Std | 20910 |
| [Adobe Kaiti Std.otf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/Adobe%20Kaiti%20Std.otf) | Adobe 楷体 Std | 20910 |
| [Adobe Fangsong Std.otf](https://github.com/cheenwe/fonts/raw/main/04-cjk-hans-extra/Adobe%20Fangsong%20Std.otf) | Adobe 仿宋 Std | 20910 |

> ⚠️ **注意**：如果同时给某个环境配上「HuaWen SongTi → SimSun」这类字体别名，再把 `STSong.TTF` 装进去，fontconfig 会**优先精确匹配**「HuaWen SongTi」到 STSong，别名失效，字宽随之变化，可能改变分页。要装就得重新做一次分页比对。

## 05-cjk-ja-ko-hant —— 日 / 韩 / 繁（10 个 / 160MB）

| 文件 | 家族名 | 说明 |
|---|---|---|
| [YuGothR.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/YuGothR.ttc) · [YuGothM.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/YuGothM.ttc) · [YuGothB.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/YuGothB.ttc) · [YuGothL.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/YuGothL.ttc) | Yu Gothic / 游ゴシック | 日文，Win8+ 默认 |
| [malgun.ttf](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/malgun.ttf) · [malgunbd.ttf](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/malgunbd.ttf) | Malgun Gothic / 맑은 고딕 | 韩文，Win Vista+ 默认 |
| [msjh.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/msjh.ttc) · [msjhbd.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/msjhbd.ttc) · [msjhl.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/msjhl.ttc) | Microsoft JhengHei / 微軟正黑體 | 繁中 |
| [mingliub.ttc](https://github.com/cheenwe/fonts/raw/main/05-cjk-ja-ko-hant/mingliub.ttc) | MingLiU-ExtB / 細明體-ExtB | 繁中扩展区（36.8MB，含 HKSCS） |

中日韩混排文档（报关单、原产地证等）里偶尔会引用。

## 06-latin-extra —— 等宽 / 混合 / 商业英文（30 个 / 45MB）

| 文件 | 家族名 | 单独存放的原因 |
|---|---|---|
| [Arial Narrow.TTF](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Arial%20Narrow.TTF) · [Arial Narrow Bold.TTF](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Arial%20Narrow%20Bold.TTF) · [Arial Narrow Italic.TTF](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Arial%20Narrow%20Italic.TTF) · [Arial Narrow Bold Italic.TTF](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Arial%20Narrow%20Bold%20Italic.TTF) | Arial Narrow | 字体元数据 family 字段是 `Arial, Arial Narrow` → 与 Arial 混放会让 fontconfig 把「Arial」解析成 Arial Narrow |
| [Arial Black.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Arial%20Black.ttf) | Arial Black | 同上，family 含 `Arial` |
| [YaHeiConsolasHybrid-1.12-Powerline.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/YaHeiConsolasHybrid-1.12-Powerline.ttf) | YaHei Consolas Hybrid | 中文+等宽混合，Powerline 补丁版（终端/编辑器用） |
| [YaHeiConsolasHybrid-1.11b.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/YaHeiConsolasHybrid-1.11b.ttf) | YaHei Consolas Hybrid | 同上，另一版本（不带 Powerline 符号） |
| [YaHeiMono.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/YaHeiMono.ttf) | Yahei Mono | 雅黑等宽混合 |
| [Monaco.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/Monaco.ttf) | Monaco | macOS 经典等宽 |
| [VeraMono.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/VeraMono.ttf) | Bitstream Vera Sans Mono | 自由授权等宽 |
| [DejaVuSansMono.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/DejaVuSansMono.ttf) | DejaVu Sans Mono | Linux 常见等宽 |
| [SimplifiedArabic.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/SimplifiedArabic.ttf) · [SimplifiedArabic-Bold.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/SimplifiedArabic-Bold.ttf) · [SimplifiedArabicFixed.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/SimplifiedArabicFixed.ttf) | Simplified Arabic | Office 自带阿拉伯文（外贸单据偶见） |
| [TempusSansITC.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/TempusSansITC.ttf) | Tempus Sans ITC | Office 装饰字体 |
| [AGaramondPro-Regular.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/AGaramondPro-Regular.otf) · [AGaramondPro-Bold.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/AGaramondPro-Bold.otf) · [AGaramondPro-Italic.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/AGaramondPro-Italic.otf) · [AGaramondPro-BoldItalic.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/AGaramondPro-BoldItalic.otf) | Adobe Garamond Pro | 商业字体，正式文档基本不用 |
| [MinionPro-Regular.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MinionPro-Regular.otf) · [MinionPro-Bold.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MinionPro-Bold.otf) · [MinionPro-It.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MinionPro-It.otf) · [MinionPro-BoldIt.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MinionPro-BoldIt.otf) | Minion Pro | 商业字体 |
| [MyriadPro-Regular.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MyriadPro-Regular.otf) · [MyriadPro-Bold.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MyriadPro-Bold.otf) · [MyriadPro-It.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MyriadPro-It.otf) · [MyriadPro-BoldIt.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/MyriadPro-BoldIt.otf) | Myriad Pro | 商业字体 |
| [P22 Cezanne Pro.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/P22%20Cezanne%20Pro.otf) · [CopperplateGothic.otf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/CopperplateGothic.otf) · [TeX Gyre Adventor.ttf](https://github.com/cheenwe/fonts/raw/main/06-latin-extra/TeX%20Gyre%20Adventor.ttf) | 装饰字体 | |

**如果要按 family 建字体目录，Arial Narrow / Arial Black 必须单独隔离**，否则会污染 Arial 的匹配。

---

## 版本取舍（同族多版本怎么选）

| 字体 | 可选版本 | 建议 |
|---|---|---|
| 宋体 | `SimSun.ttc` 15.3MB/20910 字；`simsun-Win10.ttc` 18.0MB/20992 字 | 两者字面宽度一致，**Win10 版更全可平滑替换**；替换后最好做一次分页比对 |
| 微软雅黑 | `msyh.ttc` 19.7MB/20992（含 36 个 ExtB）> `msyh-21m.ttc` 21.5MB/20910 > `msyh-22m.ttf` 21.8MB/20909 | **用 `msyh.ttc`**，体积最小但覆盖最全 |
| 微软雅黑 Bold | `msyhbd.ttc` 16.9MB/20992（Win10）；旧版 `MSYHBD.TTC` 13.7MB 已弃 | 用 `msyhbd.ttc` |
| 楷体 | `Kaiti.ttf` 全量 20902；`simkai.ttf` 仅 6763 | 两个都留：全量给「楷体」，GB2312 给「楷体_GB2312」 |
| 宋体扩展 | `simsunb.ttf` 21.9MB（留）；旧版 14.7MB 已弃 | 用本库 21.9MB 版 |
| HuaWen ZhongSong | `STZhongsong.ttf`；`STZhongsong-alt.TTF` | 差别极小，留一份即可 |
| 雅黑混合等宽 | `YaHeiConsolasHybrid-1.12-Powerline`（终端补丁）与 `-1.11b`（无补丁） | 终端用 1.12，普通文档环境装 1.11b 即可 |

> 字体在 Linux 端是靠**字体元数据里的 family 名**匹配的，跟文件名无关（`Times.ttf` 装进去照样叫 Times New Roman）。Linux 忽略大小写，但为了可读，本目录已把 `ARIALUNI.TTF`→`arialuni.ttf`、`MSYH.ttc`→`msyh-21m.ttc` 等规范化。

## 缺失与替代策略

| 文档里的字体名 | 现状 | 替代方案 |
|---|---|---|
| Calibri | 缺 | `fonts-crosextra-carlito`（Carlito，度量完全一致，换行位置分毫不差） |
| Cambria | 缺 | `fonts-crosextra-caladea`（Caladea，度量一致） |
| PingFang SC | 缺，Apple 授权拿不到 | 别名 → Noto Sans CJK SC（思源黑体），CJK 等宽，只差字形 |
| FangZheng ShuTi | 缺 | 别名 → SimSun（艺术毛笔字，不影响分页） |
| HuaWen SongTi | 有真字体 `STSong.TTF` | 若不装真字体，别名 → SimSun；见「04」的警告 |
| 仿宋_GB2312 / 楷体_GB2312 | 有 | 别名 → `simfang.ttf` / `simkai.ttf` |
| 生僻字（U+20000 起） | 有 SimSun-ExtB | fontconfig `<edit mode="append">` 挂到宋体后；**ExtG（U+30EDE）仍缺，会显示豆腐块**；装 `FZSongS-Extended-SIP.TTF` 可覆盖 SIP 平面 |

## 常用命令

```bash
# 看某个字体名实际会命中哪个文件
fc-match "宋体"
fc-match "宋体:charset=20bb7"        # 生僻字回落检查
fc-list :charset=20bb7 family file   # 哪些字体有 这个字

# 查看字体信息（家族 / 字重 / 版本 / 字符集）
fc-query --format '%{family} | %{style} | %{fontversion}\n' SimSun.ttc
fc-query --format '%{charset}\n' SimSun.ttc   # 字符集，可统计汉字覆盖数

# 安装到用户目录（macOS）：拷贝后重启应用即可
cp 01-cjk-core/*.ttc ~/Library/Fonts/

# 安装到字体目录并刷新缓存（Linux）
cp 01-cjk-core/* /usr/share/fonts/custom/ && chmod 644 /usr/share/fonts/custom/* && fc-cache -f
```

