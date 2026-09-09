# Beya Photo to Paper Cover Prompt Template

Use this template with exactly one style from `style-presets.md`.

## Required Variables

- `{SIGNATURE_NAME}`: the user-provided signature name.
- `{STYLE_NUMBER}`: `1`, `2`, `3`, `4`, or `5`.
- `{STYLE_NAME}`: the selected style name.
- `{STYLE_PROMPT}`: the selected style's full preset prompt.
- `{OUTPUT_MODE}`: `1` for split photo plus illustration, or `2` for illustration only.

## Chinese Master Prompt

请基于我上传的原始照片生成成品图。输出模式为 `{OUTPUT_MODE}`。

如果输出模式是 `1`：请生成上下严格 1:1 平均分割的成品图，上半部分必须保留并呈现我上传的原始照片，像真实照片，光线自然，构图完整，质感干净舒服，不要把照片半区变成插画、滤镜或绘画；下半部分生成插画。

如果输出模式是 `2`：请只生成一张完整的 Beya 纸感封面插图，不要出现原始照片半区，不要做上下分割；原图只作为内容、构图、颜色和情绪参考。

另一半根据照片内容重新创作一张 Beya 纸感封面插图。不要照搬照片，不要简单变成线稿，不要做滤镜化处理，也不要把整张照片画成写实风景插画。请提取原图中最有识别性的主体、动作、轮廓、空间关系、重要物件和情绪，只保留最关键的视觉信息，进行高度概括和重新设计。

插画部分必须遵循 demo 的底层结构：像独立出版物里的小纸面图版，而不是完整风景画。主体应小、低、克制，通常只用 3-7 个视觉组件完成识别；使用粗糙纸张、干刷丙烯色块、断裂颗粒、不规则边缘、少量线条和大量留白。

使用第 `{STYLE_NUMBER}` 种风格：`{STYLE_NAME}`。

风格细则：

`{STYLE_PROMPT}`

签名是强制元素。请在插图半区加入清晰可见但克制的小型 Beya 手写品牌签名。不要做成普通打字 byline，也不要写成 `BY {SIGNATURE_NAME}`。不要画出波浪号、下划线符号、项目符号或单独一行圆点。

`{SIGNATURE_NAME}` 保留用户提供的写法，但呈现为手写签名。如果名字是 `beya`，请参考最新签名图的格式：白纸上的低饱和橄榄灰绿色墨迹，像中细号软笔或 brush pen 写出来，有轻微笔压变化；整体是松弛的英文小写连笔 `beya`，`b` 的起笔很高并向上伸出，字母自然连接，`y` 有明显向下的大环，`a` 之后向右拖出一条优雅长尾。长尾必须明显，比 `beya` 字母主体至少再向右延伸 60%-100% 的宽度；最右侧有一个随手点出的不规则小墨点，圆点必须远离 `a`，不能紧贴字母，不能规整得像几何圆，不能变成普通的 `beya.`。小圆点是签名尾巴的一部分，不是单独一行文字。整体 `beya` 签名更小，只占插图区域宽度约 2%-4%，固定放在插图区域右下角，并保留舒服的纸面边距。

如果名字不是 `beya`，请为这个名字设计同气质的抽象手写签名：低饱和墨色、中细号 brush pen 或铅笔墨迹、自然连笔或半连笔、松弛但高级；允许根据字母形状设计一个优雅收笔长尾或小小墨点，但不要强行模仿 `beya` 的具体字形。签名同样放在插图区域右下角，保持小而清楚、像个人品牌签名。

`2026` 作为极小手写年份放在签名附近或下方，不能用规整印刷字体。签名不能大，不能喧宾夺主，不能替换成其他标题。除非用户明确要求，不要添加其他标题、地点、短句或对象名称。

整体必须高级、清爽、干净、有留白、有呼吸感。配色要从原图中提取后重新压缩和调色，形成非常克制、非常耐看的高级色组。保留纸张颗粒、轻微涂抹痕迹、不规则边缘和手工感，避免光滑数字插画感。

不要出现手机界面、按钮、App 标签、生成记录、After 标签、水印、截图边框或任何 demo 截图里的 UI 元素。

## English Master Prompt

Create one finished image from the uploaded source photo. Output mode is `{OUTPUT_MODE}`.

If output mode is `1`: create a split image divided into two perfectly equal horizontal halves. The top half must preserve and present the uploaded original photo as a real photograph, with natural light, complete composition, clean comfortable texture, and no illustration effect. Do not turn the photo half into a filter, painting, or drawing. The bottom half is the illustration.

If output mode is `2`: create only one standalone Beya paper-cover illustration. Do not include the original photo half, and do not use a split layout. Use the uploaded photo only as the source reference for content, composition, colors, and mood.

The other half must be a newly designed Beya paper-cover illustration inspired by the photo. Do not copy the photo directly. Do not convert it into line art. Do not apply a filter. Do not redraw the whole source as a realistic scenic illustration. Extract only the most recognizable subject, action, silhouette, spatial relationship, important objects, and emotional tone, then redesign them into essential visual cues.

The illustration must follow the demo's underlying structure: an independent-publication paper plate, not a full landscape painting. Keep the subject small, low, restrained, and made from only 3-7 visual components; use rough paper, dry acrylic blocks, broken pigment, irregular edges, sparse linework, and lots of blank space.

Use style `{STYLE_NUMBER}`: `{STYLE_NAME}`.

Style details:

`{STYLE_PROMPT}`

Required signature must appear in the illustration half as a clear but restrained small Beya handwritten brand signature. Do not render it as ordinary typed byline text, do not write `BY {SIGNATURE_NAME}`, and do not draw a literal tilde, underline symbol, bullet label, or separate dot line.

Preserve the supplied spelling of `{SIGNATURE_NAME}`, but render it as a handwritten signature. If the name is `beya`, match the latest signature reference: muted olive-gray ink on white paper, medium-thin brush-pen strokes with slight pressure variation, loose lowercase cursive `beya`, a very tall rising first stroke on the `b`, relaxed connected letters, a large descending loop on the `y`, an elegant extended rightward tail after the final `a`, and a small irregular casual ink dot at the far right aligned with the tail. The rightward tail after `a` must be obviously long, extending at least 60-100% of the written word width beyond the letters, and the final dot must sit far from the `a`, not immediately after it. The dot should look like a quick imperfect ink tap, not a perfect geometric circle. Do not make the signature look like a standard cursive font or short `beya.` text. The dot is part of the signature tail, not a separate text line. Make the `beya` signature smaller than previous outputs, only about 2-4% of the illustration area width, and place it in the lower-right corner with comfortable paper margin.

If the name is not `beya`, design a custom abstract handwritten signature for the supplied name: low-saturation ink, medium-thin brush-pen or pencil-ink strokes, natural connected or semi-connected lettering, relaxed but premium rhythm, and an elegant finishing tail or subtle ink dot when the letterforms allow. Do not force the exact `beya` shape onto other names. Place the signature in the lower-right corner, small but legible, like a personal brand mark.

Place tiny handwritten `2026` near or below the signature as secondary year text, not in regular printed numerals. The signature must be small and secondary. Do not replace it with a title. Do not add any other title, location, phrase, or object name unless explicitly requested.

The whole image must feel premium, fresh, clean, restrained, breathable, and durable. Extract colors from the photo, then compress and grade them into an elegant limited palette. Preserve paper grain, slight paint smudges, irregular edges, tactile marks, and handmade imperfections. Avoid smooth generic digital illustration.

Do not include phone UI, buttons, app labels, generation-history UI, After labels, watermarks, screenshot borders, or any interface elements from the demo images.

## Universal Negative Prompt

Avoid glossy digital rendering, direct tracing, generic line-art conversion, realistic scenic painting, full-frame photo redraw, over-rendered trees/grass/buildings, phone interface elements, app UI, watermarks, labels from demo screenshots, over-detailed backgrounds, clutter, complex decorative patterns, large typography, harsh saturation, cheap pastel palette, childish cartoon style, anime style, generic sticker style, vector-logo flatness, photorealistic illustration-only mode, missing signature, typed `BY` byline text, literal tilde characters, separate dot lines, short `beya.` text when the name is beya, dot immediately after `a` when the name is beya, overly perfect round dot, oversized signature, centered signature, printed `2026`, missing long tail for beya, incorrect year text, unrelated title text, and any result where the five presets would look interchangeable.
