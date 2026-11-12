<!-- ppt-master-schema: spec-lock/v1 -->
# Execution Lock

## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## communication
- primary_language: zh-CN
- audience: 高中信息技术课堂学生（公开课听众，约 40—50 人，高一或高二）；已有基本计算机操作能力，对图像在计算机中的表示方式缺少系统理解
- objective: 讲清图像数字化的采样、量化、编码三个环节，并让学生在三次动手任务中亲自验证像素、分辨率与格式的差异，最终能估算未压缩体积并据此选择格式
- core_message: 图像进入计算机的过程就是「采样成点、量化成数、编码成文件」三步；分辨率决定细节多少，位深决定颜色多少，格式决定用什么方式压缩
- consumption_mode: balanced

## mode
- mode: custom
- mode_references: instructional
- mode_behavior: 以 instructional 的「拆解—演示—练习—检验」顺序推进全篇：每页只解决一个教学步骤，同级概念用同形同深度的直角色块卡对齐，抽象量先给具体例子再给定义；每张任务卡页固定给出目标、操作步骤、时间盒、检查点四部分；章节之间用一句话指路；页面标题直接写明本页要教会学生什么，不作修辞。

## visual_style
- visual_style: custom
- visual_style_references: pixel-art
- visual_style_behavior: 全篇严格像素网格：所有可见形体按 8px 网格对齐、轮廓为像素阶梯而非平滑曲线；分隔使用阶梯状像素条，重点概念由放大的像素精灵承载，页面四角以 HUD 式像素角括号分区，底部铺一条瓦片地脚带；只用纯色块分层表现体积（受光面在上、背光面在下），不用渐变、不用投影；标题取点阵显示气质，正文用清晰无衬线体；与软件截图对照的区域一律铺浅底面板，避免和学生看到的浅色窗口混淆。

## colors
- background: #101425
- secondary_bg: #1B2340
- primary: #4C8DFF
- accent: #FFC94A
- secondary_accent: #3ED6C0
- body_text: #EDF1FF
- secondary_text: #8FA3D9
- divider: #2A3355
- panel_light: #E8ECF5
- text_on_light: #16203A
- shade_primary: #396ABF
- shade_accent: #C0891F
- image_rendering: custom
- image_rendering_references: pixel-art
- image_rendering_behavior: 由 pixel-art 负责严格像素网格、有限色板与硬边阶梯轮廓；构图沿用经典 8-bit 取景，形体简化到低分辨率网格；不出现抗锯齿与平滑曲线；色值直接取本套课件的颜色角色，主色作画面主导、辅助色作地台、强调色只用于高亮标记，不引入第二套配色。

## typography
- font_family: Microsoft YaHei, Arial, sans-serif
- title_family: Microsoft YaHei, Arial, sans-serif
- body_family: Microsoft YaHei, Arial, sans-serif
- data_family: Consolas, Microsoft YaHei, monospace
- display: 56
- title: 42
- subtitle: 32
- lead: 30
- body: 24
- data: 22
- annotation: 18
- footnote: 16

## icons
- library: chunk-filled
- inventory: grid, dots-horizontal, square, image, images, camera, magnifying-glass, zoom-in, zoom-out, cursor-click, eyedropper, palette, droplet, circle-half, brush, layers, card-stack, file, files, file-plus, archive-box, calculator, circle-number-1, circle-number-2, circle-number-3, circle-number-4, ruler, chart-bar, chart-line, target, circle-checkmark, checkmark, square-checkmark, flag, clock, hourglass-empty, users, person, microchip, cog, lightbulb, book-open, text, table, vector-circle, vector-curve, vector-line, pencil, arrow-right, circle-info, triangle-exclamation

## images
- P01: images/cover_pixel_hero.jpg | source=ai | crop=adaptive
- P04: images/chapter_three_gates.jpg | source=ai | crop=adaptive
- P10: images/demo_photo_pixels.jpg | source=web | crop=no-crop
- P18: images/demo_photo_blocks.jpg | source=web | crop=no-crop

## page_visualizations
- P14: chart/column_chart
- P16: table/comparison_matrix

## page_rhythm
- P01: anchor
- P02: anchor
- P03: dense
- P04: anchor
- P05: breathing
- P06: dense
- P07: dense
- P08: dense
- P09: anchor
- P10: dense
- P11: dense
- P12: dense
- P13: anchor
- P14: dense
- P15: breathing
- P16: dense
- P17: anchor
- P18: dense
- P19: dense
- P20: anchor
- P21: dense
- P22: anchor

## pptx_structure
- mode: flat

## forbidden
- `mask`, `<style>`, `class`, external CSS, `<foreignObject>`, `textPath`, `@font-face`, `<animate*>`, `<set>`, `<script>` / event attributes, `<iframe>`
- HTML named entities in text; write typography as raw Unicode and escape XML reserved characters
