# 维兹真实案例图库（视觉模板参考）

> 来源：作者「维兹logo设计」视频封面图（作者作品的成品展示图，323x430）
> 用途：作为 `image_edit` 的参考图（image reference），生成 logo 时选 1-3 张最贴需求行业/手法的案例做风格对齐
> 收录日期：2026-08-28

## 极简黑白 · 高雅参考（首选，最贴作者"高雅极简"审美）

| 文件 | 品牌 | 特征 | 对应手法 |
|------|------|------|---------|
| `jingyukui.jpg` | 鲸与盔 | 黑底白形，鲸尾+头盔负形，极简高对比 | 正负形、结构共用 |
| `suzhuang.jpg` | 素妆 SUZHUANG | 篆体印章式"素"字，东方雅致 | 字体设计、国风 |
| `yinguo-jewelry.jpg` | 银国珠宝 | 菱形+G 字母组合，暗调高级感 | 字母+行业、高级感 |
| `qianhe.jpg` | QIANHE | 圆环缺口+竖形组字 Q，深浅双版本 | 字母设计、双版本 |
| `fouji-photo.jpg` | 否极摄影 | 线条构成眼/相机，大理石暗纹背景 | 线条符号化 |

## 字母/字体组合（英文 logo）

| 文件 | 品牌 | 特征 | 对应手法 |
|------|------|------|---------|
| `yubai.jpg` | 屿白 YUBAI | SB 图形标，清新自然 | 字母图形化 |
| `qinai.jpg` | 柒奈 QINAI | 艺术化 m 字，服装调性 | 单字母创意 |
| `hudai.jpg` | hudeï | 蝴蝶/花瓣双片对称，i 点爱心 | 对称造型、记忆点 |
| `grand-car.jpg` | GRAND | G+红色速度元素，汽车 | 字母+行业 |
| `bowen-bike.jpg` | BOWEN | 橙色箭头，骑行运动 | 抽象符号、行业 |
| `jy-recycle.jpg` | J&Y RECYCLE | 三互锁箭头+Y，环保回收 | 符号+字母结合 |

## 同构/结合类（行业符号融合）

| 文件 | 品牌 | 特征 | 对应手法 |
|------|------|------|---------|
| `shanhai-chazhan.jpg` | 山海茶盏 | 茶盏剪影+山形 LOGO，深蓝国风 | 行业符号结合 |
| `lemon-tea.jpg` | LEMON TEA | 柠檬+笑脸杯+吸管 | 同构、替换 |
| `lajiaoyazi.jpg` | 辣椒鸭 | 双辣椒组合造型 | 元素组合 |
| `jixieshi-repairer.jpg` | 机械师 | 扳手+摩托+齿轮 | 多元素堆砌 |
| `lanqiuji.jpg` | 篮球鸡 | 篮球纹理+鸡头/鸡冠 | 跨界同构 |
| `duolaimi-music.jpg` | 哆唻咪 | 高音谱号+数字1+吉他 | 谐音/符号 |
| `quanshijie.jpg` | 犬适界 | 狗+房屋结合 | 同构结合 |
| `xianhuashizhong.jpg` | 鲜花时钟 | 椭圆内时针+郁金香 | 元素替换 |
| `xianhua-coffee.jpg` | 鲜花咖啡 | 白色线条花朵+咖啡杯 | 元素结合 |
| `polaris.jpg` | Polaris 北极星 | 新月+北极熊剪影 | 象征元素 |
| `chimeng-music.jpg` | 驰梦音乐 | 抽象吉他 | 行业符号 |
| `mashangyouqian.jpg` | 马上有钱 | 马头+钱币菱形 | 谐音创意 |
| `shijuepingheng.jpg` | 视觉平衡术 | 猫耳/对话框+播放键 | 正负形 |
| `xiongdan.jpg` | 熊蛋 | 卡通熊抱蛋 | 卡通图形 |

## 国风/VI 应用（品牌全案）

| 文件 | 品牌 | 特征 | 对应手法 |
|------|------|------|---------|
| `jinhuamuzi.jpg` | 金华木子 | 金=屋顶造型，国风字体 | 字体设计、国风 |
| `alex-move-viapp.jpg` | Alex move | 儿童体适能 VI 全套应用 | 品牌应用展示 |
| `sienna-restaurant.jpg` | Sienna | 餐厅灯箱招牌效果 | 应用场景展示 |
| `coffee-jy.jpg` | Coffee.jy | 咖啡杯套应用 | 应用场景展示 |
| `shaoshupai.jpg` | 少数派 | 多彩抽象背景白色图标 | 对比展示 |

## 使用规则

1. **选图匹配**：先按需求行业/手法在「weizi-perspective」定决策方向，再从本目录选 1-3 张最贴的案例
2. **参考方式**：用 `image_edit`，把选中案例图作为 `image_reference_url_list` 传入，prompt 描述"参考此图的风格/手法，为[品牌]设计"
3. **高雅极简优先**：凡需求要求"高级/极简/黑白"，优先参考 `jingyukui.jpg`、`suzhuang.jpg`、`yinguo-jewelry.jpg`、`qianhe.jpg`
4. **程序化兜底**：若需精确几何（如字母完美耦合），参考这些案例的**手法**（结构共用/正负形），用程序化 SVG/几何绘制实现，文生图无法精确复现
