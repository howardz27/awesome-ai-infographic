<div>
  <p align="center">
    <img src="assets/logo.png" width="128" height="128" alt="AI 信息图资源精选标志">
  </p>
  <h1>AI 信息图资源精选 <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a></h1>
</div>

> AI 信息图资源精选，涵盖生成工具、Agent Skills、模型、论文，以及可嵌入信息图的图表与图解。

[English](README.md) · 简体中文

各小节按条目标注的第一个日期从新到旧排列。日期注明对应事件，例如仓库创建、版本发布、论文发表或文件首次提交。未公开日期的条目排在最后。GitHub Star 数（⭐️）采集于 2026-11-24。

## 目录

- [按用途选方案](#按用途选方案)
- [完整信息图生成项目](#完整信息图生成项目)
- [信息图 Agent 技能](#信息图-agent-技能)
- [信息图渲染引擎](#信息图渲染引擎)
- [可下载模型](#可下载模型)
- [图表与图解组件](#图表与图解组件)
- [在线工具](#在线工具)
- [研究论文与评测](#研究论文与评测)
- [教程与设计指南](#教程与设计指南)

## 按用途选方案

根据你要做的内容和希望怎样修改成品，选择合适的方案。

**编辑文字和对象**。Editable Design 提供可视化编辑器，Paper2Poster 输出可编辑 PPTX，AntV Infographic 渲染可编辑的模板化 SVG。

**修改 HTML、CSS 或 SVG 源码**。Epic Infographics 适合完整构图，Guizang Social Card Skill 适合社交媒体多页图文。

**直接生成位图**。baoyu-infographic 组织提示词并调用生图工具，SenseNova-U1 Infographic V3 提供针对信息图训练的可下载权重。

**从数据生成图表，或从文字生成图解**。Flint 和 Data Formulator 使用结构化数据，Diagram Design 输出 HTML/SVG，Next AI Draw.io 可编辑 draw.io 图解。

**直接在浏览器里生成**。Piktochart AI 生成可编辑草稿，Gemini Notebook 根据来源文档生成视觉摘要。

**评估生成质量**。IGenBench 核验内容与数据编码，InfoEdit 评估编辑后布局如何变化。

## 完整信息图生成项目

从文字、数据或文档出发，制作整张信息图或海报。部分项目支持输出可编辑的 HTML 或 PowerPoint。

- [Editable Design](https://github.com/yejy53/Editable-Design) - **创建于 2026-08-24 · ⭐️ 1,272**<br>
  用编程智能体生成信息图和海报，保留可编辑文本和独立素材，提供可视化编辑器，并可将兼容设计导出为可编辑 PPTX。
- [AesCode](https://github.com/microsoft/AesCode) - **创建于 2026-07-23 · ⭐️ 285**<br>
  用生成图像提供设计参考，再编写可编辑的 HTML/CSS，并针对浏览器渲染结果检查内容与设计。
- [Paper2Poster](https://github.com/Paper2Poster/Paper2Poster) - **创建于 2025-05-16 · ⭐️ 4,055**<br>
  从论文 PDF 提炼内容、复用原论文插图，再排版成可编辑的学术海报 PPTX。
- [LIDA](https://github.com/microsoft/lida) - **创建于 2023-03-09 · ⭐️ 3,299**<br>
  从表格数据提取摘要和可视化目标并生成图表代码，可进一步用生图模型对渲染结果做风格化。

## 信息图 Agent 技能

把这些技能加载到兼容的 AI 助手中，让它按步骤提炼内容、选择布局，再调用 HTML 渲染或生图工具。

- [Epic Infographics](https://github.com/OrRon/EpicInfographics) - **创建于 2026-08-23 · ⭐️ 502**<br>
  以场景为构图单位的 HTML/CSS 信息图技能，包含数据驱动的图形尺寸计算、渲染检查和 PNG 导出，并支持动态版本。
- [Guizang Social Card Skill](https://github.com/op7418/guizang-social-card-skill) - **创建于 2026-05-27 · ⭐️ 8,244**<br>
  生成单文件 HTML 的小红书图文轮播和微信公众号封面对，并用 Playwright 导出 PNG。
- [Visual Explainer](https://github.com/nicobailon/visual-explainer) - **创建于 2026-02-16 · ⭐️ 11,253**<br>
  生成自包含 HTML 解释页的 Agent Skill，适合组合技术图解、对比表格与项目概览。
- [baoyu-infographic](https://github.com/JimLiu/baoyu-skills/blob/main/skills/baoyu-infographic/SKILL.md) - **首次提交于 [2026-01-20](https://github.com/JimLiu/baoyu-skills/blob/b30dcca67e47ed269683f706489e782adee3de04/skills/baoyu-infographic/SKILL.md) · 仓库创建于 2026-01-13 · ⭐️ 27,853**<br>
  先重组原始内容，再搭配信息布局与视觉风格，最后调用生图工具输出 PNG 的 Agent Skill。

## 信息图渲染引擎

可集成到应用中的渲染代码，接收结构化数据和布局配置，输出 SVG 等可展示的信息图。

- [AntV Infographic](https://github.com/antvis/Infographic) - **创建于 2025-09-11 · ⭐️ 7,157**<br>
  通过面向大模型的声明式语法生成和流式渲染模板化 SVG 信息图，自带编辑器。

## 可下载模型

下载模型权重，在自己的工作流中运行。这里标注的是权重许可，访问条件及代码、数据集的独立许可可查阅模型卡。

### 信息图专用模型

面向整图构图、密集文字排版或可编辑 HTML/CSS 生成等信息图任务训练的模型。

- [AesCode 8B and 32B](https://huggingface.co/microsoft/AesCode-8B) - **发布于 [2026-10-14](https://huggingface.co/microsoft/AesCode-8B/commits/main) · Hub 创建于 2026-09-29** Apache-2.0。根据提示词与可选参考图，为海报、幻灯片和仪表板生成可编辑的 HTML/CSS。[32B 权重](https://huggingface.co/microsoft/AesCode-32B) (发布于 [2026-10-14](https://huggingface.co/microsoft/AesCode-32B/commits/main) · Hub 创建于 2026-09-29)。
- [SenseNova-U1 Infographic V3](https://huggingface.co/sensenova/SenseNova-U1-8B-MoT-Infographic-V3) - **发布于 [2026-07-16](https://github.com/OpenSenseNova/SenseNova-U1#news) · Hub 创建于 2026-07-15** Apache-2.0。针对信息图微调的多模态模型，支持文生图和基于指令的位图编辑。
- [BizGen](https://huggingface.co/PYY2001/BizGen) - **Hub 创建于 2025-03-24** 模型卡标注 Apache-2.0。基于 SDXL 的权重，根据给定布局渲染信息图和幻灯片中按区域指定的密集文字。

### 生图与图层编辑模型

用于生成位图信息图和插画、修改已有图片，或把一张图片拆成可独立处理的图层。

- [Ideogram 4](https://huggingface.co/ideogram-ai/ideogram-4-nf4) - **发布于 [2026-06-03](https://ideogram.ai/news/ideogram-4.0/) · Hub 创建于 2026-05-30** Ideogram 4 非商业许可，访问 NF4 权重需接受访问条款。支持位图生成与编辑、区域控制和多语言文字渲染。
- [FLUX.2 klein 4B](https://huggingface.co/black-forest-labs/FLUX.2-klein-4B) - **发布于 [2026-01-15](https://bfl.ai/blog/flux2-klein-towards-interactive-visual-intelligence) · Hub 创建于 2026-01-14** Apache-2.0。较轻量的通用生图与图像编辑模型，可用于生成插画素材或基于参考图迭代。
- [GLM-Image](https://huggingface.co/zai-org/GLM-Image) - **公布于 [2026-01-13](https://www.zhipuai.cn/zh/research/158) · Hub 创建于 2026-01-08** MIT。重视文字渲染的生图和图像编辑模型，模型卡包含知识型视觉示例。
- [Qwen-Image-Layered](https://huggingface.co/Qwen/Qwen-Image-Layered) - **发布于 [2025-12-19](https://github.com/QwenLM/Qwen-Image/blob/main/README.md) · Hub 创建于 2025-12-17** Apache-2.0。把一张图片拆成多个 RGBA 位图图层，各图层可单独移动或替换。
- [Z-Image-Turbo](https://huggingface.co/Tongyi-MAI/Z-Image-Turbo) - **发布于 [2025-11-26](https://github.com/Tongyi-MAI/Z-Image#news) · Hub 创建于 2025-11-25** Apache-2.0。蒸馏版生图模型，模型卡提供中文和英文文字渲染示例。
- [Qwen-Image](https://huggingface.co/Qwen/Qwen-Image) - **发布于 [2025-08-04](https://qwenlm.github.io/blog/qwen-image/) · Hub 创建于 2025-08-02** Apache-2.0。生图模型，模型卡展示了海报和视觉排版中的密集中文、英文文字。

## 图表与图解组件

制作可放进信息图的单个组件，例如数据图表、流程图和科研插图。

### 数据图表

从数据生成图表，从截图复刻图表，或把 AI 生成的图表配置嵌入应用。

- [Flint](https://github.com/microsoft/flint-chart) - **创建于 2026-05-13 · ⭐️ 4,605**<br>
  提供精简的图表语言和 MCP 接入，可将人可编辑的规范编译为 Vega-Lite、ECharts、Chart.js、Plotly 或可编辑的 Excel 图表。
- [AntV MCP Server Chart](https://github.com/antvis/mcp-server-chart) - **创建于 2025-04-25 · ⭐️ 4,423**<br>
  通过 MCP 工具和技能，根据结构化参数生成常用统计图表与部分图解。
- [ChartCoder](https://github.com/thunlp/ChartCoder) - **创建于 2025-01-14 · ⭐️ 81**<br>
  把图表截图转成可编辑绘图代码的专用模型，作者提供可下载权重。
- [Data Formulator](https://github.com/microsoft/data-formulator) - **创建于 2024-06-07 · ⭐️ 17,696**<br>
  支持自然语言数据变换和迭代式图表编写的交互式 AI 数据分析工具。
- [GPT-Vis](https://github.com/antvis/GPT-Vis) - **创建于 2023-11-13 · ⭐️ 807**<br>
  渲染 AI 生成的图表配置，提供可嵌入网页应用的可视化组件。

### 图解与科研插图

把文字描述或科研材料转换为流程图、系统架构图和科研插图等视觉内容。

- [Diagram Design](https://github.com/cathrynlavery/diagram-design) - **创建于 2026-04-16 · ⭐️ 71,452**<br>
  用单文件 HTML 和内嵌 SVG 生成流程、对比和系统架构图的 Agent Skill。
- [PaperBanana](https://github.com/llmsresearch/paperbanana) - **创建于 2026-02-04 · ⭐️ 2,506**<br>
  PaperBanana 论文的社区实现，根据方法描述和图注生成科研示意图与数据图。
- [AutoFigure-Edit](https://github.com/ResearAI/AutoFigure-Edit) - **创建于 2026-02-03 · ⭐️ 4,429**<br>
  从长篇技术文本及参考风格生成科研插图，包含原生 SVG 编辑步骤。
- [draw.io MCP](https://github.com/jgraph/drawio-mcp) - **创建于 2026-02-02 · ⭐️ 5,892**<br>
  draw.io 官方工具，可接收 AI 生成的图解，并将 Mermaid 转为含可编辑形状和连线的 draw.io 图。
- [CanvasAnvil](https://github.com/CodingFeng101/CanvasAnvil) - **创建于 2026-01-24 · ⭐️ 226**<br>
  可自托管的 AI 图解编辑器，支持无限画布和可编辑的 draw.io 文件。
- [Next AI Draw.io](https://github.com/DayuanJiang/next-ai-draw-io) - **创建于 2025-03-23 · ⭐️ 37,154**<br>
  通过对话创建和修改 draw.io 图解，提供 Web、桌面和 MCP 入口。

### 图表与图解渲染库

把 AI 生成的图表配置或图解语法渲染成可嵌入或导出的图形。

- [Vega-Lite](https://github.com/vega/vega-lite) - **创建于 2014-11-20 · ⭐️ 5,562**<br>
  以 JSON 声明数据编码、图层组合和交互方式的可视化语法。
- [Mermaid](https://github.com/mermaid-js/mermaid) - **创建于 2014-11-01 · ⭐️ 91,221**<br>
  通过文本语法渲染流程图、时序图、时间线等结构化图解。
- [Apache ECharts](https://github.com/apache/echarts) - **创建于 2013-04-03 · ⭐️ 67,788**<br>
  用 JavaScript 配置对象渲染交互式网页图表，支持 SVG 和 Canvas。

## 在线工具

直接在浏览器中制作整张信息图，或生成可放进信息图的素材。

### 信息图与图解制作工具

把提示词、文档或选中的段落转换为信息图、图解或矢量素材。编辑和导出能力因工具而异。

- [AntV Infographic AI Demo](https://infographic.antv.vision/ai) - **首次提交于 [2025-11-21](https://github.com/antvis/Infographic/blob/3bae7c338c60108fbfba0fe93cfa26e2c0b1c67d/site/src/pages/ai.tsx)** 可交互体验 AntV 信息图生成流程，并查看渲染效果。
- [Gemini Notebook (NotebookLM)](https://support.google.com/gemininotebook/answer/16758265?hl=en) - **发布于 [2025-11-20](https://workspaceupdates.googleblog.com/2025/11/workspace-nano-banana-pro.html)** 根据笔记本中的来源生成可下载的视觉摘要，可指定重点、画布方向和信息详略。
- [Napkin AI](https://www.napkin.ai/) - **公布于 [2024-08-07](https://www.napkin.ai/blog/introducing-napkin/)** 将选中的段落变成可编辑的图解或图表，可导出 SVG 或 PowerPoint 等格式。
- [Venngage AI Infographic Generator](https://venngage.com/ai-tools/infographic-generator) - **发布于 [2024-05-29](https://www.producthunt.com/products/venngage/launches/free-ai-infographic-generator)** 从提示词生成信息图，可在浏览器编辑器中修改文字、颜色和布局。
- [Infogram AI](https://support.infogram.com/hc/en-us/articles/13245179858844-Create-a-project-with-AI) - **公布于 [2024-03-25](https://infogram.com/blog/infogram-ai-data-visualization-tool/)** 根据描述生成可编辑的信息图项目，可发布、下载或嵌入。
- [Recraft AI Vector Generator](https://www.recraft.ai/ai-vector-generator) - **最迟见于 [2024-01-18](https://www.recraft.ai/press-releases/series-a-announcement)** 根据文本生成可编辑 SVG 素材，适合制作信息图中的图标、图解和插画。
- [Piktochart AI](https://support.piktochart.com/article/1988-how-to-generate-infographics-in-pikto-ai) - **发布于 [2023-11-14](https://www.producthunt.com/products/piktochart/launches/piktochart-ai) · 指南更新于 2026-04-30** 根据提示词、粘贴文本或上传文档生成可编辑的信息图草稿。
- [DiagramGPT (Eraser)](https://www.eraser.io/diagramgpt) - **发布于 [2023-05](https://kylepoyar.substack.com/p/how-an-ai-sidecar-product-drove-30)** 把提示词或代码片段转成可编辑的技术图解，包括架构图和流程图。

### 在线生图工具

通过托管生图模型，根据提示词或参考图生成和编辑位图。

- [ChatGPT Images 2.0](https://openai.com/index/introducing-chatgpt-images-2-0/) - **发布于 2026-04-21** 托管生图与图像编辑服务，支持图解、教学图和密集文字排版，输出位图。
- [Nano Banana Pro](https://blog.google/innovation-and-ai/products/nano-banana-pro/) - **发布于 2025-11-20** Google 托管的 Gemini 3 Pro Image 生图与图像编辑模型，提供多语言文字排版和信息图示例。

## 研究论文与评测

了解信息图生成和编辑的研究方法，以及如何衡量生成质量。

### 生成与编辑方法

研究如何从文字、数据或文档生成视觉布局，以及如何在保留内容的情况下修改版面。

- [InfoAgent](https://arxiv.org/abs/2609.39380) - **arXiv v1 2026-09-30** 研究基于证据的信息图生成和局部修复，将图中的表述追溯到原始证据。
- [Editable Visual Design](https://arxiv.org/abs/2609.04034) - **arXiv v1 2026-09-03** 介绍用编程智能体生成保留可编辑文本与素材的结构化海报和信息图。
- [AutoFigure-Edit](https://arxiv.org/abs/2603.06674) - **arXiv v1 2026-03-03** 研究从长篇文本生成可编辑科研插图的方法，结合参考图风格迁移与原生 SVG 编辑。
- [InfoAlign](https://arxiv.org/abs/2602.22901) - **arXiv v1 2026-02-26** 用于创作叙事信息图的人机协作系统，帮助对齐 AI 生成设计与用户的叙事意图。
- [PaperBanana](https://research.google/pubs/paperbanana-automating-academic-illustration-for-ai-scientists/) - **arXiv v1 [2026-01-30](https://arxiv.org/abs/2601.23265)** 从论文上下文及图注生成学术示意图和统计图的多智能体方法。
- [Infogen](https://aclanthology.org/2025.acl-long.1003/) - **发表于 2025-07** 先生成元数据，再转换成信息图代码，将文档变为复杂统计信息图，并提出 Infodat 数据集。
- [BizGen](https://openaccess.thecvf.com/content/CVPR2025/html/Peng_BizGen_Advancing_Article-level_Visual_Text_Rendering_for_Infographics_Generation_CVPR_2025_paper.html) - **发表于 [2025-06-03](https://openaccess.thecvf.com/)** 采用布局引导的扩散模型生成包含长篇文字和密集排版的信息图。[项目页](https://bizgen-msra.github.io/) (站点源码首次提交于 [2025-03-25](https://github.com/bizgen-msra/bizgen-msra.github.io/commit/1ae0721b0f15937724028ee4520bc1451f686ccd)) · [推理代码](https://github.com/1230young/bizgen) (创建于 2025-03-26 · ⭐️ 304)。
- [Epigraphics](https://arxiv.org/abs/2404.10152) - **arXiv v1 2024-04-15** 以想传达的核心信息为创作起点，指导视觉元素的选择和编排。
- [LayoutDM](https://github.com/CyberAgentAILab/layout-dm) - **创建于 2023-03-08 · ⭐️ 297**<br>
  用于可控布局生成的离散扩散模型，可作为分配文本和图形位置的模块。[论文](https://openaccess.thecvf.com/content/CVPR2023/html/Inoue_LayoutDM_Discrete_Diffusion_Model_for_Controllable_Layout_Generation_CVPR_2023_paper.html) (发表于 2023-05-16)。
- [Infographics Wizard](https://arxiv.org/abs/2204.09904) - **arXiv v1 2022-04-21** 从用户提供的文字生成、排序结构化和流程型信息图布局的半自动创作框架。
- [Calliope](https://arxiv.org/abs/2010.09975) - **arXiv v1 2020-10-20** 将电子表格自动编排为可视化数据故事，并支持在故事编辑器中修改。
- [DataShot](https://zhdsun.github.io/papers/sun_tvcg19_paper.pdf) - **发表于 [2019-08-19](https://ieeexplore.ieee.org/abstract/document/8805442)** 从表格数据提取、组织事实，生成视觉化事实摘要。
- [Text-to-Viz](https://arxiv.org/abs/1907.09091) - **arXiv v1 2019-07-22** 从描述比例关系的自然语言陈述生成信息图设计的早期系统。

### 数据集与评测基准

用于评估事实准确性、图表还原度、布局变化，以及模型读取和理解信息图的能力。

- [InfoEdit](https://arxiv.org/abs/2609.33286) - **arXiv v1 2026-09-27** 评估基于指令的信息图编辑，包含结构变更后能否正确重排布局。
- [IGenBench](https://aclanthology.org/2026.acl-long.1713/) - **发表于 2026-07** 用基于问题的核验评估文生信息图，覆盖标签错误和数据编码失真等问题。[代码](https://github.com/MisterBrookT/IGenBench) (创建于 2026-01-09 · ⭐️ 23) · [数据集](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset) (数据首次上传于 [2026-01-15](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset/commits/main) · Hub 创建于 2026-01-09)。
- [BizGenEval](https://microsoft.github.io/BizGenEval/) - **发布于 [2026-03-26](https://arxiv.org/abs/2603.25732)** 面向商业视觉内容生成的基准，包含信息图任务，检查文字、信息与布局要求。
- [InfoChartQA](https://arxiv.org/abs/2505.19028) - **arXiv v1 2025-05-25** 面向信息图中风格化图表理解的视觉问答基准。
- [ChartMimic](https://github.com/chartmimic/chartmimic) - **创建于 2024-06-13 · ⭐️ 135**<br>
  评估视觉语言模型能否根据参考图生成可执行代码来复刻图表。
- [VisEval](https://github.com/microsoft/VisEval) - **创建于 2024-04-18 · ⭐️ 61**<br>
  从有效性、合规性和可读性等维度评估自然语言生成图表的方法。
- [InfographicVQA](https://site.docvqa.org/datasets/infographicvqa) - **训练集发布于 [2020-12](https://site.docvqa.org/challenges/2021)** 针对整张信息图的视觉问答数据集，考查布局、文字、图形元素和数据解读。

## 教程与设计指南

查阅选图表、做版式和写生图提示词的实用方法。

- [OpenAI Image Prompting Guide](https://developers.openai.com/api/docs/guides/image-prompting) - **示例首次提交于 [2026-04-21](https://github.com/openai/openai-cookbook/commits/main/examples/multimodal/image-gen-models-prompting-guide.ipynb)** 提供教学视觉、图解和密集文字画面的提示词与迭代示例。
- [AntV Infographic Design](https://infographic.antv.vision/learn/design) - **首次提交于 [2025-11-21](https://github.com/antvis/Infographic/blob/3bae7c338c60108fbfba0fe93cfa26e2c0b1c67d/site/src/content/learn/design.md)** 解释结构、数据项组件和装饰如何组成一套信息图模板。
- [Nano Banana Pro Prompting Tips](https://blog.google/products-and-platforms/products/gemini/prompting-tips-nano-banana-pro/) - **发表于 2025-11-20** Google 的提示词指南，涉及文字排版、视觉规范，以及图解等高信息密度设计。
- [Choosing a chart type (Datawrapper)](https://www.datawrapper.de/blog/chart-types-guide) - **发表于 2025-06-16** 根据比较、排序和时间变化等分析问题选择合适的图表类型。
- [draw.io Diagram Generation Guide](https://www.drawio.com/docs/reference/diagram-generation/) - **发布日期未公开** 涵盖 AI 图解的输入格式、校验方法，以及在 draw.io 中打开或导出的方法。

## 参与贡献

欢迎推荐新资源、更新条目描述或报告失效链接。参阅[贡献指南](CONTRIBUTING.md#中文)。
