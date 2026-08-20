# 把点线面，变成 6 种海报：一套现代水墨 AI 视觉系统的完整拆解

![文章封面](images/cover-5x2.png)

> 本仓库包含 6 套完整提示词与 40 张示例图。所有提示词均可在 [`prompts/`](prompts/) 中单独复制；所有配图均位于 [`images/`](images/) 中。

最近我一直在做一个实验：如果不把“吴冠中风格”只当成一个生成关键词，而是把它拆成一套能够分析、控制和迁移的视觉语言，它能不能进入今天的海报设计？

围绕同一个视觉母体，我完成了六组作品：成语文化海报、文化视觉海报、角色视觉海报、城市文旅海报、产品宣传海报，以及不带文字的现代水墨构成插画。

这篇文章不是简单罗列六段提示词。我想从视觉原理开始，讲清楚每种形式为什么成立、该如何构图、点线面分别承担什么功能、文字放在哪里、哪些内容必须人工复核，并为每一种形式提供一条可以直接复制的提示词。

> 更准确地说，本文讨论的是“受吴冠中现代水墨视觉语言启发的 AI 海报设计”。重点是学习形式原则并创造新构图，而不是复刻某一幅具体作品。

---

## 一、这种视觉语言到底是什么？

吴冠中同时实践油画与水墨。他的重要探索之一，是将现实中的山川、江南村镇、屋宇、树木和水面，从自然形态中提炼出来，再组织成具有现代形式感的画面。

中国美术馆在《春雪》的馆藏解读中，将其语言概括为大块墨面、富有韵律的墨线和跳跃的墨点所构成的半抽象视觉意象；相关研究也强调了他在油画色彩、水墨材料、形式美和中西融合之间的持续实践。大都会艺术博物馆对《北戴河海滨》的介绍，则将其概括为由真实景观走向近乎完全抽象的构成。

把这些艺术史背景转化为今天可以操作的设计语言，我会归纳为六个词。

### 黑白灰

黑白灰不是“把彩色图调成灰色”，而是画面的骨架。黑色压住重心，灰色建立层次，白色制造空间。一张图在缩小后仍能看出清晰的黑白结构，说明它的骨架基本成立。

### 点

点是画面的节拍器。它可以是窗户、灯笼、树叶、人物、船、品牌色、印章或远处灯光。点不宜平均分布，最好有聚集、有稀疏、有停顿。彩色点通常控制在约 3%—10%。

### 线

线负责带领视线。树枝、屋檐、桥梁、水纹、道路、雨丝、衣褶和天际线，都能成为画面的运动轨迹。好的线要有快慢、粗细、断续和方向变化。

### 面

面负责稳定画面。白墙、黑瓦、山体、人物衣服、产品本体和建筑群，都可以被概括成面。如果元素过碎，画面会像素材拼贴；如果只有大面没有线和点，又会显得沉闷。

### 留白

留白不是模型“忘了生成”，而是一块被主动设计的面。它可以来自天空、水面、墙面、雾气或纯纸面。文化海报中的留白承载标题；角色海报中的留白衬托人物；纯插画中的留白形成空气与距离。

### 少量颜色

朱红、橙黄、墨绿、青灰、淡粉和湖蓝，不是为了把画面变热闹，而是为了留下记忆。颜色必须承担季节、品牌、角色识别或视线引导功能，否则就应该删掉。

---

## 二、所有类型都能使用的底层工作流

我通常先不写长提示词，而是填写一张“五问表”：

1. 唯一的视觉中心是什么？
2. 哪些东西分别承担点、线、面？
3. 最大的留白区域在哪里？
4. 唯一的主点缀色是什么？
5. 文字是画面主体、辅助信息，还是完全不要？

例如“雨中的旗袍女子”：视觉中心是撑伞女子；耳饰、花纹和远处灯光是点；雨丝、伞骨和旗袍轮廓是线；深色旗袍、灰色水面和白色天空是面；左侧留给标题；墨绿或朱红作为点缀色。

先完成这一步，再写提示词，结果会比堆砌几十个风格词稳定得多。

---

# 形式一：成语文化海报

![成语海报：一叶知秋](images/01-idiom-one-leaf-knows-autumn.png)

![成语海报：一鸣惊人](images/01-idiom-amazing-with-one-cry.png)

## 适用内容与生成逻辑

适合成语、古诗名句、校训和东方哲思主题。它的核心任务不是解释词典含义，而是把抽象语义转化为一个可以观看的场景。

先判断成语属于自然意境、精神气质、人物关系、动势变化还是抽象哲思；然后只选 2—5 个视觉元素，并确定一个核心意象。最忌讳把成语中每个字都画出来。

## 示例深拆：《一叶知秋》

这张图真正的主角不是江南建筑，而是画面中央那片正在下落的橙色叶子。

- **点**：落叶、枝头稀疏叶片、印章和远处小人物。
- **线**：右侧树干向上延伸，桥与屋檐构成横向线。
- **面**：下方白墙黑瓦构成主要黑白面，远山是浅灰面。
- **留白**：上半部暖白天空，为标题和落叶保留呼吸。
- **叙事顺序**：先看到标题，再看到落叶，最后读到江南已入秋。

这说明成语视觉化不需要直白说明。只要意象准确，留白本身就能完成叙事。

## 版式公式

> 大标题 40%＋核心意象 30%＋环境 20%＋出处与注脚 10%

标题要大而克制；出处、拼音、英文和编号只作为辅助层。AI 生成的出处、作者、英文和中文小字必须人工校对。

## 可直接复制的提示词

```text
【成语】：一叶知秋

生成1张3:4竖版现代水墨成语文化海报。先理解成语含义、情绪、典故和视觉象征，再提取2—5个代表元素，只保留一个视觉中心。本例以一片正在下落的橙色秋叶为中心，辅以稀疏枝条、江南白墙黑瓦、石桥、淡灰远山和水面。

暖白宣纸底，水墨黑、深灰和淡灰为主；树枝、屋檐、桥与水纹形成有书写感的线；窗、远人、叶片和印章形成点；白墙、黑瓦、天空与水面形成清楚的面。彩色低于5%，以橙叶作为主要记忆点。上方与左侧保留大面积留白。

加入中文主标题“一叶知秋”，大而克制；生成6—14字安静副标题；加入经过核验的出处小字、拼音或简洁英文意译。整体像收藏级成语文化海报。

避免：写实摄影、工笔画、满版古风元素、复杂国潮拼贴、高饱和色、促销字效、错误典故、伪文字、复制具体作品。
```

---

# 形式二：文化视觉海报

![文化视觉海报：昆曲](images/02-culture-kunqu.png)

![文化视觉海报：中国茶事](images/02-culture-chinese-tea.png)

## 适用内容与核心区别

适合非遗、节日、节气、戏曲、器物、展览、地方文化和生活美学。它比成语海报拥有更完整的“策展文字系统”，更接近展览海报、文化期刊封面或图录单页。

成语海报从语义出发；文化视觉海报从主题资产出发。做昆曲，可以提取水袖、戏服、头面、窗格和舞台；做中国茶事，可以提取壶、杯、茶叶、桌面和远处水乡。不要做文化百科，只保留最能代表主题的动作、器物或场景。

## 示例深拆：《昆曲》

人物位于右侧，水袖和长裙形成巨大的流动面；左侧用标题和副标题压住留白。

- **点**：头饰珠翠、梅花、朱红小字和印章。
- **线**：人物轮廓、水袖、垂绦、窗格和枝条。
- **面**：白色戏服、灰色帷幕、左下黑色舞台块面。
- **留白**：左中部为主标题区，避免文字压住人物。
- **信息层级**：中文主题最大，英文次之，日期、类别和引文最小。

系列统一来自相同纸张、灰度、字体层级和点色比例，而不是每张使用同一构图。

## 版式公式

> 文化主体 45%＋中央标题留白 30%＋边栏与图录信息 15%＋气氛细节 10%

## 可直接复制的提示词

```text
【文化主题】：昆曲

生成1张3:4竖版现代水墨文化视觉海报。提取昆曲最有识别度的水袖、戏服轮廓、头面珠翠、舞台帷幕、江南窗格和梅枝，只保留一位侧身人物作为主视觉，不做复杂剧情。

人物位于中右部，长水袖形成贯穿画面的流动线和白色大面；左中部保留稳定标题留白；左下以浓墨舞台块面压住重心。黑白灰主导，少量青绿用于戏服边缘，朱红和米金只用于头饰、梅花和编辑标记，彩色低于10%。宣纸肌理、清爽水墨晕染、干笔边缘、点线面节奏清楚。

加入中文主标题“昆曲”、小型副标题“水磨雅韵，百戏之祖”、英文“KUNQU OPERA”，以及简洁日期、系列编号和一条经核验的文化注脚。像非遗展览海报或文化图录封面。

避免：戏曲剧照、宫廷重装饰、满版信息、促销感、虚假史料、伪ISBN、过度艳丽、复制具体作品。
```

日期、农历、期号、引文、ISBN 和署名如果不是真实出版信息，不要伪装成真实资料。

---

# 形式三：角色视觉海报

![角色海报：雨中的旗袍女子](images/03-character-qipao-rain.png)

![角色海报：骑自行车的男生](images/03-character-bicycle-boy.png)

## 适用内容与角色公式

适合角色概念、小说人物、影视气质稿、IP 设定和人物主题海报。它不是传统参数式角色设定表，而是用一张海报表达人物身份与情绪。

> 身份＋动作＋标志性道具＋环境＋情绪

“一个女孩”信息太少；“雨中的旗袍女子，手持纸伞，站在江南水岸，安静回望”才形成可设计的角色。

## 示例深拆：《雨中的旗袍女子》

人物占据右侧约三分之一至二分之一，左侧完整留给标题和短句。

- **点**：耳饰、旗袍花纹、远处窗灯和红印。
- **线**：雨丝、伞骨、手臂、旗袍轮廓和岸边栏杆。
- **面**：墨绿色旗袍是最重的人物面，天空与水面组成大白面。
- **道具**：纸伞同时交代天气、地域和人物动作。
- **环境**：远处白墙黑瓦只保留轮廓，不与人物争焦点。

这类人物的脸型、五官和比例明显融合了当代唯美人物插画。更准确的说法是“现代水墨构成结合当代人物造型”。

## 版式公式

> 单一人物 50%＋环境 20%＋标题留白 20%＋中英文短句 10%

## 可直接复制的提示词

```text
【角色】：雨中的旗袍女子

生成1张3:4竖版现代水墨角色视觉海报。一位成年东方女性，穿剪裁简洁的深墨绿色旗袍，侧身站在江南河岸，手持黑色纸伞，神情安静克制。人物为唯一主角，完整或四分之三身，位于中右部；左侧保留大面积干净留白。背景只保留淡灰水面、白墙黑瓦、远船和少量树枝。

旗袍和头发形成深色块面；雨丝、伞骨、发丝、衣褶和栏杆形成流动线；耳饰、花纹、灯点和印章形成少量彩色点。黑白灰主导，墨绿为唯一主辅助色，朱红低于3%。人物轮廓清楚，但不是写实照片，也不是夸张动漫造型。

加入竖排中文角色名“雨中的旗袍女子”、英文“THE QIPAO LADY IN THE RAIN”，以及一条8—16字中文人物注脚和简短英文呼应。

避免：多人群像、时尚硬照、宫廷古装、过度性感、复杂背景、日漫大眼、商业广告感、复制具体作品。
```

---

# 形式四：城市文旅宣传海报

![城市文旅海报：上海](images/04-city-shanghai.png)

![城市文旅海报：巴黎](images/04-city-paris.png)

## 适用内容与城市分类

适合城市形象、目的地推广、城市礼物、文旅节庆和旅行内容封面。它既要有艺术性，也必须让人快速认出城市。

先判断城市属于江南水乡、现代都市、山水城市、海滨港口还是历史古都，再选择一组主要地标、一种地貌和一个生活符号。

## 示例深拆：《上海》

这张图使用东方明珠、现代高楼、外滩建筑、黄浦江与船只来建立识别度。

- **点**：红旗、塔身灯点、行人和小船。
- **线**：天际线、塔尖、桥体、道路与河岸曲线。
- **面**：建筑群是灰黑竖向面，江面和天空是大白面。
- **时间层次**：现代陆家嘴与历史建筑并置，形成“旧与新”的城市叙事。
- **标题区**：左上留白承载“上海／SHANGHAI”和城市注脚。

城市海报不是景点大全。地标越多，越容易出现比例混乱和地域错误。

## 版式公式

> 城市地标 45%＋地貌与水岸 25%＋上方留白 20%＋标题文案 10%

## 可直接复制的提示词

```text
【城市】：上海

生成1张3:4竖版现代水墨城市文旅海报。以黄浦江两岸为主题，选择东方明珠、陆家嘴天际线、外滩历史建筑、江面和一两艘小船作为主要元素，不堆满全部景点。建筑经过简洁概括，但关键地标轮廓可识别。

建筑群位于中下部，江面横向展开，上方保留大面积暖白天空作为标题区。高楼与塔尖形成竖向线，河岸和船行轨迹形成横向与弧线，窗灯、行人、船只和红旗形成小点。黑白灰主导，少量朱红、青灰和淡赭用于记忆点，彩色低于8%。宣纸肌理、墨色层次、清爽倒影，兼具东方诗意和现代秩序。

左上加入“上海”、英文“SHANGHAI”，生成一句4—12字城市短句和2—8词英文注脚。

避免：写实照片、地标大杂烩、错误建筑、虚假地图关系、高饱和夜景、赛博朋克、宣传册拼贴、复制具体作品。
```

生成后要核查地标、建筑年代、真实地域、旗帜和视角。若是诗意重组，应标注为“城市意象创作”。

---

# 形式五：产品宣传海报

![产品宣传海报：香水](images/05-product-perfume.png)

![产品宣传海报：汽车](images/05-product-mercedes.png)

## 适用内容与阅读顺序

适合品牌概念稿、产品发布视觉、东方限定包装提案、社交广告和商业插画探索。它有一个不能妥协的指标：产品识别度。

理想阅读顺序是：第一眼认出产品类别与轮廓；第二眼认出品牌资产；第三眼感受到现代水墨语言。

## 示例深拆：《香水》

方形玻璃瓶是唯一主视觉，花枝和抽象墨块只负责建立气味与空间。

- **点**：花朵、金色小方块、标签细节。
- **线**：花枝、瓶体边缘和细长垂线。
- **面**：透明瓶体、左侧留白、右下黑色墨块。
- **材质**：产品保持玻璃结构与高光，背景水墨化。若产品也完全晕染，识别度会丢失。
- **品牌色**：黑、米金和极淡粉已经足够。

汽车可用道路弧线表达速度；酒类可用杯、山水和香气线连接文化；科技产品应保留工业轮廓；咖啡使用杯、蒸汽和桌面；潮玩可略增加颜色。

## 版式公式

> 产品主体 50%＋使用／品牌意象 20%＋留白 20%＋品牌与文案 10%

## 可直接复制的提示词

```text
【产品】：极简方形香水瓶（商业使用时替换为已获授权的产品资料）

生成1张3:4竖版现代水墨产品宣传海报。一只具有清晰几何轮廓和透明玻璃质感的方形香水瓶作为唯一主视觉，位于中下部偏右；瓶盖、瓶肩、标签区和玻璃折射结构清楚。背景加入一两枝细长梅花、少量香气流线、淡灰远山和抽象墨块，但不遮挡产品。

产品本体保持精确、干净；环境使用宣纸、水墨晕染和干笔边缘。黑白灰与暖白为主，米金和淡粉只用于标签、花朵和几个小点，彩色低于7%。左上保留稳定留白，用于品牌名、产品名和一句文案。

加入已获授权且准确的Logo与产品名称；生成一句4—12字中文短句和2—8词英文短句。若无授权，使用无品牌概念产品，不生成真实Logo。

避免：错误Logo、伪包装文字、虚假功效、折扣信息、产品变形、满版花朵、厚重金色、电商主图感、复制具体作品。
```

真实品牌案例涉及商标、包装、产品外观和广告表述。正式传播前应取得授权并人工校对。

---

# 形式六：现代水墨构成插画

![现代水墨构成插画：园林](images/06-illustration-garden.png)

![现代水墨构成插画：春日河岸](images/06-illustration-spring-riverbank.png)

## 适用内容与基础作用

适合艺术挂画、文章配图、书籍内页、空间装饰、文创底图和视觉研究。它最接近纯绘画，也可以视作另外五种海报的底层母体。

它不需要主标题、英文、日期、编号或品牌。画面本身就是内容。

## 示例深拆：《园林一角》

圆形月洞门是明确的视觉中心，同时也是“框中框”。观众先看到圆，再透过门洞看到内部树木与廊架。

- **点**：嫩叶、花苞、石头墨点和栏杆节点。
- **线**：屋檐、树枝、栏杆、门洞圆弧和水面倒影。
- **面**：白墙占最大面积，太湖石形成右侧灰黑重面，水面承接倒影。
- **空间**：门洞连接前景与中景，水面拉开纵深。
- **颜色**：淡绿与极少朱红提示春意，不改变整体灰度。

纯插画最好先做黑白灰缩略图：先确定最大白面，再放一块黑色重心，用主线连接画面，最后添加彩色小点。若顺序反过来，很容易只有细节、没有结构。

## 可直接复制的提示词

```text
【主题】：春日苏州园林一角

生成1张3:4竖版现代水墨构成插画，不添加任何标题和说明文字。以一面暖白园林墙和圆形月洞门为视觉中心；透过门洞看到简化的廊架、细树和石径；右侧放置一组太湖石，前景有浅灰水面与倒影，左上有一枝向画面内部伸展的春树。

白墙、天空和水面构成大面积留白；黑色屋檐、树干和局部石块压住重心；门洞圆弧、枝条、栏杆和水纹形成方向变化的线；嫩叶、花苞和少量石点形成节奏。黑白灰主导，淡绿与极少朱红低于6%。宣纸纤维可见，墨色有浓淡，晕染清爽，干笔边缘自然，平面化但保留空间层次。

整体是一张原创现代中式艺术挂画，诗意、克制、安静、有抽象构成感。

避免：任何大标题、Logo、水印、二维码、人物大头像、工笔细描、满版景点、高饱和色、厚涂、3D、摄影感、复制具体作品。
```

---

## 三、六种形式之间是什么关系？

它们不是六种互不相干的风格，而是一棵树的六个分支：

> 现代水墨构成  
> ＋典故语义＝成语文化海报  
> ＋策展文字＝文化视觉海报  
> ＋人物主体＝角色视觉海报  
> ＋城市地标＝城市文旅海报  
> ＋产品与品牌资产＝产品宣传海报

想让系列保持一致，不必每次都画同一排白墙黑瓦。真正需要保持的是相近的黑白灰比例、纸张与笔触、点色方式、文字层级、留白意识，以及“一个画面只有一个视觉中心”的纪律。

**构图应该变化，语法应该统一。**

---

## 四、生成后必须做的人工检查

### 视觉检查

- 缩小后，黑白结构是否仍然清楚？
- 第一眼能否看到唯一主角？
- 彩色是否过多或平均散布？
- 留白是否真的参与构图？
- 枝条、屋檐和水纹是否过密？

### 内容检查

- 成语出处、古诗、作者是否准确？
- 日期、农历、节气是否准确？
- 城市地标与地理关系是否合理？
- 产品型号、Logo、包装文字是否准确？
- 英文是否自然，而不是生硬直译？

### 商业检查

- 是否拥有品牌、Logo、IP 或包装的使用权？
- 是否造成官方合作或真实广告的误解？
- 是否包含未经证实的产品功效？
- 是否过度接近某位艺术家的具体作品？

AI 负责提供构图可能性，最终的事实、文字和权利判断仍然属于创作者。

---

## 五、最后：风格不是一个名字，而是一套选择

做完这六组之后，我越来越确定：稳定的视觉风格并不来自一串永远不变的关键词。

它来自你持续作出的选择：什么必须保留，什么可以概括，什么应该删掉；什么成为点，什么成为线，什么压成面；又有哪里必须保持沉默。

当这些问题都有明确答案时，AI 生成才不再只是“抽卡”，而开始接近真正的视觉设计。

**黑白灰建立秩序，点线面制造节奏，留白提供呼吸，少量颜色留下记忆。**

这就是我把同一种现代水墨语言，转化成六种海报形式的方法。

---

## 六套完整通用提示词

以下文件均为完整版本，不是文章中的精简示例。进入文件后可点击 GitHub 的 Raw 按钮复制全文。

| 类型 | 只需填写 | 完整提示词 |
|---|---|---|
| 成语文化海报 | 成语 | [查看完整提示词](prompts/01-idiom-poster-prompt.md) |
| 文化视觉海报 | 文化主题 | [查看完整提示词](prompts/02-cultural-visual-prompt.md) |
| 角色视觉海报 | 角色 | [查看完整提示词](prompts/03-character-poster-prompt.md) |
| 城市文旅海报 | 城市 | [查看完整提示词](prompts/04-city-travel-prompt.md) |
| 产品宣传海报 | 产品 | [查看完整提示词](prompts/05-product-poster-prompt.md) |
| 现代水墨构成插画 | 主题 | [查看完整提示词](prompts/06-modern-ink-illustration-prompt.md) |

## 全部示例图库

下面收录本教程六组共 40 张示例图。点击图片可查看原图。

<details open>
<summary><strong>01｜成语文化海报（7张）</strong></summary>
<br>
<p align="center">
<a href="images/01-idiom-one-leaf-knows-autumn.png"><img src="images/01-idiom-one-leaf-knows-autumn.png" width="31%"></a>
<a href="images/01-idiom-amazing-with-one-cry.png"><img src="images/01-idiom-amazing-with-one-cry.png" width="31%"></a>
<a href="images/01-idiom-spring-breeze-success.png"><img src="images/01-idiom-spring-breeze-success.png" width="31%"></a>
</p>
<p align="center">
<a href="images/01-idiom-same-boat.png"><img src="images/01-idiom-same-boat.png" width="31%"></a>
<a href="images/01-idiom-flowing-clouds-water.png"><img src="images/01-idiom-flowing-clouds-water.png" width="31%"></a>
<a href="images/01-idiom-high-mountains-water.png"><img src="images/01-idiom-high-mountains-water.png" width="31%"></a>
</p>
<p align="center"><a href="images/01-idiom-tranquility-leads-afar.png"><img src="images/01-idiom-tranquility-leads-afar.png" width="31%"></a></p>
</details>

<details open>
<summary><strong>02｜文化视觉海报（6张）</strong></summary>
<br>
<p align="center">
<a href="images/02-culture-stage-old-dreams.png"><img src="images/02-culture-stage-old-dreams.png" width="31%"></a>
<a href="images/02-culture-dragon-boat.png"><img src="images/02-culture-dragon-boat.png" width="31%"></a>
<a href="images/02-culture-huangshan-pines.png"><img src="images/02-culture-huangshan-pines.png" width="31%"></a>
</p>
<p align="center">
<a href="images/02-culture-kunqu.png"><img src="images/02-culture-kunqu.png" width="31%"></a>
<a href="images/02-culture-old-city-gate.png"><img src="images/02-culture-old-city-gate.png" width="31%"></a>
<a href="images/02-culture-chinese-tea.png"><img src="images/02-culture-chinese-tea.png" width="31%"></a>
</p>
</details>

<details open>
<summary><strong>03｜角色视觉海报（7张）</strong></summary>
<br>
<p align="center">
<a href="images/03-character-bicycle-boy.png"><img src="images/03-character-bicycle-boy.png" width="31%"></a>
<a href="images/03-character-window-youth.png"><img src="images/03-character-window-youth.png" width="31%"></a>
<a href="images/03-character-girl-with-cat.png"><img src="images/03-character-girl-with-cat.png" width="31%"></a>
</p>
<p align="center">
<a href="images/03-character-swordsman.png"><img src="images/03-character-swordsman.png" width="31%"></a>
<a href="images/03-character-city-girl.png"><img src="images/03-character-city-girl.png" width="31%"></a>
<a href="images/03-character-boy-with-book.png"><img src="images/03-character-boy-with-book.png" width="31%"></a>
</p>
<p align="center"><a href="images/03-character-qipao-rain.png"><img src="images/03-character-qipao-rain.png" width="31%"></a></p>
</details>

<details open>
<summary><strong>04｜城市文旅海报（7张）</strong></summary>
<br>
<p align="center">
<a href="images/04-city-shanghai.png"><img src="images/04-city-shanghai.png" width="31%"></a>
<a href="images/04-city-hong-kong.png"><img src="images/04-city-hong-kong.png" width="31%"></a>
<a href="images/04-city-qingdao.png"><img src="images/04-city-qingdao.png" width="31%"></a>
</p>
<p align="center">
<a href="images/04-city-chengdu.png"><img src="images/04-city-chengdu.png" width="31%"></a>
<a href="images/04-city-new-york.png"><img src="images/04-city-new-york.png" width="31%"></a>
<a href="images/04-city-macau.png"><img src="images/04-city-macau.png" width="31%"></a>
</p>
<p align="center"><a href="images/04-city-paris.png"><img src="images/04-city-paris.png" width="31%"></a></p>
</details>

<details open>
<summary><strong>05｜产品宣传海报（7张）</strong></summary>
<br>
<p align="center">
<a href="images/05-product-mercedes.png"><img src="images/05-product-mercedes.png" width="31%"></a>
<a href="images/05-product-moutai-a.png"><img src="images/05-product-moutai-a.png" width="31%"></a>
<a href="images/05-product-perfume.png"><img src="images/05-product-perfume.png" width="31%"></a>
</p>
<p align="center">
<a href="images/05-product-popmart.png"><img src="images/05-product-popmart.png" width="31%"></a>
<a href="images/05-product-iphone.png"><img src="images/05-product-iphone.png" width="31%"></a>
<a href="images/05-product-coffee.png"><img src="images/05-product-coffee.png" width="31%"></a>
</p>
<p align="center"><a href="images/05-product-moutai-b.png"><img src="images/05-product-moutai-b.png" width="31%"></a></p>
</details>

<details open>
<summary><strong>06｜现代水墨构成插画（6张）</strong></summary>
<br>
<p align="center">
<a href="images/06-illustration-snow-roofs.png"><img src="images/06-illustration-snow-roofs.png" width="31%"></a>
<a href="images/06-illustration-spring-riverbank.png"><img src="images/06-illustration-spring-riverbank.png" width="31%"></a>
<a href="images/06-illustration-water-town.png"><img src="images/06-illustration-water-town.png" width="31%"></a>
</p>
<p align="center">
<a href="images/06-illustration-garden.png"><img src="images/06-illustration-garden.png" width="31%"></a>
<a href="images/06-illustration-white-houses.png"><img src="images/06-illustration-white-houses.png" width="31%"></a>
<a href="images/06-illustration-riverside-village.png"><img src="images/06-illustration-riverside-village.png" width="31%"></a>
</p>
</details>

## 仓库结构

```text
github-modern-ink-poster-guide/
├─ README.md
├─ images/
│  ├─ cover-5x2.png
│  └─ 40 张分类示例图
└─ prompts/
   ├─ 01-idiom-poster-prompt.md
   ├─ 02-cultural-visual-prompt.md
   ├─ 03-character-poster-prompt.md
   ├─ 04-city-travel-prompt.md
   ├─ 05-product-poster-prompt.md
   └─ 06-modern-ink-illustration-prompt.md
```

## 使用与发布说明

- 本仓库用于视觉方法研究和提示词教学，不代表与吴冠中先生、其家属、相关美术机构或示例品牌存在官方合作。
- 不直接复制具体艺术作品；请基于点线面、黑白灰、留白等一般形式原则创造新构图。
- 产品示例中的商标、Logo、包装和外观归相应权利人所有。正式商业传播前需取得授权。
- 成语出处、节气日期、城市地标、英文、产品型号和包装文字均需人工复核。
- 若公开仓库，需要自行选择适当的代码／内容许可；未获得示例图片再分发权之前，不建议添加允许商业复用图片的开放许可。

## 参考资料

- [中国美术馆：《春雪》馆藏解读](https://www.namoc.org/xwzx/zt/xj/syzr/zp/201403/t20140305_274312.htm)
- [中国美术馆：《中国现代绘画史上的吴冠中》](https://www.namoc.org/zgmsg/qknrlj/201303/48df434cd7a140c59f046d7c246d86e3.shtml)
- [大都会艺术博物馆：Robert H. Ellsworth Collection](https://www.metmuseum.org/exhibitions/listings/2001/robert-ellsworth-collection)
