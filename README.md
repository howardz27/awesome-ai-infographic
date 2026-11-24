# Awesome AI Infographic [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of AI tools, skills, models and research for generating infographics, charts and diagrams.

English · [简体中文](README.zh-CN.md)

Resources are sorted newest first within each section. Dates identify the event shown, including repository creation, releases, publications and first commits. Undated resources appear last. GitHub star counts (⭐️) are a snapshot from 2026-11-24.

## Contents

- [Start here](#start-here)
- [Complete infographic generators](#complete-infographic-generators)
- [Agent skills for infographics](#agent-skills-for-infographics)
- [Infographic rendering engines](#infographic-rendering-engines)
- [Downloadable models](#downloadable-models)
- [Chart and diagram components](#chart-and-diagram-components)
- [Online tools](#online-tools)
- [Research papers and benchmarks](#research-papers-and-benchmarks)
- [Tutorials and design guides](#tutorials-and-design-guides)

## Start here

Choose a workflow based on what you want to make and how you want to edit the result.

**Editable text and objects**. Editable Design offers a visual editor, and Paper2Poster writes editable PPTX. AntV Infographic renders editable template-based SVG.

**HTML, CSS or SVG source**. Epic Infographics creates full compositions, and Guizang Social Card Skill handles social carousels.

**Raster images**. baoyu-infographic builds an image prompt and calls a generator. SenseNova-U1 Infographic V3 has downloadable weights tuned for infographics.

**Charts from data or diagrams from text**. Flint and Data Formulator use structured data. Diagram Design writes HTML/SVG, and Next AI Draw.io edits draw.io diagrams.

**Browser-only workflow**. Piktochart AI creates editable drafts, and Gemini Notebook generates a visual summary from source documents.

**Evaluate generated output**. IGenBench checks content and data encodings, and InfoEdit tests how layouts respond to edits.

## Complete infographic generators

Start with text, data or a document and use these projects to produce a complete infographic or poster. Some offer editable HTML or PowerPoint output.

- [Editable Design](https://github.com/yejy53/Editable-Design) - **Created 2026-08-24 · ⭐️ 1,272**<br>
  Coding-agent workflow for infographics and posters with editable text, independent assets, a visual editor and optional editable PPTX export for compatible designs.
- [AesCode](https://github.com/microsoft/AesCode) - **Created 2026-07-23 · ⭐️ 285**<br>
  Research pipeline that uses a generated image as a design reference, then produces editable HTML/CSS and checks the rendered result against content and design criteria.
- [Paper2Poster](https://github.com/Paper2Poster/Paper2Poster) - **Created 2025-05-16 · ⭐️ 4,055**<br>
  Multi-agent pipeline that summarizes a research PDF, reuses figures from the paper and lays out an editable academic poster in PPTX.
- [LIDA](https://github.com/microsoft/lida) - **Created 2023-03-09 · ⭐️ 3,299**<br>
  Summarizes tabular data, proposes visualization goals, generates chart code and optionally uses an image model to stylize the rendered chart.

## Agent skills for infographics

Load these instructions into a compatible AI agent to guide how it organizes content, chooses a layout and calls an HTML renderer or image model.

- [Epic Infographics](https://github.com/OrRon/EpicInfographics) - **Created 2026-08-23 · ⭐️ 502**<br>
  Agent skill for scene-based HTML/CSS infographics with computed chart geometry, render checks and PNG export. It also supports animated variants.
- [Guizang Social Card Skill](https://github.com/op7418/guizang-social-card-skill) - **Created 2026-05-27 · ⭐️ 8,244**<br>
  Renders Xiaohongshu carousels and WeChat cover pairs from single-file HTML to PNG using Playwright.
- [Visual Explainer](https://github.com/nicobailon/visual-explainer) - **Created 2026-02-16 · ⭐️ 11,253**<br>
  Agent skill for self-contained HTML explainers with diagrams, comparison tables and project recaps.
- [baoyu-infographic](https://github.com/JimLiu/baoyu-skills/blob/main/skills/baoyu-infographic/SKILL.md) - **First commit [2026-01-20](https://github.com/JimLiu/baoyu-skills/blob/b30dcca67e47ed269683f706489e782adee3de04/skills/baoyu-infographic/SKILL.md) · Repository created 2026-01-13 · ⭐️ 27,853**<br>
  Agent skill that restructures source material, pairs an information layout with a visual style and calls an image generator to produce a PNG.

## Infographic rendering engines

Integrate these engines into your own project to turn a structured specification and data into a visual, such as a template-based SVG.

- [AntV Infographic](https://github.com/antvis/Infographic) - **Created 2025-09-11 · ⭐️ 7,157**<br>
  Declarative, LLM-friendly syntax for generating and streaming template-based SVG infographics, with a built-in editor.

## Downloadable models

Download weights to run a model in your own workflow. License labels apply to the linked weights. Check the model card for access terms and separate licenses for code or datasets.

### Models built for infographics

These models are trained for tasks such as composing an infographic, rendering text-heavy layouts, or producing editable HTML and CSS.

- [AesCode 8B and 32B](https://huggingface.co/microsoft/AesCode-8B) - **Released [2026-10-14](https://huggingface.co/microsoft/AesCode-8B/commits/main) · Hub created 2026-09-29** Apache-2.0. Generates editable HTML/CSS for posters, slides and dashboards from a prompt and an optional reference image. [32B weights](https://huggingface.co/microsoft/AesCode-32B) (Released [2026-10-14](https://huggingface.co/microsoft/AesCode-32B/commits/main) · Hub created 2026-09-29).
- [SenseNova-U1 Infographic V3](https://huggingface.co/sensenova/SenseNova-U1-8B-MoT-Infographic-V3) - **Released [2026-07-16](https://github.com/OpenSenseNova/SenseNova-U1#news) · Hub created 2026-07-15** Apache-2.0. An infographic-tuned multimodal model for text-to-image generation and instruction-based raster editing.
- [BizGen](https://huggingface.co/PYY2001/BizGen) - **Hub created 2025-03-24** Apache-2.0 as listed on the model card. SDXL-based checkpoints for rendering dense, region-specific text in infographics and slides from a supplied layout.

### Image generation and layer editing

Use these models to generate a raster infographic or illustration, edit an existing image, or split an image into layers.

- [Ideogram 4](https://huggingface.co/ideogram-ai/ideogram-4-nf4) - **Released [2026-06-03](https://ideogram.ai/news/ideogram-4.0/) · Hub created 2026-05-30** Gated NF4 weights under the Ideogram 4 Non-Commercial license. Generates or edits raster images with region-level controls and multilingual text rendering.
- [FLUX.2 klein 4B](https://huggingface.co/black-forest-labs/FLUX.2-klein-4B) - **Released [2026-01-15](https://bfl.ai/blog/flux2-klein-towards-interactive-visual-intelligence) · Hub created 2026-01-14** Apache-2.0. Compact general-purpose image generation and editing model for creating illustration assets or iterating on a visual reference.
- [GLM-Image](https://huggingface.co/zai-org/GLM-Image) - **Announced [2026-01-13](https://www.zhipuai.cn/zh/research/158) · Hub created 2026-01-08** MIT. Image generation and editing model with an explicit focus on text rendering and examples of knowledge-rich graphics.
- [Qwen-Image-Layered](https://huggingface.co/Qwen/Qwen-Image-Layered) - **Released [2025-12-19](https://github.com/QwenLM/Qwen-Image/blob/main/README.md) · Hub created 2025-12-17** Apache-2.0. Decomposes one image into multiple RGBA layers that can be repositioned or replaced separately.
- [Z-Image-Turbo](https://huggingface.co/Tongyi-MAI/Z-Image-Turbo) - **Released [2025-11-26](https://github.com/Tongyi-MAI/Z-Image#news) · Hub created 2025-11-25** Apache-2.0. Distilled image generation model with Chinese and English text-rendering examples.
- [Qwen-Image](https://huggingface.co/Qwen/Qwen-Image) - **Released [2025-08-04](https://qwenlm.github.io/blog/qwen-image/) · Hub created 2025-08-02** Apache-2.0. Image generation model with examples of dense Chinese and English typography in posters and visual layouts.

## Chart and diagram components

Build individual pieces to place inside an infographic, such as a data chart, a flowchart or a scientific illustration.

### Data charts

Generate charts from data, recreate charts from screenshots, or embed AI-generated chart specifications in an app.

- [Flint](https://github.com/microsoft/flint-chart) - **Created 2026-05-13 · ⭐️ 4,605**<br>
  Compact chart language and MCP integration. Compiles human-editable specifications to Vega-Lite, ECharts, Chart.js, Plotly or editable Excel charts.
- [AntV MCP Server Chart](https://github.com/antvis/mcp-server-chart) - **Created 2025-04-25 · ⭐️ 4,423**<br>
  MCP tools and a skill for generating charts from structured arguments, including common statistical charts and some diagrams.
- [ChartCoder](https://github.com/thunlp/ChartCoder) - **Created 2025-01-14 · ⭐️ 81**<br>
  Chart-to-code model trained to turn chart screenshots into editable plotting code, with downloadable weights linked by the authors.
- [Data Formulator](https://github.com/microsoft/data-formulator) - **Created 2024-06-07 · ⭐️ 17,696**<br>
  Interactive AI data analysis with natural-language data transformations and iterative chart authoring.
- [GPT-Vis](https://github.com/antvis/GPT-Vis) - **Created 2023-11-13 · ⭐️ 807**<br>
  Renderer for AI-generated chart specifications, with embeddable visualization components for web applications.

### Diagrams and scientific illustrations

Turn descriptions or research material into visuals such as flowcharts, architecture diagrams and scientific figures.

- [Diagram Design](https://github.com/cathrynlavery/diagram-design) - **Created 2026-04-16 · ⭐️ 71,452**<br>
  Agent skill for creating self-contained HTML and inline SVG diagrams such as workflows, comparisons and system architecture.
- [PaperBanana](https://github.com/llmsresearch/paperbanana) - **Created 2026-02-04 · ⭐️ 2,506**<br>
  Community implementation of the PaperBanana paper for generating scientific diagrams and plots from a method description and caption.
- [AutoFigure-Edit](https://github.com/ResearAI/AutoFigure-Edit) - **Created 2026-02-03 · ⭐️ 4,429**<br>
  Generates scientific illustrations from long-form technical text and reference styles, with a native SVG editing stage.
- [draw.io MCP](https://github.com/jgraph/drawio-mcp) - **Created 2026-02-02 · ⭐️ 5,892**<br>
  Official draw.io tools for passing AI-generated diagrams into draw.io, including Mermaid-to-draw.io conversion with editable shapes and connectors.
- [CanvasAnvil](https://github.com/CodingFeng101/CanvasAnvil) - **Created 2026-01-24 · ⭐️ 226**<br>
  Self-hostable AI diagram editor with an infinite canvas and editable draw.io files for generated diagrams.
- [Next AI Draw.io](https://github.com/DayuanJiang/next-ai-draw-io) - **Created 2025-03-23 · ⭐️ 37,154**<br>
  Chat-driven creation and editing of draw.io diagrams, with web, desktop and MCP entry points.

### Chart and diagram renderers

Turn AI-generated chart specifications or diagram syntax into visuals you can embed or export.

- [Vega-Lite](https://github.com/vega/vega-lite) - **Created 2014-11-20 · ⭐️ 5,562**<br>
  Declarative grammar for chart encodings, layered views and interactions, represented as JSON.
- [Mermaid](https://github.com/mermaid-js/mermaid) - **Created 2014-11-01 · ⭐️ 91,221**<br>
  Text-to-diagram syntax for flowcharts, sequences, timelines and other structured diagrams.
- [Apache ECharts](https://github.com/apache/echarts) - **Created 2013-04-03 · ⭐️ 67,788**<br>
  JavaScript chart engine that renders option objects as interactive web charts, with SVG or Canvas rendering.

## Online tools

Try hosted tools in the browser to create an infographic or make visuals for one.

### Infographic and diagram makers

Turn prompts, documents or selected passages into infographics, diagrams or vector assets. Editing and export options vary by tool.

- [AntV Infographic AI Demo](https://infographic.antv.vision/ai) - **First commit [2025-11-21](https://github.com/antvis/Infographic/blob/3bae7c338c60108fbfba0fe93cfa26e2c0b1c67d/site/src/pages/ai.tsx)** Interactive demo for trying the AntV generation workflow and inspecting its rendered output.
- [Gemini Notebook (NotebookLM)](https://support.google.com/gemininotebook/answer/16758265?hl=en) - **Released [2025-11-20](https://workspaceupdates.googleblog.com/2025/11/workspace-nano-banana-pro.html)** Builds a downloadable visual summary grounded in notebook sources, with controls for focus, orientation and level of detail.
- [Napkin AI](https://www.napkin.ai/) - **Announced [2024-08-07](https://www.napkin.ai/blog/introducing-napkin/)** Turns selected passages into editable visuals such as diagrams and charts, with SVG and PowerPoint among its export options.
- [Venngage AI Infographic Generator](https://venngage.com/ai-tools/infographic-generator) - **Released [2024-05-29](https://www.producthunt.com/products/venngage/launches/free-ai-infographic-generator)** Generates an infographic from a prompt and opens it in a browser editor for changes to text, colors and layout.
- [Infogram AI](https://support.infogram.com/hc/en-us/articles/13245179858844-Create-a-project-with-AI) - **Announced [2024-03-25](https://infogram.com/blog/infogram-ai-data-visualization-tool/)** Generates an editable infographic project from a description, with options to publish, download or embed it.
- [Recraft AI Vector Generator](https://www.recraft.ai/ai-vector-generator) - **Documented by [2024-01-18](https://www.recraft.ai/press-releases/series-a-announcement)** Generates editable SVG assets from text, useful for icons, diagrams and illustrations within an infographic.
- [Piktochart AI](https://support.piktochart.com/article/1988-how-to-generate-infographics-in-pikto-ai) - **Released [2023-11-14](https://www.producthunt.com/products/piktochart/launches/piktochart-ai) · Guide updated 2026-04-30** Generates an editable infographic draft from a prompt, pasted text or an uploaded document.
- [DiagramGPT (Eraser)](https://www.eraser.io/diagramgpt) - **Released [2023-05](https://kylepoyar.substack.com/p/how-an-ai-sidecar-product-drove-30)** Turns prompts or code snippets into editable technical diagrams, including architecture diagrams and flowcharts.

### Online image generators

Generate and edit raster images from prompts or references using a hosted image model.

- [ChatGPT Images 2.0](https://openai.com/index/introducing-chatgpt-images-2-0/) - **Released 2026-04-21** Hosted image generation and editing with examples of diagrams, instructional visuals and dense text layouts. Outputs raster images.
- [Nano Banana Pro](https://blog.google/innovation-and-ai/products/nano-banana-pro/) - **Released 2025-11-20** Google’s hosted Gemini 3 Pro Image model for image generation and editing, with examples of multilingual typography and infographics.

## Research papers and benchmarks

Explore how researchers generate and edit infographics and measure the quality of the results.

### Generation and editing methods

Research on turning text, data or documents into visual layouts, and on editing those layouts while preserving their content.

- [InfoAgent](https://arxiv.org/abs/2609.39380) - **arXiv v1 2026-09-30** Studies evidence-grounded infographic generation and targeted repairs that trace visual claims back to source evidence.
- [Editable Visual Design](https://arxiv.org/abs/2609.04034) - **arXiv v1 2026-09-03** Describes a coding-agent workflow for producing structured posters and infographics with editable text and assets.
- [AutoFigure-Edit](https://arxiv.org/abs/2603.06674) - **arXiv v1 2026-03-03** Generates editable scientific illustrations from long-form text, combining reference-guided styling with native SVG editing.
- [InfoAlign](https://arxiv.org/abs/2602.22901) - **arXiv v1 2026-02-26** Human–AI co-authoring system for storytelling infographics that helps align AI-generated designs with user intent.
- [PaperBanana](https://research.google/pubs/paperbanana-automating-academic-illustration-for-ai-scientists/) - **arXiv v1 [2026-01-30](https://arxiv.org/abs/2601.23265)** Multi-agent method for generating academic diagrams and statistical plots from manuscript context and a caption.
- [Infogen](https://aclanthology.org/2025.acl-long.1003/) - **Published 2025-07** Turns documents into complex statistical infographics by first generating metadata, then converting it to infographic code. Introduces the Infodat dataset.
- [BizGen](https://openaccess.thecvf.com/content/CVPR2025/html/Peng_BizGen_Advancing_Article-level_Visual_Text_Rendering_for_Infographics_Generation_CVPR_2025_paper.html) - **Published [2025-06-03](https://openaccess.thecvf.com/)** Uses layout-guided diffusion for article-length text and dense infographic layouts. [Project](https://bizgen-msra.github.io/) (First site source commit [2025-03-25](https://github.com/bizgen-msra/bizgen-msra.github.io/commit/1ae0721b0f15937724028ee4520bc1451f686ccd)) · [Inference code](https://github.com/1230young/bizgen) (Created 2025-03-26 · ⭐️ 304).
- [Epigraphics](https://arxiv.org/abs/2404.10152) - **arXiv v1 2024-04-15** Message-driven infographic authoring that uses a textual takeaway to guide selection and arrangement of visual elements.
- [LayoutDM](https://github.com/CyberAgentAILab/layout-dm) - **Created 2023-03-08 · ⭐️ 297**<br>
  Discrete diffusion for controllable layout generation, useful as a module for placing text and graphics on a canvas. [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Inoue_LayoutDM_Discrete_Diffusion_Model_for_Controllable_Layout_Generation_CVPR_2023_paper.html) (Published 2023-05-16).
- [Infographics Wizard](https://arxiv.org/abs/2204.09904) - **arXiv v1 2022-04-21** Semi-automated authoring framework that generates and ranks structured and flow-based infographic layouts from user-provided text.
- [Calliope](https://arxiv.org/abs/2010.09975) - **arXiv v1 2020-10-20** Automatically generates visual data stories from spreadsheets and supports revision in a story editor.
- [DataShot](https://zhdsun.github.io/papers/sun_tvcg19_paper.pdf) - **Published [2019-08-19](https://ieeexplore.ieee.org/abstract/document/8805442)** Extracts and composes facts from tabular data into a visual fact sheet.
- [Text-to-Viz](https://arxiv.org/abs/1907.09091) - **arXiv v1 2019-07-22** Early system that translates natural-language statements about proportions into infographic designs.

### Datasets and evaluation benchmarks

Use these resources to assess factual accuracy, chart fidelity, layout changes and how well models read infographics.

- [InfoEdit](https://arxiv.org/abs/2609.33286) - **arXiv v1 2026-09-27** Benchmark for instruction-based infographic editing, including whether layouts reflow correctly after structural changes.
- [IGenBench](https://aclanthology.org/2026.acl-long.1713/) - **Published 2026-07** Text-to-infographic benchmark with question-based checks for errors such as mislabeled content and distorted data encodings. [Code](https://github.com/MisterBrookT/IGenBench) (Created 2026-01-09 · ⭐️ 23) · [Dataset](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset) (First data upload [2026-01-15](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset/commits/main) · Hub created 2026-01-09).
- [BizGenEval](https://microsoft.github.io/BizGenEval/) - **Released [2026-03-26](https://arxiv.org/abs/2603.25732)** Benchmark for commercial visual content generation, including infographics, with checks for text, information and layout requirements.
- [InfoChartQA](https://arxiv.org/abs/2505.19028) - **arXiv v1 2025-05-25** Question-answering benchmark for reading stylized charts embedded in infographics.
- [ChartMimic](https://github.com/chartmimic/chartmimic) - **Created 2024-06-13 · ⭐️ 135**<br>
  Tests whether vision-language models can reproduce reference charts as executable plotting code.
- [VisEval](https://github.com/microsoft/VisEval) - **Created 2024-04-18 · ⭐️ 61**<br>
  Benchmarks natural-language-to-visualization methods on validity, legality and readability.
- [InfographicVQA](https://site.docvqa.org/datasets/infographicvqa) - **Training split released [2020-12](https://site.docvqa.org/challenges/2021)** Visual question answering dataset that probes layout, text, graphical elements and data interpretation across whole infographics.

## Tutorials and design guides

Practical resources for choosing charts, designing layouts and writing prompts for infographic workflows.

- [OpenAI Image Prompting Guide](https://developers.openai.com/api/docs/guides/image-prompting) - **Examples first committed [2026-04-21](https://github.com/openai/openai-cookbook/commits/main/examples/multimodal/image-gen-models-prompting-guide.ipynb)** Examples of prompting and iterating on instructional visuals, diagrams and text-heavy compositions.
- [AntV Infographic Design](https://infographic.antv.vision/learn/design) - **First commit [2025-11-21](https://github.com/antvis/Infographic/blob/3bae7c338c60108fbfba0fe93cfa26e2c0b1c67d/site/src/content/learn/design.md)** Explains how the structure, data item components and decorations combine in an infographic template.
- [Nano Banana Pro Prompting Tips](https://blog.google/products-and-platforms/products/gemini/prompting-tips-nano-banana-pro/) - **Published 2025-11-20** Google’s prompting guide covers typography, visual specifications and information-rich designs such as diagrams.
- [Choosing a chart type (Datawrapper)](https://www.datawrapper.de/blog/chart-types-guide) - **Published 2025-06-16** Maps analytical questions such as comparison, ranking and change over time to chart types.
- [draw.io Diagram Generation Guide](https://www.drawio.com/docs/reference/diagram-generation/) - **Publication date unlisted** Documents input formats, diagram validation and ways to export or open AI-generated diagrams in draw.io.

## Contributing

Suggest a resource, update a description or report a broken link. See the [contribution guidelines](CONTRIBUTING.md).
