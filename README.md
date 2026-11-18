<!--
  Visual system: https://walidmoustafa2077.github.io (2026)
    bg #0A0705 · panel #15100B · paper #F4ECE2 · muted #AB9D8F · dim #8B7D71 · accent #FF5A1F
    Playfair-style serif display · Inter UI · IBM Plex Mono labels
  The banner and diagram ship in dark and light variants; <picture> picks the one that matches the page.
  Icons are Font Awesome Free 6.7.2 (CC BY 4.0 — fontawesome.com/license/free),
  recolored to accent (#FF5A1F) and muted (#8B7D71): assets/icons/<icon>-accent.svg / <icon>-muted.svg
-->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img src="assets/header-light.svg" width="100%" alt="Walid Mostafa, full-stack developer. Ships systems, not demos. Egypt, remote.">
</picture>

<div align="center">

<p>
<a href="https://walidmoustafa2077.github.io"><img src="assets/icons/globe-accent.svg" height="15" alt="">&nbsp;Portfolio</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/walidmoustafa2077"><img src="assets/icons/github-accent.svg" height="15" alt="">&nbsp;GitHub</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://linkedin.com/in/walidmostafa77"><img src="assets/icons/linkedin-accent.svg" height="15" alt="">&nbsp;LinkedIn</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="mailto:walidmostafa2077@gmail.com"><img src="assets/icons/envelope-accent.svg" height="15" alt="">&nbsp;Email</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://stackoverflow.com/users/walid-mostafa"><img src="assets/icons/stack-overflow-accent.svg" height="15" alt="">&nbsp;Stack Overflow</a>
</p>

<p><sub>
<a href="#-about">About</a> &nbsp;·&nbsp;
<a href="#-featured-work">Work</a> &nbsp;·&nbsp;
<a href="#-document-vision-pipeline">Pipeline</a> &nbsp;·&nbsp;
<a href="#-also-building">More</a> &nbsp;·&nbsp;
<a href="#-tech-stack">Stack</a> &nbsp;·&nbsp;
<a href="#-github-stats">Stats</a>
</sub></p>

</div>

## <img src="assets/icons/user-accent.svg" height="22" alt="">&nbsp; About

I build the parts of a product that never make it to the landing page: **auth, payments, migrations, deploys**. Backend first, in C# and Python. I keep scope small enough to finish and tests honest enough to trust, then ship the thing.

The typing got faster. The judgement stayed mine.

> **Read the diff. Ship the system.**

<sub><img src="assets/icons/globe-muted.svg" height="13" alt="">&nbsp; Egypt, remote &nbsp;·&nbsp; open to backend and full-stack work &nbsp;·&nbsp; BSc in Business Information Systems</sub>

## <img src="assets/icons/rocket-accent.svg" height="22" alt="">&nbsp; Featured Work

<table>
<tr>
<td width="50%" valign="top">

### <img src="assets/icons/file-image-accent.svg" height="18" alt="">&nbsp; Document Vision

Small, focused models that turn a **phone photo into a clean scan**: detect → dewarp → remove shadows → export.

`PyTorch` `ONNX` `.NET` `Blender`

[PaperMask](https://github.com/walidmoustafa2077/PaperMask) · [Details below ↓](#-document-vision-pipeline)

</td>
<td width="50%" valign="top">

### <img src="assets/icons/microphone-lines-accent.svg" height="18" alt="">&nbsp; Voice Agent

A local phone-call loop you can **interrupt mid-sentence**. Barge-in at ~250 ms, audio never leaves the machine.

`Silero VAD` `Zipformer` `Ollama` `SignalR`

[Source](https://github.com/walidmoustafa2077/voice-agent)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### <img src="assets/icons/cash-register-accent.svg" height="18" alt="">&nbsp; NexaPOS

Retail point of sale: a **.NET 9 API** (products, sales, carts, inventory) and a **WPF counter client**. JWT auth with Admin, Manager, and Cashier roles.

`ASP.NET Core` `EF Core` `WPF` `MVVM`

<sub>Private</sub>

</td>
<td width="50%" valign="top">

### <img src="assets/icons/mosque-accent.svg" height="18" alt="">&nbsp; Tathkīr

Windows prayer companion: multi-location times, Hijri calendar, tray widget, athkar, and Qur'an with **100+ reciters**. RTL, localization, dynamic theming.

`WPF` `HttpClient` `Docker` `ASP.NET Core`

[Source](https://github.com/walidmoustafa2077/Tathkir)

</td>
</tr>
<tr>
<td colspan="2" valign="top">

### <img src="assets/icons/file-invoice-accent.svg" height="18" alt="">&nbsp; NexaCV <sub>(private)</sub>

Subscription CV builder where the boring parts are the product: **Paddle billing** (checkout, webhooks, customer portal, subscription sync), ATS-friendly exports, a documented design system, and **Playwright** coverage across the Next.js app.

`Next.js` `Paddle` `Playwright`

</td>
</tr>
</table>

## <img src="assets/icons/wand-magic-sparkles-accent.svg" height="22" alt="">&nbsp; Document Vision Pipeline

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/pipeline-dark.svg">
    <img src="assets/pipeline-light.svg" width="100%" alt="Detect, dewarp, clean, ship: PaperMask, DocDewarper-Lite, DocShadow-Lite, exported to ONNX for .NET">
  </picture>
</p>

Each stage is a **small model with one job**, exported to ONNX so the .NET app can run it offline. The hard part is never the architecture — it is the data, so the training pipeline is part of the product.

<table>
  <tr>
    <th width="118" align="left">Stage</th>
    <th width="220" align="left">Project</th>
    <th align="left">What it does</th>
  </tr>
  <tr>
    <td><img src="assets/icons/crosshairs-muted.svg" height="14" alt="">&nbsp; <b>Detect</b></td>
    <td><a href="https://github.com/walidmoustafa2077/PaperMask"><b>PaperMask</b></a></td>
    <td>MobileNetV3-Small + Lite-FPN, heatmap head with sub-pixel offsets, exported to ONNX (~1 MB) for .NET</td>
  </tr>
  <tr>
    <td><img src="assets/icons/draw-polygon-muted.svg" height="14" alt="">&nbsp; <b>Dewarp</b></td>
    <td><a href="https://github.com/walidmoustafa2077/DocDewarper-Lite"><b>DocDewarper-Lite</b></a></td>
    <td>UVDoc fine-tuned on NexaDoc 50K, with a Kaggle 2×T4 training notebook</td>
  </tr>
  <tr>
    <td><img src="assets/icons/circle-half-stroke-muted.svg" height="14" alt="">&nbsp; <b>Clean</b></td>
    <td><a href="https://github.com/walidmoustafa2077/DocShadow-Lite"><b>DocShadow-Lite</b></a></td>
    <td>Two-stage shadow removal: IOANet, then Laplacian-pyramid refinement</td>
  </tr>
  <tr>
    <td><img src="assets/icons/flask-muted.svg" height="14" alt="">&nbsp; <b>Data</b></td>
    <td><a href="https://github.com/walidmoustafa2077/Doc-Dataset-Generate"><b>Doc-Dataset-Generate</b></a></td>
    <td>SynDoc_Wild: synthetic shadows, camera degradation, perspective warp, plus a photorealistic Blender 4.2 pipeline</td>
  </tr>
  <tr>
    <td><img src="assets/icons/database-muted.svg" height="14" alt="">&nbsp; <b>Dataset</b></td>
    <td><b>NexaDoc 50K</b></td>
    <td>Published on Kaggle, the dataset behind the dewarping work</td>
  </tr>
</table>

## <img src="assets/icons/toolbox-accent.svg" height="22" alt="">&nbsp; Also Building

<table>
  <tr>
    <th width="170" align="left">Project</th>
    <th width="170" align="left">Stack</th>
    <th align="left">What it is</th>
  </tr>
  <tr>
    <td><a href="https://github.com/walidmoustafa2077/let-me-code"><b>let-me-code</b></a></td>
    <td><code>Node.js</code> <code>MCP</code></td>
    <td>Agent factory for opencode: specialised subagents, workflow skills, and a delegation MCP server, installed with one command</td>
  </tr>
  <tr>
    <td><a href="https://github.com/walidmoustafa2077/termyx"><b>termyx</b></a></td>
    <td><code>Rust</code></td>
    <td>Native terminal with first-class RTL support</td>
  </tr>
  <tr>
    <td><a href="https://github.com/walidmoustafa2077/RecycleBinTray"><b>RecycleBinTray</b></a></td>
    <td><code>C#</code> <code>Win32</code></td>
    <td>Windows tray monitor: live item count and size, open or empty from a native menu</td>
  </tr>
  <tr>
    <td><a href="https://github.com/walidmoustafa2077/tasks-lite"><b>tasks-lite</b></a></td>
    <td><code>Node.js</code> <code>JWT</code></td>
    <td>Task API with validation, clean errors, and Swagger docs</td>
  </tr>
  <tr>
    <td><b>store-system</b> <sub>(private)</sub></td>
    <td><code>ASP.NET Core</code> <code>SQL Server</code></td>
    <td>Retail back office plus public storefront in one codebase: terminal, inventory, shifts, wallets, Paymob checkout</td>
  </tr>
</table>

## <img src="assets/icons/screwdriver-wrench-accent.svg" height="22" alt="">&nbsp; Tech Stack

<p>
<b>Languages</b> — C# · Python · TypeScript · JavaScript · Rust · SQL<br/>
<b>Backend</b> — ASP.NET Core · .NET 9 / 10 · EF Core · Minimal APIs · SignalR<br/>
<b>Frontend</b> — React · Next.js · Tailwind · WPF (MVVM)<br/>
<b>Data &amp; ML</b> — PyTorch · ONNX · PostgreSQL · SQL Server · SQLite<br/>
<b>Ship</b> — Docker · GitHub Actions · Playwright · Git · Blender
</p>

## <img src="assets/icons/magnifying-glass-accent.svg" height="22" alt="">&nbsp; Currently Working On

- Closing the document pipeline end to end
- Small, local-first tools that keep working after the demo
- Cleaner .NET backends with minimal APIs, EF Core, and honest tests
- Automating builds and releases with GitHub Actions

## <img src="assets/icons/certificate-accent.svg" height="22" alt="">&nbsp; Certifications

<p align="center"><sub><b>Microsoft</b> — C# &amp; back-end &nbsp;·&nbsp; <b>IBM</b> — software engineering &amp; Git &nbsp;·&nbsp; <b>Meta</b> — front-end</sub></p>

## <img src="assets/icons/chart-simple-accent.svg" height="22" alt="">&nbsp; GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=walidmoustafa2077&show_icons=true&hide_border=true&bg_color=0A0705&title_color=FF5A1F&icon_color=FF7A3C&text_color=F4ECE2&count_private=true&border_radius=10" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=walidmoustafa2077&layout=compact&hide_border=true&bg_color=0A0705&title_color=FF5A1F&text_color=F4ECE2&border_radius=10&langs_count=8" alt="Top languages">
</p>

<p align="center">
  <img height="165" src="https://streak-stats.demolab.com?user=walidmoustafa2077&hide_border=true&background=0A0705&ring=FF5A1F&fire=FF7A3C&currStreakNum=F4ECE2&sideNums=F4ECE2&currStreakLabel=FF5A1F&sideLabels=AB9D8F&dates=8B7D71&border_radius=10" alt="Commit streak">
</p>

---

<p align="center"><i>Shipped beats perfect.</i></p>

<p align="center">
<a href="mailto:walidmostafa2077@gmail.com"><img src="assets/icons/envelope-accent.svg" height="15" alt="">&nbsp;<b>walidmostafa2077@gmail.com</b></a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://walidmoustafa2077.github.io"><img src="assets/icons/globe-accent.svg" height="15" alt="">&nbsp;walidmoustafa2077.github.io</a>
</p>

<p align="center"><sub>© 2026 Walid Mostafa · C# · .NET · TypeScript · Python</sub></p>
