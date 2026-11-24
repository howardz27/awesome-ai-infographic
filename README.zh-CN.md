# Awesome AI Infographic [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI 信息图资源精选，涵盖生成工具、Agent Skills、模型、论文，以及可嵌入信息图的图表与图解。

[English](README.md) · 简体中文

## 目录

- [按需求查找](#按需求查找)
- [完整信息图生成](#完整信息图生成)
- [渲染框架与信息图技能](#渲染框架与信息图技能)
- [可下载权重的模型](#可下载权重的模型)
- [图表与图解组件](#图表与图解组件)
- [在线工具](#在线工具)
- [论文与评测](#论文与评测)
- [指南与文章](#指南与文章)

## 按需求查找

**编辑文字和对象**。Editable Design 提供可视化编辑器，Paper2Poster 输出可编辑 PPTX，AntV Infographic 渲染可编辑的模板化 SVG。

**修改 HTML、CSS 或 SVG 源码**。Epic Infographics 适合完整构图，Guizang Social Card Skill 适合社交媒体多页图文。

**直接生成位图**。baoyu-infographic 组织提示词并调用生图工具，SenseNova-U1 Infographic V3 提供针对信息图训练的可下载权重。

**从数据生成图表，或从文字生成图解**。Flint 和 Data Formulator 使用结构化数据，Diagram Design 输出 HTML/SVG，Next AI Draw.io 可编辑 draw.io 图解。

**直接在浏览器里生成**。Piktochart AI 生成可编辑草稿，Gemini Notebook 根据来源文档生成视觉摘要。

**评估生成质量**。IGenBench 核验内容与数据编码，InfoEdit 评估编辑后布局如何变化。

## 完整信息图生成

- [AesCode](https://github.com/microsoft/AesCode) - 用生成图像提供设计参考，再编写可编辑的 HTML/CSS，并针对浏览器渲染结果检查内容与设计。
- [Editable Design](https://github.com/yejy53/Editable-Design) - 用编程智能体生成信息图和海报，保留可编辑文本和独立素材，提供可视化编辑器，并可将兼容设计导出为可编辑 PPTX。
- [LIDA](https://github.com/microsoft/lida) - 从表格数据提取摘要和可视化目标并生成图表代码，可进一步用生图模型对渲染结果做风格化。
- [Paper2Poster](https://github.com/Paper2Poster/Paper2Poster) - 从论文 PDF 提炼内容、复用原论文插图，再排版成可编辑的学术海报 PPTX。

## 渲染框架与信息图技能

- [AntV Infographic](https://github.com/antvis/Infographic) - 通过面向大模型的声明式语法生成和流式渲染模板化 SVG 信息图，自带编辑器。
- [baoyu-infographic](https://github.com/JimLiu/baoyu-skills/blob/main/skills/baoyu-infographic/SKILL.md) - 先重组原始内容，再搭配信息布局与视觉风格，最后调用生图工具输出 PNG 的 Agent Skill。
- [Epic Infographics](https://github.com/OrRon/EpicInfographics) - 以场景为构图单位的 HTML/CSS 信息图技能，包含数据驱动的图形尺寸计算、渲染检查和 PNG 导出，并支持动态版本。
- [Guizang Social Card Skill](https://github.com/op7418/guizang-social-card-skill) - 生成单文件 HTML 的小红书图文轮播和微信公众号封面对，并用 Playwright 导出 PNG。
- [Visual Explainer](https://github.com/nicobailon/visual-explainer) - 生成自包含 HTML 解释页的 Agent Skill，适合组合技术图解、对比表格与项目概览。

## 可下载权重的模型

许可证标注对应所链接的权重。访问条件以及代码、数据集的独立许可证可在模型卡中查看。

### 信息图专用模型

- [AesCode 8B and 32B](https://huggingface.co/microsoft/AesCode-8B) - Apache-2.0。根据提示词与可选参考图，为海报、幻灯片和仪表板生成可编辑的 HTML/CSS。[32B 权重](https://huggingface.co/microsoft/AesCode-32B)。
- [BizGen](https://huggingface.co/PYY2001/BizGen) - 模型卡标注 Apache-2.0。基于 SDXL 的权重，根据给定布局渲染信息图和幻灯片中按区域指定的密集文字。
- [SenseNova-U1 Infographic V3](https://huggingface.co/sensenova/SenseNova-U1-8B-MoT-Infographic-V3) - Apache-2.0。针对信息图微调的多模态模型，支持文生图和基于指令的位图编辑。

### 生图与图层模型

- [FLUX.2 klein 4B](https://huggingface.co/black-forest-labs/FLUX.2-klein-4B) - Apache-2.0。较轻量的通用生图与图像编辑模型，可用于生成插画素材或基于参考图迭代。
- [GLM-Image](https://huggingface.co/zai-org/GLM-Image) - MIT。重视文字渲染的生图和图像编辑模型，模型卡包含知识型视觉示例。
- [Ideogram 4](https://huggingface.co/ideogram-ai/ideogram-4-nf4) - Ideogram 4 非商业许可，访问 NF4 权重需接受访问条款。支持位图生成与编辑、区域控制和多语言文字渲染。
- [Qwen-Image](https://huggingface.co/Qwen/Qwen-Image) - Apache-2.0。生图模型，模型卡展示了海报和视觉排版中的密集中文、英文文字。
- [Qwen-Image-Layered](https://huggingface.co/Qwen/Qwen-Image-Layered) - Apache-2.0。把一张图片拆成多个 RGBA 位图图层，各图层可单独移动或替换。
- [Z-Image-Turbo](https://huggingface.co/Tongyi-MAI/Z-Image-Turbo) - Apache-2.0。蒸馏版生图模型，模型卡提供中文和英文文字渲染示例。

## 图表与图解组件

这些资源用于生成、复刻或渲染单个组件，例如数据图表、流程图和科研插图。

### 数据图表

- [AntV MCP Server Chart](https://github.com/antvis/mcp-server-chart) - 通过 MCP 工具和技能，根据结构化参数生成常用统计图表与部分图解。
- [ChartCoder](https://github.com/thunlp/ChartCoder) - 把图表截图转成可编辑绘图代码的专用模型，作者提供可下载权重。
- [Data Formulator](https://github.com/microsoft/data-formulator) - 支持自然语言数据变换和迭代式图表编写的交互式 AI 数据分析工具。
- [Flint](https://github.com/microsoft/flint-chart) - 提供精简的图表语言和 MCP 接入，可将人可编辑的规范编译为 Vega-Lite、ECharts、Chart.js、Plotly 或可编辑的 Excel 图表。
- [GPT-Vis](https://github.com/antvis/GPT-Vis) - 渲染 AI 生成的图表配置，提供可嵌入网页应用的可视化组件。

### 图解与科研插图

- [AutoFigure-Edit](https://github.com/ResearAI/AutoFigure-Edit) - 从长篇技术文本及参考风格生成科研插图，包含原生 SVG 编辑步骤。
- [CanvasAnvil](https://github.com/CodingFeng101/CanvasAnvil) - 可自托管的 AI 图解编辑器，支持无限画布和可编辑的 draw.io 文件。
- [Diagram Design](https://github.com/cathrynlavery/diagram-design) - 用单文件 HTML 和内嵌 SVG 生成流程、对比和系统架构图的 Agent Skill。
- [draw.io MCP](https://github.com/jgraph/drawio-mcp) - draw.io 官方工具，可接收 AI 生成的图解，并将 Mermaid 转为含可编辑形状和连线的 draw.io 图。
- [Next AI Draw.io](https://github.com/DayuanJiang/next-ai-draw-io) - 通过对话创建和修改 draw.io 图解，提供 Web、桌面和 MCP 入口。
- [PaperBanana](https://github.com/llmsresearch/paperbanana) - PaperBanana 论文的社区实现，根据方法描述和图注生成科研示意图与数据图。

### 渲染库

可把这些确定性渲染库接在 AI 生成的图表描述与源数据之后。

- [Apache ECharts](https://github.com/apache/echarts) - 用 JavaScript 配置对象渲染交互式网页图表，支持 SVG 和 Canvas。
- [Mermaid](https://github.com/mermaid-js/mermaid) - 通过文本语法渲染流程图、时序图、时间线等结构化图解。
- [Vega-Lite](https://github.com/vega/vega-lite) - 以 JSON 声明数据编码、图层组合和交互方式的可视化语法。

## 在线工具

这些托管服务可生成整张信息图，或完成其中某个环节。

### 信息图与组件工具

- [AntV Infographic AI Demo](https://infographic.antv.vision/ai) - 可交互体验 AntV 信息图生成流程，并查看渲染效果。
- [DiagramGPT (Eraser)](https://www.eraser.io/diagramgpt) - 把提示词或代码片段转成可编辑的技术图解，包括架构图和流程图。
- [Gemini Notebook (NotebookLM)](https://support.google.com/gemininotebook/answer/16758265?hl=en) - 根据笔记本中的来源生成可下载的视觉摘要，可指定重点、画布方向和信息详略。
- [Infogram AI](https://support.infogram.com/hc/en-us/articles/13245179858844-Create-a-project-with-AI) - 根据描述生成可编辑的信息图项目，可发布、下载或嵌入。
- [Napkin AI](https://www.napkin.ai/) - 将选中的段落变成可编辑的图解或图表，可导出 SVG 或 PowerPoint 等格式。
- [Piktochart AI](https://support.piktochart.com/article/1988-how-to-generate-infographics-in-pikto-ai) - 根据提示词、粘贴文本或上传文档生成可编辑的信息图草稿。
- [Recraft AI Vector Generator](https://www.recraft.ai/ai-vector-generator) - 根据文本生成可编辑 SVG 素材，适合制作信息图中的图标、图解和插画。
- [Venngage AI Infographic Generator](https://venngage.com/ai-tools/infographic-generator) - 从提示词生成信息图，可在浏览器编辑器中修改文字、颜色和布局。

### 托管生图服务

- [ChatGPT Images 2.0](https://openai.com/index/introducing-chatgpt-images-2-0/) - 托管生图与图像编辑服务，支持图解、教学图和密集文字排版，输出位图。
- [Nano Banana Pro](https://blog.google/innovation-and-ai/products/nano-banana-pro/) - Google 托管的 Gemini 3 Pro Image 生图与图像编辑模型，提供多语言文字排版和信息图示例。

## 论文与评测

### 生成与创作

- [AutoFigure-Edit](https://arxiv.org/abs/2603.06674) - 研究从长篇文本生成可编辑科研插图的方法，结合参考图风格迁移与原生 SVG 编辑。
- [BizGen](https://openaccess.thecvf.com/content/CVPR2025/html/Peng_BizGen_Advancing_Article-level_Visual_Text_Rendering_for_Infographics_Generation_CVPR_2025_paper.html) - 采用布局引导的扩散模型生成包含长篇文字和密集排版的信息图。[项目页](https://bizgen-msra.github.io/) · [推理代码](https://github.com/1230young/bizgen)。
- [Calliope](https://arxiv.org/abs/2010.09975) - 将电子表格自动编排为可视化数据故事，并支持在故事编辑器中修改。
- [DataShot](https://zhdsun.github.io/papers/sun_tvcg19_paper.pdf) - 从表格数据提取、组织事实，生成视觉化事实摘要。
- [Editable Visual Design](https://arxiv.org/abs/2609.04034) - 介绍用编程智能体生成保留可编辑文本与素材的结构化海报和信息图。
- [Epigraphics](https://arxiv.org/abs/2404.10152) - 以想传达的核心信息为创作起点，指导视觉元素的选择和编排。
- [InfoAgent](https://arxiv.org/abs/2609.39380) - 研究基于证据的信息图生成和局部修复，将图中的表述追溯到原始证据。
- [InfoAlign](https://arxiv.org/abs/2602.22901) - 用于创作叙事信息图的人机协作系统，帮助对齐 AI 生成设计与用户的叙事意图。
- [Infogen](https://aclanthology.org/2025.acl-long.1003/) - 先生成元数据，再转换成信息图代码，将文档变为复杂统计信息图，并提出 Infodat 数据集。
- [Infographics Wizard](https://arxiv.org/abs/2204.09904) - 从用户提供的文字生成、排序结构化和流程型信息图布局的半自动创作框架。
- [LayoutDM](https://github.com/CyberAgentAILab/layout-dm) - 用于可控布局生成的离散扩散模型，可作为分配文本和图形位置的模块。[论文](https://openaccess.thecvf.com/content/CVPR2023/html/Inoue_LayoutDM_Discrete_Diffusion_Model_for_Controllable_Layout_Generation_CVPR_2023_paper.html)。
- [PaperBanana](https://research.google/pubs/paperbanana-automating-academic-illustration-for-ai-scientists/) - 从论文上下文及图注生成学术示意图和统计图的多智能体方法。
- [Text-to-Viz](https://arxiv.org/abs/1907.09091) - 从描述比例关系的自然语言陈述生成信息图设计的早期系统。

### 数据集与评估

- [BizGenEval](https://microsoft.github.io/BizGenEval/) - 面向商业视觉内容生成的基准，包含信息图任务，检查文字、信息与布局要求。
- [ChartMimic](https://github.com/chartmimic/chartmimic) - 评估视觉语言模型能否根据参考图生成可执行代码来复刻图表。
- [IGenBench](https://aclanthology.org/2026.acl-long.1713/) - 用基于问题的核验评估文生信息图，覆盖标签错误和数据编码失真等问题。[代码](https://github.com/MisterBrookT/IGenBench) · [数据集](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset)。
- [InfoChartQA](https://arxiv.org/abs/2505.19028) - 面向信息图中风格化图表理解的视觉问答基准。
- [InfographicVQA](https://site.docvqa.org/datasets/infographicvqa) - 针对整张信息图的视觉问答数据集，考查布局、文字、图形元素和数据解读。
- [InfoEdit](https://arxiv.org/abs/2609.33286) - 评估基于指令的信息图编辑，包含结构变更后能否正确重排布局。
- [VisEval](https://github.com/microsoft/VisEval) - 从有效性、合规性和可读性等维度评估自然语言生成图表的方法。

## 指南与文章

- [AntV Infographic Design](https://infographic.antv.vision/learn/design) - 解释结构、数据项组件和装饰如何组成一套信息图模板。
- [Choosing a chart type (Datawrapper)](https://www.datawrapper.de/blog/chart-types-guide) - 根据比较、排序和时间变化等分析问题选择合适的图表类型。
- [draw.io Diagram Generation Guide](https://www.drawio.com/docs/reference/diagram-generation/) - 涵盖 AI 图解的输入格式、校验方法，以及在 draw.io 中打开或导出的方法。
- [Nano Banana Pro Prompting Tips](https://blog.google/products-and-platforms/products/gemini/prompting-tips-nano-banana-pro/) - Google 的提示词指南，涉及文字排版、视觉规范，以及图解等高信息密度设计。
- [OpenAI Image Prompting Guide](https://developers.openai.com/api/docs/guides/image-prompting) - 提供教学视觉、图解和密集文字画面的提示词与迭代示例。

## 参与贡献

欢迎推荐新资源、更新条目描述或报告失效链接。参阅[贡献指南](CONTRIBUTING.md#中文)。
