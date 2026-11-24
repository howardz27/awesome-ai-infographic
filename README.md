# Awesome AI Infographic [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of AI tools, skills, models and research for generating infographics, charts and diagrams.

English · [简体中文](README.zh-CN.md)

## Contents

- [Choose a workflow](#choose-a-workflow)
- [Infographic generators](#infographic-generators)
- [Rendering frameworks and skills](#rendering-frameworks-and-skills)
- [Models with downloadable weights](#models-with-downloadable-weights)
- [Chart and diagram components](#chart-and-diagram-components)
- [Web tools](#web-tools)
- [Papers and benchmarks](#papers-and-benchmarks)
- [Guides and articles](#guides-and-articles)

## Choose a workflow

**Editable text and objects**. Editable Design offers a visual editor, and Paper2Poster writes editable PPTX. AntV Infographic renders editable template-based SVG.

**HTML, CSS or SVG source**. Epic Infographics creates full compositions, and Guizang Social Card Skill handles social carousels.

**Raster images**. baoyu-infographic builds an image prompt and calls a generator. SenseNova-U1 Infographic V3 has downloadable weights tuned for infographics.

**Charts from data or diagrams from text**. Flint and Data Formulator use structured data. Diagram Design writes HTML/SVG, and Next AI Draw.io edits draw.io diagrams.

**Browser-only workflow**. Piktochart AI creates editable drafts, and Gemini Notebook generates a visual summary from source documents.

**Evaluate generated output**. IGenBench checks content and data encodings, and InfoEdit tests how layouts respond to edits.

## Infographic generators

- [AesCode](https://github.com/microsoft/AesCode) - Research pipeline that uses a generated image as a design reference, then produces editable HTML/CSS and checks the rendered result against content and design criteria.
- [Editable Design](https://github.com/yejy53/Editable-Design) - Coding-agent workflow for infographics and posters with editable text, independent assets, a visual editor and optional editable PPTX export for compatible designs.
- [LIDA](https://github.com/microsoft/lida) - Summarizes tabular data, proposes visualization goals, generates chart code and optionally uses an image model to stylize the rendered chart.
- [Paper2Poster](https://github.com/Paper2Poster/Paper2Poster) - Multi-agent pipeline that summarizes a research PDF, reuses figures from the paper and lays out an editable academic poster in PPTX.

## Rendering frameworks and skills

- [AntV Infographic](https://github.com/antvis/Infographic) - Declarative, LLM-friendly syntax for generating and streaming template-based SVG infographics, with a built-in editor.
- [baoyu-infographic](https://github.com/JimLiu/baoyu-skills/blob/main/skills/baoyu-infographic/SKILL.md) - Agent skill that restructures source material, pairs an information layout with a visual style and calls an image generator to produce a PNG.
- [Epic Infographics](https://github.com/OrRon/EpicInfographics) - Agent skill for scene-based HTML/CSS infographics with computed chart geometry, render checks and PNG export. It also supports animated variants.
- [Guizang Social Card Skill](https://github.com/op7418/guizang-social-card-skill) - Renders Xiaohongshu carousels and WeChat cover pairs from single-file HTML to PNG using Playwright.
- [Visual Explainer](https://github.com/nicobailon/visual-explainer) - Agent skill for self-contained HTML explainers with diagrams, comparison tables and project recaps.

## Models with downloadable weights

License labels apply to the linked weights. Check the model card for access terms and separate licenses for code or datasets.

### Infographic-specific models

- [AesCode 8B and 32B](https://huggingface.co/microsoft/AesCode-8B) - Apache-2.0. Generates editable HTML/CSS for posters, slides and dashboards from a prompt and an optional reference image. [32B weights](https://huggingface.co/microsoft/AesCode-32B).
- [BizGen](https://huggingface.co/PYY2001/BizGen) - Apache-2.0 as listed on the model card. SDXL-based checkpoints for rendering dense, region-specific text in infographics and slides from a supplied layout.
- [SenseNova-U1 Infographic V3](https://huggingface.co/sensenova/SenseNova-U1-8B-MoT-Infographic-V3) - Apache-2.0. An infographic-tuned multimodal model for text-to-image generation and instruction-based raster editing.

### Image and layer models

- [FLUX.2 klein 4B](https://huggingface.co/black-forest-labs/FLUX.2-klein-4B) - Apache-2.0. Compact general-purpose image generation and editing model for creating illustration assets or iterating on a visual reference.
- [GLM-Image](https://huggingface.co/zai-org/GLM-Image) - MIT. Image generation and editing model with an explicit focus on text rendering and examples of knowledge-rich graphics.
- [Ideogram 4](https://huggingface.co/ideogram-ai/ideogram-4-nf4) - Gated NF4 weights under the Ideogram 4 Non-Commercial license. Generates or edits raster images with region-level controls and multilingual text rendering.
- [Qwen-Image](https://huggingface.co/Qwen/Qwen-Image) - Apache-2.0. Image generation model with examples of dense Chinese and English typography in posters and visual layouts.
- [Qwen-Image-Layered](https://huggingface.co/Qwen/Qwen-Image-Layered) - Apache-2.0. Decomposes one image into multiple RGBA layers that can be repositioned or replaced separately.
- [Z-Image-Turbo](https://huggingface.co/Tongyi-MAI/Z-Image-Turbo) - Apache-2.0. Distilled image generation model with Chinese and English text-rendering examples.

## Chart and diagram components

Use these to generate, recover or render individual pieces such as data charts, flowcharts and scientific figures.

### Data charts

- [AntV MCP Server Chart](https://github.com/antvis/mcp-server-chart) - MCP tools and a skill for generating charts from structured arguments, including common statistical charts and some diagrams.
- [ChartCoder](https://github.com/thunlp/ChartCoder) - Chart-to-code model trained to turn chart screenshots into editable plotting code, with downloadable weights linked by the authors.
- [Data Formulator](https://github.com/microsoft/data-formulator) - Interactive AI data analysis with natural-language data transformations and iterative chart authoring.
- [Flint](https://github.com/microsoft/flint-chart) - Compact chart language and MCP integration. Compiles human-editable specifications to Vega-Lite, ECharts, Chart.js, Plotly or editable Excel charts.
- [GPT-Vis](https://github.com/antvis/GPT-Vis) - Renderer for AI-generated chart specifications, with embeddable visualization components for web applications.

### Diagrams and scientific figures

- [AutoFigure-Edit](https://github.com/ResearAI/AutoFigure-Edit) - Generates scientific illustrations from long-form technical text and reference styles, with a native SVG editing stage.
- [CanvasAnvil](https://github.com/CodingFeng101/CanvasAnvil) - Self-hostable AI diagram editor with an infinite canvas and editable draw.io files for generated diagrams.
- [Diagram Design](https://github.com/cathrynlavery/diagram-design) - Agent skill for creating self-contained HTML and inline SVG diagrams such as workflows, comparisons and system architecture.
- [draw.io MCP](https://github.com/jgraph/drawio-mcp) - Official draw.io tools for passing AI-generated diagrams into draw.io, including Mermaid-to-draw.io conversion with editable shapes and connectors.
- [Next AI Draw.io](https://github.com/DayuanJiang/next-ai-draw-io) - Chat-driven creation and editing of draw.io diagrams, with web, desktop and MCP entry points.
- [PaperBanana](https://github.com/llmsresearch/paperbanana) - Community implementation of the PaperBanana paper for generating scientific diagrams and plots from a method description and caption.

### Rendering libraries

Pair these deterministic renderers with an AI-generated specification and source data.

- [Apache ECharts](https://github.com/apache/echarts) - JavaScript chart engine that renders option objects as interactive web charts, with SVG or Canvas rendering.
- [Mermaid](https://github.com/mermaid-js/mermaid) - Text-to-diagram syntax for flowcharts, sequences, timelines and other structured diagrams.
- [Vega-Lite](https://github.com/vega/vega-lite) - Declarative grammar for chart encodings, layered views and interactions, represented as JSON.

## Web tools

These hosted tools provide infographic generation or a specific component of the workflow.

### Infographics and components

- [AntV Infographic AI Demo](https://infographic.antv.vision/ai) - Interactive demo for trying the AntV generation workflow and inspecting its rendered output.
- [DiagramGPT (Eraser)](https://www.eraser.io/diagramgpt) - Turns prompts or code snippets into editable technical diagrams, including architecture diagrams and flowcharts.
- [Gemini Notebook (NotebookLM)](https://support.google.com/gemininotebook/answer/16758265?hl=en) - Builds a downloadable visual summary grounded in notebook sources, with controls for focus, orientation and level of detail.
- [Infogram AI](https://support.infogram.com/hc/en-us/articles/13245179858844-Create-a-project-with-AI) - Generates an editable infographic project from a description, with options to publish, download or embed it.
- [Napkin AI](https://www.napkin.ai/) - Turns selected passages into editable visuals such as diagrams and charts, with SVG and PowerPoint among its export options.
- [Piktochart AI](https://support.piktochart.com/article/1988-how-to-generate-infographics-in-pikto-ai) - Generates an editable infographic draft from a prompt, pasted text or an uploaded document.
- [Recraft AI Vector Generator](https://www.recraft.ai/ai-vector-generator) - Generates editable SVG assets from text, useful for icons, diagrams and illustrations within an infographic.
- [Venngage AI Infographic Generator](https://venngage.com/ai-tools/infographic-generator) - Generates an infographic from a prompt and opens it in a browser editor for changes to text, colors and layout.

### Hosted image generation

- [ChatGPT Images 2.0](https://openai.com/index/introducing-chatgpt-images-2-0/) - Hosted image generation and editing with examples of diagrams, instructional visuals and dense text layouts. Outputs raster images.
- [Nano Banana Pro](https://blog.google/innovation-and-ai/products/nano-banana-pro/) - Google’s hosted Gemini 3 Pro Image model for image generation and editing, with examples of multilingual typography and infographics.

## Papers and benchmarks

### Generation and authoring

- [AutoFigure-Edit](https://arxiv.org/abs/2603.06674) - Generates editable scientific illustrations from long-form text, combining reference-guided styling with native SVG editing.
- [BizGen](https://openaccess.thecvf.com/content/CVPR2025/html/Peng_BizGen_Advancing_Article-level_Visual_Text_Rendering_for_Infographics_Generation_CVPR_2025_paper.html) - Uses layout-guided diffusion for article-length text and dense infographic layouts. [Project](https://bizgen-msra.github.io/) · [Inference code](https://github.com/1230young/bizgen).
- [Calliope](https://arxiv.org/abs/2010.09975) - Automatically generates visual data stories from spreadsheets and supports revision in a story editor.
- [DataShot](https://zhdsun.github.io/papers/sun_tvcg19_paper.pdf) - Extracts and composes facts from tabular data into a visual fact sheet.
- [Editable Visual Design](https://arxiv.org/abs/2609.04034) - Describes a coding-agent workflow for producing structured posters and infographics with editable text and assets.
- [Epigraphics](https://arxiv.org/abs/2404.10152) - Message-driven infographic authoring that uses a textual takeaway to guide selection and arrangement of visual elements.
- [InfoAgent](https://arxiv.org/abs/2609.39380) - Studies evidence-grounded infographic generation and targeted repairs that trace visual claims back to source evidence.
- [InfoAlign](https://arxiv.org/abs/2602.22901) - Human–AI co-authoring system for storytelling infographics that helps align AI-generated designs with user intent.
- [Infogen](https://aclanthology.org/2025.acl-long.1003/) - Turns documents into complex statistical infographics by first generating metadata, then converting it to infographic code. Introduces the Infodat dataset.
- [Infographics Wizard](https://arxiv.org/abs/2204.09904) - Semi-automated authoring framework that generates and ranks structured and flow-based infographic layouts from user-provided text.
- [LayoutDM](https://github.com/CyberAgentAILab/layout-dm) - Discrete diffusion for controllable layout generation, useful as a module for placing text and graphics on a canvas. [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Inoue_LayoutDM_Discrete_Diffusion_Model_for_Controllable_Layout_Generation_CVPR_2023_paper.html).
- [PaperBanana](https://research.google/pubs/paperbanana-automating-academic-illustration-for-ai-scientists/) - Multi-agent method for generating academic diagrams and statistical plots from manuscript context and a caption.
- [Text-to-Viz](https://arxiv.org/abs/1907.09091) - Early system that translates natural-language statements about proportions into infographic designs.

### Datasets and evaluation

- [BizGenEval](https://microsoft.github.io/BizGenEval/) - Benchmark for commercial visual content generation, including infographics, with checks for text, information and layout requirements.
- [ChartMimic](https://github.com/chartmimic/chartmimic) - Tests whether vision-language models can reproduce reference charts as executable plotting code.
- [IGenBench](https://aclanthology.org/2026.acl-long.1713/) - Text-to-infographic benchmark with question-based checks for errors such as mislabeled content and distorted data encodings. [Code](https://github.com/MisterBrookT/IGenBench) · [Dataset](https://huggingface.co/datasets/Brookseeworld/IGenBench-Dataset).
- [InfoChartQA](https://arxiv.org/abs/2505.19028) - Question-answering benchmark for reading stylized charts embedded in infographics.
- [InfographicVQA](https://site.docvqa.org/datasets/infographicvqa) - Visual question answering dataset that probes layout, text, graphical elements and data interpretation across whole infographics.
- [InfoEdit](https://arxiv.org/abs/2609.33286) - Benchmark for instruction-based infographic editing, including whether layouts reflow correctly after structural changes.
- [VisEval](https://github.com/microsoft/VisEval) - Benchmarks natural-language-to-visualization methods on validity, legality and readability.

## Guides and articles

- [AntV Infographic Design](https://infographic.antv.vision/learn/design) - Explains how the structure, data item components and decorations combine in an infographic template.
- [Choosing a chart type (Datawrapper)](https://www.datawrapper.de/blog/chart-types-guide) - Maps analytical questions such as comparison, ranking and change over time to chart types.
- [draw.io Diagram Generation Guide](https://www.drawio.com/docs/reference/diagram-generation/) - Documents input formats, diagram validation and ways to export or open AI-generated diagrams in draw.io.
- [Nano Banana Pro Prompting Tips](https://blog.google/products-and-platforms/products/gemini/prompting-tips-nano-banana-pro/) - Google’s prompting guide covers typography, visual specifications and information-rich designs such as diagrams.
- [OpenAI Image Prompting Guide](https://developers.openai.com/api/docs/guides/image-prompting) - Examples of prompting and iterating on instructional visuals, diagrams and text-heavy compositions.

## Contributing

Suggest a resource, update a description or report a broken link. See the [contribution guidelines](CONTRIBUTING.md).
