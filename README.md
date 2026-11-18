<!--
  Icons in assets/icons/ are Font Awesome Free 6.7.2 SVG files (CC BY 4.0 — fontawesome.com/license/free),
  recolored to #FF5A1F (accent) and #FF7A3C (accent-2) to match walidmoustafa2077.github.io. Files are named <icon>-accent.svg / <icon>-accent2.svg.
  assets/pipeline.svg is original artwork. Commit the whole assets/ folder next to this README.
-->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3B1A0B,50:9A3412,100:FF5A1F&height=220&section=header&text=Walid%20Moustafa&fontSize=54&fontColor=ffffff&fontAlignY=38&desc=Full-Stack%20Developer%20%C2%B7%20.NET%20Backends%20%C2%B7%20Document%20Vision&descSize=18&descAlignY=60&animation=fadeIn" width="100%" alt="Walid Moustafa — full-stack developer, .NET backends, document vision" />

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&pause=1200&color=FF7A3C&center=true&vCenter=true&width=680&lines=I+build+systems+that+have+to+work+outside+the+demo.;.NET+backends+%7C+retail+platforms+%7C+document+vision;AI+writes+code.+I+own+the+architecture+and+the+diffs.;Shipped+beats+perfect." alt="I build systems that have to work outside the demo" />
</a>

<br/><br/>

<a href="https://walidmoustafa2077.github.io"><img src="assets/icons/globe-accent.svg" height="18" alt="" />&nbsp;Portfolio</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/walidmoustafa2077"><img src="assets/icons/github-accent.svg" height="18" alt="" />&nbsp;GitHub</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://linkedin.com/in/walidmostafa77"><img src="assets/icons/linkedin-accent.svg" height="18" alt="" />&nbsp;LinkedIn</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="mailto:walidmostafa2077@gmail.com"><img src="assets/icons/envelope-accent.svg" height="18" alt="" />&nbsp;Email</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://stackoverflow.com/users/walid-mostafa"><img src="assets/icons/stack-overflow-accent.svg" height="18" alt="" />&nbsp;Stack Overflow</a>

<br/><br/>

<sub>
<a href="#-about">About</a> &nbsp;·&nbsp;
<a href="#-featured-work">Work</a> &nbsp;·&nbsp;
<a href="#-document-vision-pipeline">Pipeline</a> &nbsp;·&nbsp;
<a href="#-also-building">More</a> &nbsp;·&nbsp;
<a href="#-tech-stack">Stack</a> &nbsp;·&nbsp;
<a href="#-github-stats">Stats</a>
</sub>

</div>

<br/>

## <img src="assets/icons/user-accent2.svg" height="24" alt="" />&nbsp; About

I build the parts of a product that never make it to the landing page: **auth, payments, migrations, deploys**. Backend first, in C# and Python. I keep scope small enough to finish and tests honest enough to trust, then ship the thing.

> **Shipped beats perfect.**

| | |
|:---|:---|
| <img src="assets/icons/server-accent.svg" height="16" alt="" />&nbsp; **Backend** | C# and Python. ASP.NET Core, .NET 9/10, EF Core, minimal APIs |
| <img src="assets/icons/file-image-accent.svg" height="16" alt="" />&nbsp; **Document Vision** | Corner detection, dewarping, shadow removal, and the synthetic datasets that train them |
| <img src="assets/icons/layer-group-accent.svg" height="16" alt="" />&nbsp; **Full stack** | WPF or React/Next.js on the client, Docker and GitHub Actions on the way out |
| <img src="assets/icons/robot-accent.svg" height="16" alt="" />&nbsp; **AI-assisted** | The typing got faster. The judgement stayed mine |
| <img src="assets/icons/graduation-cap-accent.svg" height="16" alt="" />&nbsp; **Learning** | Bachelor's in BIS, plus Microsoft, Meta, and IBM certifications |

<br/>

## <img src="assets/icons/rocket-accent2.svg" height="24" alt="" />&nbsp; Featured Work

<table>
<tr>
<td width="50%" valign="top">

### <img src="assets/icons/file-image-accent.svg" height="20" alt="" />&nbsp; Document Vision
Small, focused models that turn a **phone photo into a clean scan**: detect → dewarp → remove shadows → export.

`PyTorch` `ONNX` `.NET` `Blender`

[PaperMask](https://github.com/walidmoustafa2077/PaperMask) · [Details below ↓](#-document-vision-pipeline)

</td>
<td width="50%" valign="top">

### <img src="assets/icons/microphone-lines-accent.svg" height="20" alt="" />&nbsp; Voice Agent
A local phone-call loop you can **interrupt mid-sentence**. Barge-in at ~250 ms, audio never leaves the machine.

`Silero VAD` `Zipformer` `Ollama` `SignalR`

[Source](https://github.com/walidmoustafa2077/voice-agent)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### <img src="assets/icons/cash-register-accent.svg" height="20" alt="" />&nbsp; NexaPOS
Retail point of sale: a **.NET 9 API** (products, sales, carts, inventory) and a **WPF counter client**. JWT auth with Admin, Manager, and Cashier roles.

`ASP.NET Core` `EF Core` `WPF` `MVVM`

<sub>Private</sub>

</td>
<td width="50%" valign="top">

### <img src="assets/icons/mosque-accent.svg" height="20" alt="" />&nbsp; Tathkīr
Windows prayer companion: multi-location times, Hijri calendar, tray widget, athkar, and Qur'an with **100+ reciters**. RTL, localization, dynamic theming.

`WPF` `HttpClient` `Docker` `ASP.NET Core`

[Source](https://github.com/walidmoustafa2077/Tathkir)

</td>
</tr>
<tr>
<td colspan="2" valign="top">

### <img src="assets/icons/file-invoice-accent.svg" height="20" alt="" />&nbsp; NexaCV <sub>(private)</sub>
Subscription CV builder where the boring parts are the product: **Paddle billing** (checkout, webhooks, customer portal, subscription sync), ATS-friendly exports, a documented design system, and **Playwright** coverage across the Next.js app.

`Next.js` `Paddle` `Playwright`

</td>
</tr>
</table>

<br/>

## <img src="assets/icons/wand-magic-sparkles-accent2.svg" height="24" alt="" />&nbsp; Document Vision Pipeline

<p align="center">
  <img src="assets/pipeline.svg" width="880" alt="Detect → dewarp → clean → ship: PaperMask, DocDewarper-Lite, DocShadow-Lite, exported to ONNX for .NET" />
</p>

Each stage is a **small model with one job**, exported to ONNX so the .NET app can run it offline. The hard part is never the architecture — it is the data, so the training pipeline is part of the product.

| Stage | Project | What it does |
|:---|:---|:---|
| <img src="assets/icons/crosshairs-accent.svg" height="15" alt="" />&nbsp; **Detect** | [**PaperMask**](https://github.com/walidmoustafa2077/PaperMask) | MobileNetV3-Small + Lite-FPN, heatmap head with sub-pixel offsets, exported to ONNX (~1 MB) for .NET |
| <img src="assets/icons/draw-polygon-accent.svg" height="15" alt="" />&nbsp; **Dewarp** | [**DocDewarper-Lite**](https://github.com/walidmoustafa2077/DocDewarper-Lite) | UVDoc fine-tuned on NexaDoc 50K, with a Kaggle 2×T4 training notebook |
| <img src="assets/icons/circle-half-stroke-accent.svg" height="15" alt="" />&nbsp; **Clean** | [**DocShadow-Lite**](https://github.com/walidmoustafa2077/DocShadow-Lite) | Two-stage shadow removal: IOANet, then Laplacian-pyramid refinement |
| <img src="assets/icons/flask-accent.svg" height="15" alt="" />&nbsp; **Data** | [**Doc-Dataset-Generate**](https://github.com/walidmoustafa2077/Doc-Dataset-Generate) | SynDoc_Wild: synthetic shadows, camera degradation, perspective warp, plus a photorealistic Blender 4.2 pipeline |
| <img src="assets/icons/database-accent.svg" height="15" alt="" />&nbsp; **Dataset** | **NexaDoc 50K** | Published on Kaggle, the dataset behind the dewarping work |

<br/>

## <img src="assets/icons/toolbox-accent2.svg" height="24" alt="" />&nbsp; Also Building

| Project | Stack | What it is |
|:---|:---|:---|
| [**let-me-code**](https://github.com/walidmoustafa2077/let-me-code) | `Node.js` `MCP` | Agent factory for opencode: specialised subagents, workflow skills, and a delegation MCP server, installed with one command |
| [**termyx**](https://github.com/walidmoustafa2077/termyx) | `Rust` | Native terminal with first-class RTL support |
| [**RecycleBinTray**](https://github.com/walidmoustafa2077/RecycleBinTray) | `C#` `Win32` | Windows tray monitor: live item count and size, open or empty from a native menu |
| [**tasks-lite**](https://github.com/walidmoustafa2077/tasks-lite) | `Node.js` `JWT` | Task API with validation, clean errors, and Swagger docs |
| **store-system** <sub>(private)</sub> | `ASP.NET Core` `SQL Server` | Retail back office plus public storefront in one codebase: terminal, inventory, shifts, wallets, Paymob checkout |

<br/>

## <img src="assets/icons/screwdriver-wrench-accent2.svg" height="24" alt="" />&nbsp; Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=cs,dotnet,py,ts,js,react,nextjs,tailwind&perline=8" alt="C#, .NET, Python, TypeScript, JavaScript, React, Next.js, Tailwind" />
<br/>
<img src="https://skillicons.dev/icons?i=postgres,sqlite,docker,githubactions,git,pytorch,blender,visualstudio&perline=8" alt="PostgreSQL, SQLite, Docker, GitHub Actions, Git, PyTorch, Blender, Visual Studio" />

<sub><b>Also:</b> EF Core · SQL Server · SignalR · ONNX · Playwright · Ollama · WPF (MVVM)</sub>

</div>

<br/>

## <img src="assets/icons/magnifying-glass-accent2.svg" height="24" alt="" />&nbsp; Currently Working On

- <img src="assets/icons/file-image-accent.svg" height="14" alt="" />&nbsp; Closing the document pipeline end to end
- <img src="assets/icons/cubes-accent.svg" height="14" alt="" />&nbsp; Small, local-first tools that keep working after the demo
- <img src="assets/icons/gears-accent.svg" height="14" alt="" />&nbsp; Cleaner .NET backends with minimal APIs, EF Core, and honest tests
- <img src="assets/icons/github-accent.svg" height="14" alt="" />&nbsp; Automating builds and releases with GitHub Actions

<br/>

## <img src="assets/icons/certificate-accent2.svg" height="24" alt="" />&nbsp; Certifications

<div align="center">

![Microsoft](https://img.shields.io/badge/Microsoft-C%23_%26_Back--End-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![IBM](https://img.shields.io/badge/IBM-Software_Eng._%26_Git-052FAD?style=flat-square&logo=ibm&logoColor=white)
![Meta](https://img.shields.io/badge/Meta-Front--End-0866FF?style=flat-square&logo=meta&logoColor=white)

</div>

<br/>

## <img src="assets/icons/chart-simple-accent2.svg" height="24" alt="" />&nbsp; GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=walidmoustafa2077&show_icons=true&hide_border=true&bg_color=0A0705&title_color=FF5A1F&icon_color=FF7A3C&text_color=F4ECE2&count_private=true" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=walidmoustafa2077&layout=compact&hide_border=true&bg_color=0A0705&title_color=FF5A1F&text_color=F4ECE2&langs_count=8" alt="Top languages" />

<br/><br/>

<img height="165" src="https://streak-stats.demolab.com?user=walidmoustafa2077&hide_border=true&background=0A0705&ring=FF5A1F&fire=FF7A3C&currStreakNum=F4ECE2&sideNums=F4ECE2&currStreakLabel=FF5A1F&sideLabels=AB9D8F&dates=8B7D71" alt="Commit streak" />

</div>

<br/>

<div align="center">

<i>"Shipped beats perfect."</i>

<br/><br/>

<a href="mailto:walidmostafa2077@gmail.com"><img src="assets/icons/envelope-accent.svg" height="18" alt="" />&nbsp;<b>walidmostafa2077@gmail.com</b></a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://walidmoustafa2077.github.io"><img src="assets/icons/globe-accent.svg" height="18" alt="" />&nbsp;walidmoustafa2077.github.io</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF5A1F,50:9A3412,100:3B1A0B&height=120&section=footer" width="100%" alt="" />

</div>
