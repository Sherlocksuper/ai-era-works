# 原始提示词

对应本次归档的俯拍复刻版。视频提示词直接提取自保存的生成请求，未改写。图像编辑提示词按本次实际调用记录收录。输入说明使用素材角色描述，原始参考素材未随成片归档。

## 第一镜：楼上 Dario

图片1：换成Dario后的原片第一镜起帧；视频1：原片0–4.933333秒。

参数：`metaso` / `MiniMax-H3`，请求5秒，`768P`，`9:16`，`generateAudio: false`，模式 `["imageReference:1", "videoReference:1"]`。

```text
这是原视频人物替换的虚构恶搞影片。输出单个连续镜头，不添加切镜。@图片1是已经换好角色的镜头起帧，必须从它的构图、姿态、人物外观和光影开始；@视频1是这个镜头唯一的摄影运动和人体动作参考。把视频1的原人物换成图片1的人，保持原视频的拍摄视角、景别变化和动作节奏。真实现场光照，人物与环境自然融合，保持深蓝舞池。不要字幕、文字、水印、AI生成标签、配乐或对白。
镜头1，楼上栏杆前的Dario。保留图片1的卷发、黑框眼镜、灰色针织开衫、白色内衫和面孔。完全跟随视频1：双臂松松搭在栏杆上，开始头略朝画面左边带笑，然后视线和面孔缓缓转向下方舞池，笑意逐渐收住，神情变得认真；手臂姿态不重置。镜头在同一侧缓慢向前推进，从中近景逐步靠近面部，节奏按视频1，不提前结束表演。周围舞客和栏杆位置跟随原片。这一镜头始终只在楼上，不要切到背后或舞池。
```

## 第二镜：越肩俯看舞池，首次生成

图片1：换成Dario后的后脑起帧；图片2：肌肉梁俯拍近景起帧；视频1：原片4.933333–10.100000秒。这次中心舞者未替换成功，成片没有直接采用。

参数：`metaso` / `MiniMax-H3`，请求6秒，`768P`，`9:16`，`generateAudio: false`，模式 `["imageReference:2", "videoReference:1"]`。

```text
这是原视频人物替换的虚构恶搞影片。输出单个连续镜头，不添加切镜。@图片1是已经换好角色的镜头起帧，必须从它的构图、姿态、人物外观和光影开始；@视频1是这个镜头唯一的摄影运动和人体动作参考。把视频1的原人物换成图片1的人，保持原视频的拍摄视角、景别变化和动作节奏。真实现场光照，人物与环境自然融合，保持深蓝舞池。不要字幕、文字、水印、AI生成标签、配乐或对白。
镜头2，从Dario后脑越肩俯看楼下舞池，精确复刻视频1这个复杂机位变化。起点是图片1的后脑大近景：短卷发、灰色开衫，不露面。摄影机从他后脑上方缓缓升起并向前越过肩部，镜头向下俯，前景后脑与肩膀逐渐退到画面左下边缘，让远处楼下的拥挤舞池展开。维持二楼栏杆的观察高度，舞池从上往下看，绝不把摄影机降到楼下。沿用视频1的运动路径、遮挡消退、楼上栏杆、蓝光和下方舞客位置。舞池中心聚光灯下的原戴帽背带舞者替换为图片2里的蓝西装肌肉梁：蓝西装白衬衫，短黑发眼镜、极宽肌肉肩胸，他在原来同一位置弯膝、双手扶大腿连续跳舞；他在此镜头中应该很小，不要拉出全身大近景。前景人是Dario灰色针织开衫，不要变成长发衬衫。图片2只供楼下蓝衣人的身份外观，不要把图片2的近景机位带入这一镜。镜头结束仍是二楼高处向下俯视的舞池全景，不切到舞者近景。
```

## 第二镜：修正远景舞者，最终采用

图片1：Dario后脑起帧；图片2：将远景中心舞者换成肌肉梁后的画面；视频1：第二镜首次生成结果。

参数：`metaso` / `MiniMax-H3`，请求6秒，`768P`，`9:16`，`generateAudio: false`，模式 `["imageReference:2", "videoReference:1"]`。

```text
对@视频1进行严格的局部人物替换编辑，保持这个6秒镜头已有的相机运动、前景Dario、俯视角度、舞池背景、光照和所有其他舞客完全不变。唯一需要替换的是：楼下舞池中心圆形聚光灯下那个孤立跳舞、双腿分开双手扶大腿的灰黑衣服戴帽舞者。将他整个人换成@图片2中同一个位置的蓝西装肌肉梁。
@图片1是镜头开头Dario后脑，@图片2是镜头结尾应看到的完整舞池构图和已经换好人物的正确远景。严格让视频从图1的后脑越肩镜头连续运动到图2的俯视远景。这里图片2是远景构图参考，不要放大舞者。蓝西装白衬衫舞者始终在圆形聚光灯同一位置，体型宽厚、短黑发、眼镜，双手扶大腿弯膝跳舞，动作沿用原舞者，跟随原视频的遮挡逐渐显现。露出来的每一帧都是蓝色西装白衬衫，绝不要保留灰色帽子、灰衣或背带。不要替换旁边的其他人。
前景Dario的短卷发和灰色开衫沿用视频1，不改成长发。全程相机仍在二楼，由后脑升起越肩向下俯拍，从原来的大后脑转为舞池远景，不下降到地面。保持已有真实灯光和自然动态融合。6秒一镜到底，不添加切镜。不要文字、标签、水印、对白或音乐。
```

## 第三镜：俯拍舞者对视

图片1：换成肌肉梁后的原片第三镜起帧；视频1：原片10.100000秒至结尾。

参数：`metaso` / `MiniMax-H3`，请求5秒，`768P`，`9:16`，`generateAudio: false`，模式 `["imageReference:1", "videoReference:1"]`。

```text
这是原视频人物替换的虚构恶搞影片。输出单个连续镜头，不添加切镜。@图片1是已经换好角色的镜头起帧，必须从它的构图、姿态、人物外观和光影开始；@视频1是这个镜头唯一的摄影运动和人体动作参考。把视频1的原人物换成图片1的人，保持原视频的拍摄视角、景别变化和动作节奏。真实现场光照，人物与环境自然融合，保持深蓝舞池。不要字幕、文字、水印、AI生成标签、配乐或对白。
镜头3，最关键是始终保持图片1和视频1的俯视角度：摄影机明显高于舞者头顶，在他前上方向下斜俯拍，清楚看见头顶、双肩上表面和透视缩短的躯干、腿部。整个镜头摄影机高度与俯角基本不变，只允许原片那样很轻的靠近，绝不能下降成胸口高度的平视机位，绝不能变成仰拍。背景是俯看的深色舞池地面与周围舞客的局部，不出现平视远处的人群地平线。
主体一直是图片1的蓝西装肌肉梁，同一张脸、短黑直发、方框眼镜、极宽厚肩胸和粗壮手臂，白衬衫。完全按视频1的轻松舞蹈表演：双腿分开、微屈膝，双手沿大腿，交替换重心带动肩胯自然起伏。身体的运动有腿部承重的重量感，不是僵硬地整体左右平移。人物开始低头、略向前俯身，眼睛先往上看，在持续跳舞中下巴逐渐抬起一点，让脸迎向高处摄影机，与二楼的Dario对视；只抬到原片的角度，不把脖子向后折，不仰脸看天花板。膝盖、肩胯、手部的舞蹈动作在抬眼前后都持续，不先停住摆正姿势再抬头，不站定收尾。视线抬向上方，但相机始终俯拍。舞者一直保持在图片1同样的画面位置、大小和角度，现场顶光随体表变化，轮廓自然。
```

## 图像编辑：imagegen

四次调用均使用本地参考图片编辑，`transparent_background: false`。

### 楼上 Dario 起帧

图片1：原片第一镜起帧；图片2：Dario外观参考。

```text
Edit image1 only replacing its main man with Dario Amodei from image2, preserving image2 face, short curly hair, dark rectangular glasses, gray knitted cardigan and white V neck undershirt. Match image1 EXACT body pose, both forearms resting across metal balcony railing, hands loosely folded, head turned slightly to image-left, small amused smile, same body size, camera, lens, framing and dark blue nightclub environment, same overhead party lighting. The observer on upstairs balcony, surrounding people left alone. Natural integrated light and edges. This is a first frame for a parody video, photorealistic vertical9:16. Remove all lettering, watermarks, AI tags and labels. No added text. Keep composition otherwise unchanged.
```

### Dario 后脑起帧

图片1：原片第二镜起帧；图片2：Dario外观参考。

```text
Edit image1 as an exact composition-matching first frame for a parody movie. The back of the head and shoulder belongs to Dario Amodei (image2), with short dark curly hair and gray knitted cardigan. Preserve image1 EXACT close rear-view composition, silhouette scale, body position, nightclub lighting and blue bokeh beyond. Viewer is directly behind him on upstairs balcony; his head is large in foreground and looks down toward dancefloor beyond. No face visible, not a side view, do not turn him around. Only change long straight hair to Dario's short curls and shirt to gray knit cardigan. Keep same perspective and everything else. Photorealistic9:16 portrait, no words, logos, UI, watermark or AI labels.
```

### 肌肉梁俯拍起帧

图片1：原片第三镜起帧；图片2：蓝西装肌肉梁梗图。

```text
Edit image 1 into a photorealistic first frame for a parody video. Preserve image 1's EXACT elevated camera angle looking obliquely DOWN at the dancer, vertical 9:16 framing, lens perspective, dark blue dancefloor, surrounding dancers and overhead spotlight. Only replace the central dancer with the muscular male parody character in image 2: same face, straight black short hair, rectangular glasses, extremely broad muscular shoulders, thick chest/upper arms, cobalt blue fitted suit and open-neck white shirt. NO cap or suspenders. Pose exactly from image 1: bent knees, legs apart, both palms on upper thighs, torso slightly leaning forward, head initially down with eyes beginning to look up towards this camera ABOVE him. The TOP of his head and TOP planes of BOTH shoulders must be conspicuously visible, torso and legs foreshortened as in image 1. His chin remains modestly lowered at this starting moment. Do not change to eye-level portrait or low angle, do not put the camera in front of him at chest height. Adapt the muscular body to the original camera and pose, never adapt camera to the reference portrait. Maintain natural coherent overhead light and shadows, integrated person edges. No microphones, podium, raised finger, titles, lettering, labels, watermarks, interface or borders. Return a single 9:16 portrait image.
```

### 修正后的舞池远景参考

图片1：第二镜首次生成结果5.5秒处；图片2：蓝西装肌肉梁梗图。

```text
Precise localized edit of image1. Preserve its EXACT upstairs steep elevated viewpoint, complete crowded blue nightclub dancefloor, all background dancers, balcony and foreground blurred observer. Only replace the SMALL central spotlit dancer near the lower middle of image1, currently in gray/black, with the character in image2: exaggerated very muscular broad-shouldered man, short black hair, rectangular glasses, COBALT BLUE suit jacket, white shirt and blue trousers. His figure must remain the SAME SMALL SCALE at the exact existing dancefloor location, viewed from steeply above, bent knees, legs apart, both hands on thighs, matching the original dancer's pose and motion phase. Maintain original spotlight and contact shadow, natural perspective, skin colors appropriate to blue club lighting. No cap, no suspenders, no podium/microphones/finger gesture. Change no other person. Do not zoom, crop, change camera or make a portrait. Keep original9:16 frame. No text or labels.
```
