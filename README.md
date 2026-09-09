# Beya Photo to Paper Cover Skill

## 中文说明

这是一个用于 Codex 的 Beya 风格图片生成 skill。它可以把用户上传的照片，转换成安静、克制、有纸张肌理的手绘封面插图，也可以生成“上半部分原图 + 下半部分插画”的对照图。

这个 skill 的重点不是把照片照搬成写实插画，而是提取照片里最有辨识度的主体、轮廓、动作、空间关系和情绪，再重新设计成极简纸感图版。画面通常会保留大量留白，使用低饱和高级配色、粗糙纸张纹理、干刷丙烯色块、手绘线条和轻微的不规则边缘。

### 使用时会询问三个内容

1. 署名名字  
   输入你希望出现在作品右下角的签名名字。

2. 风格编号  
   从 `1` 到 `5` 选择一种风格。

3. 输出模式  
   输入 `1`：生成上下 1:1 分割图，上半部分是原始照片，下半部分是插画。  
   输入 `2`：只生成一张完整插画，不包含原始照片。

### 五种风格

1. Quiet Geometry Poster  
   极简几何画报风，适合风景、建筑、道路、山林、草地等画面。

2. Still Object Collage  
   静物解构拼贴风，适合物件、建筑、植物、餐桌、空间局部等画面。

3. Wax Pencil Keepsake  
   蜡笔手记风，适合食物、小物件、宠物、花、纪念品和亲密日常。

4. Coastal Postmark Print  
   旅行邮戳版画风，适合灯塔、海岸、城市角落、地标、交通工具和强轮廓主体。

5. Pastoral Washbook  
   田园水彩绘本风，适合动物、人物、自然、乡村、花园和温柔生活场景。

### 安装方式

把 `beya-photo-to-paper-cover` 文件夹复制到你的 Codex skills 目录：

```bash
~/.codex/skills/beya-photo-to-paper-cover
```

然后在 Codex 里使用：

```text
Use $beya-photo-to-paper-cover
```

### 包含内容

- `beya-photo-to-paper-cover/`：Codex skill 本体
- `beya-photo-to-paper-cover/references/`：提示词模板和五种风格参数
- `palette/`：Beya 纸感插画配色色板

### 设计原则

这个 skill 会尽量避免写实重绘、普通线稿转换、滤镜感和过度细节。理想效果是一张像独立出版物封面、旅行手记内页、自然观察册或安静小绘本里的纸面插图。

---

## English Guide

This is a Beya-style image generation skill for Codex. It turns uploaded photos into quiet, restrained, paper-textured hand-drawn cover illustrations. It can also create a split comparison image with the original photo on top and the generated illustration below.

The goal is not to copy the photo as a realistic illustration. Instead, the skill extracts the most recognizable subject, silhouette, action, spatial relationship, and mood from the source image, then redesigns them into a minimal paper artwork. The result should feel airy and editorial, with generous negative space, muted premium colors, rough paper grain, dry acrylic blocks, hand-drawn lines, and slightly irregular handmade edges.

### The Skill Asks For Three Inputs

1. Signature name  
   Enter the name you want to appear as the small signature in the lower-right corner.

2. Style number  
   Choose one style from `1` to `5`.

3. Output mode  
   Enter `1` for a split 1:1 image: original photo on top, illustration below.  
   Enter `2` for illustration-only output.

### Five Styles

1. Quiet Geometry Poster  
   A minimalist geometric poster style for landscapes, architecture, roads, forests, fields, and quiet scenic compositions.

2. Still Object Collage  
   A deconstructed still-object collage style for objects, architecture, plants, table scenes, and spatial details.

3. Wax Pencil Keepsake  
   A warm wax-pencil diary style for food, small objects, pets, flowers, souvenirs, and intimate everyday moments.

4. Coastal Postmark Print  
   A vintage travel postcard print style for lighthouses, coastlines, city corners, landmarks, vehicles, and strong silhouettes.

5. Pastoral Washbook  
   A soft pastoral watercolor/gouache picture-book style for animals, people, gardens, countryside, nature, and gentle life scenes.

### Installation

Copy the `beya-photo-to-paper-cover` folder into your Codex skills directory:

```bash
~/.codex/skills/beya-photo-to-paper-cover
```

Then invoke it in Codex with:

```text
Use $beya-photo-to-paper-cover
```

### Included

- `beya-photo-to-paper-cover/`: the Codex skill
- `beya-photo-to-paper-cover/references/`: prompt template and five style presets
- `palette/`: Beya paper-cover color palette references

### Design Notes

This skill is designed to avoid realistic redraws, plain line-art conversion, filter-like effects, and over-rendered details. The ideal output should feel like a small independent-publishing cover, a travel journal page, a natural observation notebook, or a quiet picture-book plate.
