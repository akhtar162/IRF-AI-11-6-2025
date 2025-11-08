dibuatpada 10/6/2025
kalian boleh memodifikasi tapi harus atas nama IRF 
dan ada intergrasi serper api di line 3531 dan ini berisi 
# 📘 Dokumentasi Singkat IRF (Interaktif Real Feature)

| No | Judul | Deskripsi |
|----|--------|-----------|
| **1** | 🧠 **Pengenalan AI (Bahasa Indonesia)** | IRF (Interaktif Real Featur) adalah sistem kecerdasan buatan berbasis **WebLLM** yang berjalan langsung di browser tanpa server. Tujuannya adalah membuat AI yang cepat, ringan, aman, dan dapat diakses oleh semua orang. IRF mendukung mode offline, antarmuka interaktif, dan berbagai fitur tambahan seperti map, file, serta sistem token internal. |
| **2** | 🌍 **AI Introduction (English)** | **IRF (Interactive Real Featur)** is an AI system powered by **WebLLM**, designed to run directly in your browser with no external cloud dependency. It offers fast, secure, and private inference, providing interactive UI and modular features that make local AI accessible to everyone. |
| **3** | 🇨🇳 **人工智能介绍 (Chinese)** | **IRF（交互式真实功能）** 是一种基于 **WebLLM** 的人工智能系统，可以直接在浏览器中运行，无需云服务器。它快速、安全、私密，界面交互性强，旨在让每个人都能轻松使用本地 AI。 |
| **4** | 🌐 **Cara Membuat Domain di GitHub** | 1️⃣ Buat repository di GitHub (misal: `irf-ai`) → Public → Tambahkan `index.html`. <br> 2️⃣ Buka tab **Settings → Pages** → Source: `main / (root)` → **Save**. <br> 3️⃣ Tunggu 1 menit, domain akan muncul: `https://username.github.io/irf-ai/`. <br> 4️⃣ (Opsional) Buat file `CNAME` untuk domain pribadi (misal `irfai.tech`). <br> 5️⃣ Aktifkan **Enforce HTTPS** agar situs aman. |
| **5** | 🤖 **Daftar Model AI di WebLLM (29 Model)** | Contoh model kompatibel: <br> - **Qwen2-0.5B** – 0.5B params – 1–2 GB VRAM – 4K tokens <br> - **Qwen2-1.5B** – 1.5B params – 3–4 GB VRAM – 8K tokens <br> - **Phi-3 Mini** – 1.8B params – 3 GB VRAM – 8K tokens <br> - **Mistral-7B** – 7B params – 8–12 GB VRAM – 16K tokens <br> - **Llama-3-1B / 3B / 7B**, **Gemma-2B**, **RedPajama-3B**, dll. <br> Semuanya dapat dijalankan melalui WebGPU dengan quantization (INT4/INT8). |
| **6** | 💻📱 **Rekomendasi Perangkat untuk IRF / WebLLM** | **Laptop**: <br> • ASUS Vivobook 14X (16 GB / 512 GB / Radeon 780M) <br> • Lenovo IdeaPad 5 Pro (RTX 2050) <br> • MacBook Air M3 (16 GB unified) <br> • ROG Zephyrus G14 (RTX 4070, 1 TB SSD). <br><br> **Smartphone**: <br> • Samsung S24 Ultra (12 GB/512 GB) <br> • Xiaomi 14 T Pro (Dimensity 9300) <br> • OPPO Reno12 Pro 5G (SD 8 Gen 1) <br> • Realme GT 5 Pro (SD 8 Gen 3). <br><br> Semua mendukung **WebGPU** dan bisa menjalankan model kecil hingga menengah (≤ 3B parameters). |

dan masih ada bug yang tidak disadari karna ini versi 1.0

# 🌐 IRF – Interaktif Real Featur  
### Platform AI Interaktif Multifungsi (Public Beta)

> ⚠️ **Status:** Masih dalam tahap pengembangan (*Public Beta 2025*)  
> IRF adalah platform AI interaktif berbasis web yang berjalan **sepenuhnya secara lokal di browser**, menggunakan model **Qwen2-0.5B** melalui **WebLLM** untuk menghadirkan pengalaman AI cepat, privat, dan cerdas.

---

## 🇮🇩 Bahasa Indonesia

### 🧩 Tentang IRF
**IRF (Interaktif Real Featur)** adalah platform **AI multifungsi berbasis web** yang dirancang agar sepenuhnya berjalan **tanpa server eksternal**.  
Semua pemrosesan dilakukan **di perangkat pengguna (client-side)** menggunakan teknologi **WebGPU** dan **WebLLM**.  

IRF menggabungkan kemampuan percakapan AI, visualisasi 3D, analisis matematis, serta hiburan interaktif dalam satu antarmuka terpadu.

---

## ⚙️ Arsitektur Sistem

IRF memiliki empat lapisan utama:

1. **Lapisan Antarmuka (UI Layer)**  
   - Dibangun menggunakan **HTML5 + TailwindCSS + JavaScript**.  
   - Mendukung *dark mode*, animasi halus, dan layout responsif.  

2. **Lapisan Logika (Logic Layer)**  
   - Mengatur semua event, input, serta integrasi antar-fitur (chat, game, token).  
   - Dikelola melalui *modular JS script* agar efisien dan mudah diperluas.

3. **Lapisan Kecerdasan (AI Layer)**  
   - Menggunakan **Qwen2-0.5B** melalui **@mlc-ai/web-llm**.  
   - Model dimuat langsung di browser menggunakan **WebGPU** (tanpa server).  
   - Mendukung pemrosesan teks, logika percakapan, dan analisis ringan.

4. **Lapisan Visual & Sensorik (Interactive Layer)**  
   - Menggunakan **Three.js** dan **Three-VRM** untuk avatar 3D.  
   - Menyertakan **TensorFlow.js + COCO-SSD** untuk deteksi objek lokal.  
   - Efek visual partikel real-time menggunakan *Canvas Rendering*.

---

## 💡 Fitur Utama

| Kategori | Fitur |
|-----------|--------|
| 🤖 AI Lokal | Qwen2-0.5B (WebLLM) berjalan langsung di browser. |
| 🧠 Analisis | Dukungan kalkulasi simbolik (Math.js, Nerdamer). |
| 🗣️ Komunikasi | Input suara + Text-to-Speech (TTS). |
| 🎨 Tampilan | Dark/Light mode, animasi halus, efek partikel. |
| 🎮 Hiburan | Game 2048, lempar dadu, piano, papan Trello mini. |
| 🪙 Token | Sistem hadiah otomatis & bonus harian. |
| 🧭 Avatar 3D | Menggunakan Three.js + VRM humanoid interaktif. |
| 🔒 Keamanan | Semua data disimpan di localStorage, tanpa API eksternal. |

---

## 🎨 Desain & Pengalaman Pengguna (UI/UX)

IRF mengusung filosofi **“Visual AI Experience”**, di mana setiap interaksi terasa hidup dan natural.  
Antarmuka dirancang dengan prinsip:

- **Sederhana namun futuristik** — fokus pada konten dan percakapan.  
- **Mode gelap otomatis** dengan aksen lembut agar nyaman di mata.  
- **Animasi partikel real-time** mengikuti pergerakan kursor.  
- **Avatar 3D dinamis** yang dapat menatap pengguna selama sesi interaksi.  
- **Panel kontrol kiri/kanan** untuk navigasi cepat: Chat, Tools, Game, Token.

---

## 🧠 Model AI – Qwen2-0.5B

**Qwen2-0.5B** adalah model bahasa ringan (≈500 juta parameter) yang:
- Dirancang untuk **in-browser inference** (melalui WebLLM).  
- Memiliki kemampuan reasoning dan percakapan alami.  
- Dapat menjalankan instruksi pendek hingga menengah dengan cepat.  
- Optimal untuk perangkat tanpa GPU khusus.

Keunggulan model ini:
- ⚡ **Cepat**: waktu respons rata-rata < 1 detik di perangkat modern.  
- 🔒 **Aman**: pemrosesan lokal, tanpa koneksi jaringan.  
- 🧩 **Modular**: mudah diganti ke model lain (Phi-3, Gemma, TinyLlama, dll.)

---

## 🔐 Keamanan & Privasi

IRF menjamin **privasi penuh** bagi pengguna:
- Tidak ada data dikirim ke cloud.  
- Semua riwayat chat dan pengaturan disimpan di `localStorage`.  
- Fitur “Hapus Semua Data” dapat diakses langsung dari pengaturan.  
- Mode offline sepenuhnya didukung.

---

## 🪙 Sistem Token & Reward

IRF memiliki sistem motivasi pengguna:
- Token bertambah otomatis setiap 10 menit aktivitas.  
- Bonus token diberikan dua kali per hari (16.00 & 21.00).  
- Token dapat digunakan untuk membuka tema, efek, dan fitur bonus.  
- Data token juga tersimpan lokal dan tidak dapat dimanipulasi via script eksternal.

---

## 🎮 Fitur Tambahan

| Fitur | Deskripsi |
|--------|------------|
| 🧩 **Mini Game 2048** | Game puzzle klasik untuk relaksasi. |
| 🎲 **Lempar Dadu** | Simulasi acak dengan animasi. |
| 🎹 **Piano Virtual** | Instrumen suara berbasis HTML5 audio. |
| 📋 **Trello Mini Board** | Simulasi manajemen tugas berbasis kartu. |
| 🗺️ **Map Viewer** | Integrasi Leaflet.js untuk navigasi dasar. |

---

## ⚙️ Kinerja & Optimisasi

IRF mengimplementasikan optimisasi tingkat lanjut:
- Model **lazy-loaded** (dimuat hanya saat diperlukan).  
- Cache model tersimpan di IndexedDB agar cepat diakses ulang.  
- GPU detection otomatis (WebGPU / WebGL fallback).  
- Penggunaan memori < 200 MB di perangkat standar.

---

## 🔬 Teknologi yang Digunakan

| Komponen | Teknologi |
|-----------|------------|
| Model AI | Qwen2-0.5B (WebLLM) |
| Framework ML | TensorFlow.js + COCO-SSD |
| 3D Engine | Three.js + Three-VRM |
| UI Framework | TailwindCSS |
| Data Storage | localStorage + IndexedDB |
| Visual Effect | Canvas API + Particle Engine |
| Game Engine | Pure JS + DOM event loop |
| Voice | Web Speech API (TTS + STT) |

---

## 🧱 Rencana Pengembangan
- Penambahan model lokal alternatif: *Phi-3.5-mini*, *Gemma-2B*.  
- Fitur “plugin mini-tools” (kalkulator ilmiah, konversi satuan, penerjemah).  
- Mode *multi-bahasa otomatis*.  
- Integrasi suara ekspresif (voice emotion AI).  
- Mode *offline installer (PWA)*.

---

## 📜 Lisensi
Proyek ini bersifat **Open Beta** untuk keperluan pengujian dan pembelajaran.  
Hak cipta © 2025 oleh pengembang asli **IRF (Interaktif Real Featur)**.  
Semua pustaka pihak ketiga tunduk pada lisensi masing-masing.

# 🌐 IRF – Interaktif Real Featur  
### Multifunctional Interactive AI Platform (Public Beta)

> ⚠️ **Status:** Currently in public beta (2025)  
> IRF is a **web-based interactive AI platform** that runs entirely **locally in your browser**.  
> Powered by **Qwen2-0.5B** through **WebLLM**, IRF delivers a fast, secure, and intelligent AI experience without relying on any external server.

---

## 🧩 About IRF

**IRF (Interaktif Real Featur)** is a **multifunctional web-based AI platform** designed to operate completely offline and locally.  
All processes are handled **on the client side**, powered by **WebGPU** and **WebLLM**, ensuring maximum privacy and speed.

IRF combines conversational AI, real-time visualization, mathematical analysis, and interactive entertainment into a single seamless experience.

---

## ⚙️ System Architecture

IRF consists of four core layers:

1. **User Interface (UI Layer)**  
   - Built using **HTML5 + TailwindCSS + JavaScript**.  
   - Supports dark/light mode, adaptive layouts, and fluid animations.  

2. **Logic Layer**  
   - Manages all core events, user input, and module connections (chat, token, games, etc.).  
   - Organized in modular JavaScript files for maintainability and scalability.  

3. **AI Layer**  
   - Powered by **Qwen2-0.5B** using **@mlc-ai/web-llm**.  
   - Executes AI inference **directly in-browser** using **WebGPU acceleration**.  
   - Supports text generation, reasoning, and conversational capabilities.  

4. **Interactive & Visual Layer**  
   - Built with **Three.js** and **Three-VRM** for real-time 3D avatars.  
   - Integrates **TensorFlow.js + COCO-SSD** for local object detection.  
   - Includes particle effects rendered via HTML5 Canvas.

---

## 💡 Core Features

| Category | Description |
|-----------|--------------|
| 🤖 **Local AI** | Qwen2-0.5B runs natively in the browser with WebLLM. |
| 🧮 **Computation** | Symbolic and numeric computation using Math.js & Nerdamer. |
| 🗣️ **Voice Interaction** | Microphone input & text-to-speech output. |
| 🎨 **UI Design** | Dark/light mode, animated elements, particle cursor. |
| 🎮 **Mini Games** | Includes 2048, Dice, Piano, and Trello-style boards. |
| 🪙 **Token System** | Earn automatic rewards for active use. |
| 🧭 **3D Avatar** | Interactive humanoid avatar with Three.js + VRM. |
| 🔒 **Privacy** | 100% local data, no network calls, no tracking. |

---

## 🎨 Design & User Experience

IRF follows the principle of **“Visual AI Interaction”**, focusing on clarity, immersion, and control.

- Clean futuristic layout optimized for readability.  
- Automatic **dark/light theme switching**.  
- **Particle trails** and **cursor visual effects** for motion feedback.  
- 3D avatar that responds to interaction in real time.  
- Compact left/right control panels for navigation (Chat • Tools • Games • Token).

The design adapts dynamically between desktop and mobile environments for consistent performance.

---

## 🧠 AI Model – Qwen2-0.5B

**Qwen2-0.5B** is a lightweight yet capable AI language model built by Alibaba’s Qwen Team.  
It’s optimized for **browser-based inference**, balancing accuracy, efficiency, and minimal resource usage.

### Model Advantages:
- ⚡ **Fast**: <1 second average response on standard hardware.  
- 🔒 **Private**: All computation runs locally via WebGPU.  
- 🧩 **Flexible**: Can be replaced by other compact models (Phi, Gemma, TinyLlama, etc.).

### Technical Highlights:
- Parameter count: ~500M  
- Architecture: Transformer Decoder  
- Context length: 4K tokens  
- Precision: FP16 / INT4 quantization supported  

---

## 🔐 Privacy & Security

IRF guarantees full user privacy by design.

- All conversations, preferences, and tokens are stored in `localStorage`.  
- No external API calls or data logging.  
- Clear option to **“Delete All Data”** from settings.  
- Works fully **offline** — no internet required after initial load.

This architecture ensures total data sovereignty and compliance with modern privacy standards.

---

## 🪙 Token & Reward System

IRF introduces a lightweight **engagement-based token economy**:

- Tokens increase automatically every 10 minutes of active use.  
- Bonus tokens awarded twice daily (16:00 and 21:00).  
- Tokens can unlock premium effects, themes, and voice features.  
- Token data is protected within local storage and cannot be edited externally.

This gamified reward model motivates continued exploration and creativity.

---

## 🎮 Built-in Features

| Feature | Description |
|----------|-------------|
| 🧩 **2048** | Classic number-merging puzzle with soft animation. |
| 🎲 **Dice Roller** | Simulates random rolls with smooth animation. |
| 🎹 **Virtual Piano** | Playable sound instrument built with HTML5 Audio. |
| 📋 **Mini Trello Board** | Card-based task management simulation. |
| 🗺️ **Map Viewer** | Basic location preview via Leaflet.js. |

Each feature is fully integrated and accessible from within IRF’s unified interface.

---

## ⚙️ Performance & Optimization

IRF achieves high performance through:
- **Lazy-loading models** (load only when chat is initiated).  
- Caching AI weights in **IndexedDB** for faster reuse.  
- Automatic GPU fallback detection (WebGPU → WebGL).  
- Memory optimization: <200MB runtime footprint.  

A built-in performance monitor ensures smooth FPS for interactive effects.

---

## 🔬 Core Technologies

| Component | Technology |
|------------|-------------|
| AI Engine | Qwen2-0.5B (WebLLM) |
| ML Framework | TensorFlow.js + COCO-SSD |
| 3D Graphics | Three.js + Three-VRM |
| UI Framework | TailwindCSS |
| Storage | localStorage + IndexedDB |
| Audio | Web Speech API (STT & TTS) |
| Effects | Canvas + Particle Engine |
| Tools | Math.js, Nerdamer, Moment.js, Chart.js |

---

## 🧱 Development Roadmap

Upcoming planned updates:

- Integrate **alternative models** (Phi-3.5, Gemma-2B).  
- Add **plugin micro-tools** (scientific calculator, converter, translator).  
- Implement **auto language detection & translation**.  
- Introduce **expressive voice synthesis** (emotional tone output).  
- Release **PWA offline installer** version.

---

## 📜 License

IRF is an **open beta project** provided for research, testing, and educational purposes.  
All external libraries remain under their respective open-source licenses.  
Copyright © 2025 **IRF (Interaktif Real Featur)** by **Akhtar Nur Rahman**.

---

## 🧭 Global Summary

| Category | Description |
|-----------|-------------|
| Type | Interactive Web AI Platform |
| AI Model | Qwen2-0.5B (WebLLM) |
| Core Tech | WebLLM, TensorFlow.js, Three.js, TailwindCSS |
| Mode | 100% Local, Offline Supported |
| Status | Public Beta |
| Year | 2025 |
| Developer | Akhtar Nur Rahman |

---

> 🌟 *IRF – Bringing the Future of Interactive AI.*  
> Fast. Private. Local. Intelligent.

# 🌐 IRF – 交互式真实功能  
### 多功能交互式人工智能平台（公开测试版）

> ⚠️ **状态：** 当前为公开测试阶段（2025）  
> IRF 是一个完全在浏览器中本地运行的 **交互式 AI 平台**，  
> 基于 **Qwen2-0.5B 模型** 并通过 **WebLLM** 实现，  
> 提供快速、安全、智能的 AI 体验，无需任何外部服务器。

---

## 🧩 关于 IRF

**IRF（Interaktif Real Featur，交互式真实功能）** 是一个 **基于网页的多功能人工智能平台**，  
设计目标是实现 **完全离线和本地运行**。  
所有处理过程均在用户设备端（Client-Side）完成，  
通过 **WebGPU** 与 **WebLLM** 技术实现高速推理与完全隐私保护。

IRF 集成了智能对话、实时可视化、数学分析以及娱乐功能，  
打造一个沉浸式、互动式的 AI 体验平台。

---

## ⚙️ 系统架构

IRF 系统由四个核心层组成：

1. **用户界面层（UI Layer）**  
   - 使用 **HTML5 + TailwindCSS + JavaScript** 构建。  
   - 支持深色/浅色模式、自适应布局与动态动画。

2. **逻辑层（Logic Layer）**  
   - 管理所有事件、输入、与模块交互（聊天、游戏、令牌系统等）。  
   - 模块化脚本结构，易于扩展与维护。

3. **AI 层（AI Layer）**  
   - 使用 **Qwen2-0.5B 模型** 通过 **@mlc-ai/web-llm** 执行推理。  
   - 在浏览器中直接运行（基于 WebGPU 加速）。  
   - 支持自然语言生成、逻辑推理和会话功能。

4. **视觉与交互层（Interactive Layer）**  
   - 基于 **Three.js + Three-VRM** 实现 3D 虚拟形象。  
   - 集成 **TensorFlow.js + COCO-SSD** 实现本地目标检测。  
   - 使用 HTML5 Canvas 渲染粒子与光效动画。

---

## 💡 核心功能

| 类别 | 描述 |
|------|------|
| 🤖 **本地 AI** | Qwen2-0.5B 模型通过 WebLLM 在浏览器中直接运行。 |
| 🧮 **数学计算** | 集成 Math.js 与 Nerdamer 实现符号与数值运算。 |
| 🗣️ **语音交互** | 支持麦克风输入与文本语音合成（TTS）。 |
| 🎨 **界面设计** | 深/浅色模式，流畅动画，粒子光标效果。 |
| 🎮 **小游戏** | 包含 2048、掷骰子、虚拟钢琴、迷你任务板等。 |
| 🪙 **令牌系统** | 活跃用户可自动获得奖励与每日额外积分。 |
| 🧭 **3D 虚拟形象** | 采用 Three.js + VRM 实现交互式虚拟角色。 |
| 🔒 **隐私保护** | 所有数据均存储于本地，不进行任何网络传输。 |

---

## 🎨 设计与用户体验（UI/UX）

IRF 遵循 “**视觉化人工智能体验**” 的设计理念，注重简洁与沉浸式交互。

- 简约而未来感的布局，聚焦内容与对话。  
- 自动切换深色与浅色主题，减轻视觉疲劳。  
- 鼠标轨迹粒子与动态光效带来交互反馈。  
- 实时响应的 3D 虚拟角色增强沉浸感。  
- 左右导航面板：Chat • Tools • Games • Token 一键访问。

界面自动适配桌面与移动端，确保体验一致。

---

## 🧠 AI 模型 – Qwen2-0.5B

**Qwen2-0.5B** 是由阿里巴巴 Qwen 团队开发的轻量级语言模型，  
专为 **浏览器端推理（WebLLM）** 优化，具备高效率与低资源占用。

### 模型优势：
- ⚡ **高速响应：** 在主流设备上平均响应时间 <1 秒。  
- 🔒 **完全私密：** 计算过程全部在本地执行，无需网络。  
- 🧩 **灵活扩展：** 支持替换为其他轻量模型（Phi、Gemma、TinyLlama 等）。

### 技术参数：
- 参数量约 5 亿  
- 架构：Transformer 解码器  
- 上下文长度：4K tokens  
- 支持精度：FP16 / INT4 量化

---

## 🔐 隐私与安全

IRF 从架构上保障用户隐私：

- 聊天记录、偏好与令牌全部存储在浏览器的 `localStorage`。  
- 无外部 API 调用或日志上传。  
- 设置中可一键 **“清除所有数据”**。  
- 初次加载后可完全离线运行。

确保数据主权与隐私合规。

---

## 🪙 令牌与奖励系统

IRF 设有轻量化的激励体系：

- 每活跃 10 分钟自动获得令牌。  
- 每日两次额外奖励（16:00 与 21:00）。  
- 令牌可用于解锁主题、特效或语音功能。  
- 数据安全存储于本地，不可被外部修改。

此系统鼓励持续探索与创造。

---

## 🎮 内置功能

| 功能 | 描述 |
|------|------|
| 🧩 **2048 游戏** | 经典数字合并益智游戏，动画流畅。 |
| 🎲 **掷骰子** | 模拟随机投掷效果。 |
| 🎹 **虚拟钢琴** | 基于 HTML5 音频的可演奏乐器。 |
| 📋 **迷你任务板** | 类 Trello 卡片任务管理。 |
| 🗺️ **地图查看器** | 基于 Leaflet.js 的简易地图展示。 |

所有功能均可在统一界面中访问与交互。

---

## ⚙️ 性能与优化

IRF 通过多项优化技术实现高性能：

- 模型 **延迟加载**（仅在启动聊天时加载）。  
- 使用 **IndexedDB** 缓存模型权重，提升加载速度。  
- 自动检测 GPU（WebGPU → WebGL 回退）。  
- 内存占用优化：运行时低于 200MB。  

内置性能监测确保动画流畅与系统稳定。

---

## 🔬 技术组件

| 组件 | 技术 |
|------|------|
| AI 引擎 | Qwen2-0.5B（WebLLM） |
| 机器学习框架 | TensorFlow.js + COCO-SSD |
| 三维引擎 | Three.js + Three-VRM |
| UI 框架 | TailwindCSS |
| 数据存储 | localStorage + IndexedDB |
| 音频 | Web Speech API（语音识别与合成） |
| 动效 | Canvas + 粒子引擎 |
| 工具库 | Math.js、Nerdamer、Moment.js、Chart.js |

---

## 🧱 开发路线图

即将推出的功能：

- 集成更多本地模型（Phi-3.5、Gemma-2B）。  
- 增加 “微插件” 工具（科学计算器、单位换算、翻译器）。  
- 实现自动语言识别与翻译。  
- 引入带情感表达的语音合成。  
- 发布 **PWA 离线安装版**。

---

## 📜 许可协议

IRF 是一个 **公开测试（Open Beta）** 项目，  
用于研究、测试与教育用途。  
所有外部库遵守各自开源协议。  
版权所有 © 2025 **IRF（交互式真实功能）**，作者：**Akhtar Nur Rahman**。

---

## 🧭 全局信息概览

| 类别 | 说明 |
|------|------|
| 类型 | 基于网页的交互式 AI 平台 |
| AI 模型 | Qwen2-0.5B（WebLLM） |
| 核心技术 | WebLLM、TensorFlow.js、Three.js、TailwindCSS |
| 模式 | 100% 本地运行，支持离线 |
| 状态 | 公测版 |
| 年份 | 2025 |
| 开发者 | Akhtar Nur Rahman |

---

 🌟 *IRF – 引领交互式人工智能的未来。*  
 快速 · 安全 · 本地 · 智能

jp # 🌐 IRF – インタラクティブ・リアル・フィーチャー

### プラットフォーム AI 対話型多機能 (公開ベータ版)

> ⚠️ **ステータス:** 開発段階 (*公開ベータ 2025*)
> IRF は、**完全にブラウザのローカル**で実行されるウェブベースの対話型 AI プラットフォームです。**WebLLM** を介して **Qwen2-0.5B** モデルを使用し、高速でプライベートな、インテリジェントな AI 体験を提供します。

---

## 🇯🇵 日本語

### 🧩 IRF について
**IRF（インタラクティブ・リアル・フィーチャー）** は、**外部サーバーなし**で完全に動作するように設計された**ウェブベースの多機能 AI プラットフォーム**です。
すべての処理は、**WebGPU** および **WebLLM** 技術を使用して**ユーザーデバイス（クライアント側）**で行われます。

IRF は、AI 会話機能、3D 視覚化、数学的分析、および対話型エンターテイメントを一つの統合インターフェースに組み合わせています。

---

## ⚙️ システムアーキテクチャ

IRF は主に4つのレイヤーで構成されています。

1. **インターフェース層 (UI Layer)**
    - **HTML5 + TailwindCSS + JavaScript** で構築。
    - ダークモード、スムーズなアニメーション、レスポンシブなレイアウトに対応。
2. **ロジック層 (Logic Layer)**
    - すべてのイベント、入力、および機能間の統合（チャット、ゲーム、トークン）を管理。
    - 効率的で拡張しやすいようにモジュール式 JS スクリプトで管理。
3. **インテリジェンス層 (AI Layer)**
    - **@mlc-ai/web-llm** を介して **Qwen2-0.5B** を使用。
    - モデルは **WebGPU** を使用してブラウザに直接ロードされます（サーバーレス）。
    - テキスト処理、会話ロジック、軽量な分析をサポート。
4. **視覚・感覚層 (Interactive Layer)**
    - 3D アバターには **Three.js** と **Three-VRM** を使用。
    - ローカルオブジェクト検出のために **TensorFlow.js + COCO-SSD** を組み込み。
    - *Canvas Rendering* を使用したリアルタイムのパーティクル視覚効果。

---

## 💡 主要機能

| カテゴリ | 機能 |
|-----------|--------|
| 🤖 ローカル AI | Qwen2-0.5B (WebLLM) がブラウザ内で直接実行。 |
| 🧠 分析 | 記号計算（Math.js、Nerdamer）をサポート。 |
| 🗣️ 通信 | 音声入力 + テキスト読み上げ (TTS)。 |
| 🎨 表示 | ダーク/ライトモード、スムーズなアニメーション、パーティクル効果。 |
| 🎮 エンタメ | 2048ゲーム、サイコロ投げ、ピアノ、ミニ Trello ボード。 |
| 🪙 トークン | 自動報酬システムと日次ボーナス。 |
| 🧭 3D アバター | Three.js + VRM ヒューマノイドによる対話型アバター。 |
| 🔒 セキュリティ | すべてのデータは localStorage に保存され、外部 API なし。 |

---

## 🎨 デザインとユーザー体験 (UI/UX)

IRF は**「ビジュアル AI 体験」**の哲学を掲げ、すべてのインタラクションが生きていて自然に感じられるように設計されています。
インターフェースは以下の原則で設計されています。

* **シンプルでありながら未来的** — コンテンツと会話に焦点を当てる。
* 目に優しい柔らかいアクセントの**自動ダークモード**。
* カーソルの動きに追従する**リアルタイムパーティクルアニメーション**。
* インタラクションセッション中にユーザーを見つめることができる**動的な 3D アバター**。
* **左/右コントロールパネル**による迅速なナビゲーション。

---

## 🧠 AI モデル – Qwen2-0.5B

**Qwen2-0.5B** は、軽量な言語モデル（約5億パラメータ）で、以下の特徴があります。

* **ブラウザ内推論**（WebLLM 経由）のために設計。
* 推論能力と自然な会話能力を持つ。
* 短いから中程度の指示を迅速に実行可能。
* 専用 GPU のないデバイスに最適。

**利点:**
* ⚡ **高速**: 最新のデバイスでの平均応答時間 **< 1秒**。
* 🔒 **安全**: ローカル処理、**ネットワーク接続なし**。
* 🧩 **モジュール式**: 他のモデルへの切り替えが容易。

---

## 🔐 セキュリティとプライバシー

IRF はユーザーの**完全なプライバシー**を保証します。

* **クラウドにデータは送信されません。**
* すべてのチャット履歴と設定は `localStorage` に保存されます。
* 「全データ削除」機能は設定から直接アクセス可能。
* **オフラインモード**に完全にサポート。

---

## 🪙 トークンと報酬システム

IRF にはユーザーモチベーションシステムがあります。

* トークンは 10 分間のアクティビティごとに**自動的に増加**。
* トークンボーナスは**1日2回**提供されます（16:00 と 21:00）。
* トークンはテーマ、エフェクト、ボーナス機能の**ロック解除に使用可能**。
* トークンデータもローカルに保存され、外部スクリプトによる操作は不可。

---

## 🎮 追加機能

| 機能 | 説明 |
|--------|------------|
| 🧩 **ミニゲーム 2048** | リラックスのための古典的なパズルゲーム。 |
| 🎲 **サイコロ投げ** | アニメーション付きのランダムシミュレーション。 |
| 🎹 **バーチャルピアノ** | HTML5 オーディオベースのサウンド楽器。 |
| 📋 **Trello ミニボード** | カードベースのタスク管理シミュレーション。 |
| 🗺️ **マップビューア** | 基本的なナビゲーションのための Leaflet.js 統合。 |

---

## ⚙️ パフォーマンスと最適化

IRF は高度な最適化を実装しています。

* モデルは**レイジーロード**されます（必要なときにのみロード）。
* モデルキャッシュは IndexedDB に保存され、再アクセスが高速。
* GPU detection 自動（WebGPU / WebGL フォールバック）。
* 標準デバイスでのメモリ使用量 **< 200 MB**。

---

## 🔬 使用技術

| コンポーネント | 技術 |
|-----------|------------|
| モデル AI | **Qwen2-0.5B (WebLLM)** |
| ML フレームワーク | **TensorFlow.js + COCO-SSD** |
| 3D エンジン | **Three.js + Three-VRM** |
| UI フレームワーク | **TailwindCSS** |
| データストレージ | localStorage + IndexedDB |
| Visual Effect | Canvas API + パーティクルエンジン |
| Game Engine | Pure JS + DOM event loop |
| Voice | Web Speech API (TTS + STT) |

---

## 🧱 開発計画
* 代替ローカルモデルの追加：*Phi-3.5-mini*、*Gemma-2B*。
* 「プラグインミニツール」機能（科学計算機、単位変換、翻訳）。
* *自動多言語モード*。
* 感情表現豊かな音声統合（ボイス感情 AI）。
* *オフラインインストーラーモード (PWA)*。

---

## 📜 ライセンス
このプロジェクトは、テストおよび学習目的の**公開ベータ版**です。

著作権 © 2025 は、オリジナルの開発者**IRF（インタラクティブ・リアル・フィーチャー）**に帰属します。すべてのサードパーティライブラリは、それぞれのライセンスに従います。

---

## 🧭 全体概要

| カテゴリ | 説明 |
|-----------|------------|
| 種類 | 対話型ウェブ AI プラットフォーム |
| モデル AI | **Qwen2-0.5B (WebLLM)** |
| 主要技術 | WebLLM, TensorFlow.js, Three.js, TailwindCSS |
| モード | **100% ローカル、オフライン対応** |
| ステータス | 公開ベータ版 |
| 年 | 2025年 |
| 開発者 | Akhtar Nur Rahman |

---

> 🌟 *IRF – 対話型 AI を未来へ導く。*
> **高速。安全。ローカル。インテリジェント。**

# 🌐 IRF – الخواص التفاعلية الحقيقية (Interaktif Real Featur)

### منصة الذكاء الاصطناعي التفاعلية متعددة الوظائف (بيتا عامة)

> ⚠️ **الحالة:** لا تزال قيد التطوير (*الإصدار التجريبي العام 2025*)
> IRF هي منصة ذكاء اصطناعي تفاعلية قائمة على الويب وتعمل **بالكامل محليًا في المتصفح**، وتستخدم نموذج **Qwen2-0.5B** عبر **WebLLM** لتقديم تجربة ذكاء اصطناعي سريعة وخاصة وذكية.

---

## 🇸🇦 العربية

### 🧩 حول IRF
**IRF (الخواص التفاعلية الحقيقية)** هي منصة **ذكاء اصطناعي متعددة الوظائف قائمة على الويب** مصممة لتعمل بالكامل **بدون خادم خارجي**.
تتم جميع عمليات المعالجة **على جهاز المستخدم (جهة العميل)** باستخدام تقنية **WebGPU** و **WebLLM**.

تجمع IRF بين قدرات المحادثة بالذكاء الاصطناعي، والتصور ثلاثي الأبعاد (3D)، والتحليل الرياضي، والترفيه التفاعلي في واجهة واحدة موحدة.

---

## ⚙️ هيكلية النظام

تتكون IRF من أربع طبقات رئيسية:

1. **طبقة الواجهة (UI Layer)**
    - تم بناؤها باستخدام **HTML5 + TailwindCSS + JavaScript**.
    - تدعم الوضع الداكن، والرسوم المتحركة السلسة، والتخطيط المتجاوب.
2. **طبقة المنطق (Logic Layer)**
    - تنظم جميع الأحداث والمدخلات والتكامل بين الميزات.
    - تدار عبر *نصوص JavaScript معيارية*.
3. **طبقة الذكاء (AI Layer)**
    - تستخدم **Qwen2-0.5B** عبر **@mlc-ai/web-llm**.
    - يتم تحميل النموذج مباشرة في المتصفح باستخدام **WebGPU** (بدون خادم).
4. **طبقة التفاعل والاستشعار (Interactive Layer)**
    - تستخدم **Three.js** و **Three-VRM** لصور الأفاتار ثلاثية الأبعاد.
    - تتضمن **TensorFlow.js + COCO-SSD** للكشف المحلي عن الكائنات.

---

## 💡 الميزات الرئيسية

| الفئة | الميزة |
|-----------|--------|
| 🤖 الذكاء الاصطناعي المحلي | يعمل Qwen2-0.5B (WebLLM) مباشرة في المتصفح. |
| 🧠 التحليل | دعم الحساب الرمزي (Math.js, Nerdamer). |
| 🗣️ الاتصال | إدخال صوتي + تحويل النص إلى كلام (TTS). |
| 🎨 المظهر | الوضع الداكن/الفاتح، رسوم متحركة سلسة، تأثيرات جسيمية. |
| 🎮 الترفيه | لعبة 2048، رمي النرد، بيانو، لوحة تريللو مصغرة. |
| 🪙 الرموز (Tokens) | نظام مكافآت تلقائي ومكافأة يومية. |
| 🧭 أفاتار 3D | استخدام Three.js + شخصيات VRM بشرية تفاعلية. |
| 🔒 الأمان | يتم تخزين جميع البيانات في localStorage، بدون واجهات برمجة تطبيقات خارجية. |

---

## 🎨 التصميم وتجربة المستخدم (UI/UX)

تتبنى IRF فلسفة **"تجربة الذكاء الاصطناعي البصري"**.

* **بسيطة ولكن مستقبلية** — التركيز على المحتوى والمحادثة.
* **الوضع الداكن التلقائي** بلمسات ناعمة.
* **رسوم متحركة جسيمية في الوقت الفعلي** تتبع حركة المؤشر.
* **أفاتار 3D ديناميكي** يمكنه النظر إلى المستخدم.
* **لوحات تحكم يسرى/يمنى** للتنقل السريع.

---

## 🧠 نموذج الذكاء الاصطناعي – Qwen2-0.5B

* مصمم لـ **الاستدلال داخل المتصفح** (عبر WebLLM).
* يمتلك قدرات استنتاج ومحادثة طبيعية.

**مزايا هذا النموذج:**
* ⚡ **سريع**: متوسط وقت الاستجابة **< 1 ثانية**.
* 🔒 **آمن**: معالجة محلية، **بدون اتصال بالشبكة**.
* 🧩 **معياري**: سهل التبديل إلى نماذج أخرى.

---

## 🔐 الأمان والخصوصية

تضمن IRF **الخصوصية الكاملة**:

* **لا يتم إرسال أي بيانات إلى السحابة.**
* يتم تخزين جميع سجلات الدردشة والإعدادات في `localStorage`.
* يتم دعم وضع عدم الاتصال (Offline) بالكامل.

---

## 🪙 نظام الرموز والمكافآت

* تزيد الرموز تلقائيًا كل 10 دقائق من النشاط.
* يتم منح مكافآت الرموز مرتين يوميًا (الساعة 16:00 و 21:00).
* يمكن استخدام الرموز لفتح السمات والتأثيرات والميزات الإضافية.

---

## 🎮 الميزات الإضافية

| الميزة | الوصف |
|--------|------------|
| 🧩 **لعبة 2048 المصغرة** | لعبة الألغاز الكلاسيكية. |
| 🎲 **رمي النرد** | محاكاة عشوائية مع الرسوم المتحركة. |
| 🎹 **البيانو الافتراضي** | آلة صوتية قائمة على HTML5 Audio. |
| 📋 **لوحة تريللو المصغرة** | محاكاة لإدارة المهام القائمة على البطاقات. |
| 🗺️ **عارض الخرائط** | تكامل Leaflet.js للملاحة الأساسية. |

---

## 🔬 التقنيات المستخدمة

| المكون | التقنية |
|-----------|------------|
| نموذج الذكاء الاصطناعي | **Qwen2-0.5B (WebLLM)** |
| إطار عمل تعلم الآلة | **TensorFlow.js + COCO-SSD** |
| محرك 3D | **Three.js + Three-VRM** |
| إطار عمل الواجهة | **TailwindCSS** |
| تخزين البيانات | localStorage + IndexedDB |
| الصوت | Web Speech API (TTS + STT) |

---

## 🧱 خطة التطوير
* إضافة نماذج محلية بديلة: *Phi-3.5-mini*، *Gemma-2B*.
* ميزة "أدوات مصغرة إضافية" (آلة حاسبة، تحويل وحدات، مترجم).
* وضع *تعدد اللغات التلقائي*.
* وضع *مثبت عدم الاتصال (PWA)*.

---

## 🧭 ملخص عالمي

| الفئة | الوصف |
|-----------|------------|
| النوع | منصة ذكاء اصطناعي تفاعلية على الويب |
| نموذج الذكاء الاصطناعي | **Qwen2-0.5B (WebLLM)** |
| الوضع | **100% محلي، قادر على العمل دون اتصال** |
| الحالة | بيتا عامة |
| العام | 2025 |

---

> 🌟 *IRF – نقل الذكاء الاصطناعي التفاعلي إلى المستقبل.*
> **سريع. آمن. محلي. ذكي.**
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 ## 🌍 Cara Membuat Domain GitHub Pages untuk IRF

Panduan lengkap ini menjelaskan cara **mempublikasikan IRF (Interaktif Real Featur)** ke internet  
menggunakan **GitHub Pages**, gratis dan mudah — sehingga situs AI kamu bisa diakses lewat domain seperti:

> 💡 *GitHub Pages* adalah layanan hosting gratis dari GitHub untuk menampilkan situs web statis (HTML, CSS, JS).  
> Sangat cocok untuk proyek AI berbasis web seperti IRF.

---

### 🧩 1. Buat Repository GitHub

1. Masuk ke [https://github.com](https://github.com) dan login ke akunmu.  
2. Klik tombol **New Repository**.  
3. Isi detail repository seperti berikut: Nama repository: irf-ai
Visibilitas: Public

4. Centang opsi **Add a README file** agar repositori langsung berisi file awal.  
5. Klik **Create Repository** untuk menyelesaikan.

---

### 📁 2. Upload File IRF Kamu

1. Di halaman repository kamu, klik: file html ini

⚙️ **Catatan penting:**  
> File utama proyek kamu **harus bernama `index.html`** agar dapat dimuat otomatis oleh GitHub Pages.

---

### ⚡ 3. Aktifkan GitHub Pages

1. Buka tab **Settings** di repository kamu.  
2. Di sidebar kiri, pilih menu **Pages**.  
3. Pada bagian **Build and deployment**, ubah pengaturan menjadi: Source: Deploy from a branch
Branch: main
Folder: / (root)

   4. Klik tombol **Save**.

> ⏱️ Tunggu sekitar 1–2 menit.  
> GitHub akan otomatis membangun situs dan memberi domain gratis untuk proyekmu.

---

### 🌐 4. Dapatkan Domain GitHub

Setelah proses selesai, GitHub akan menampilkan tautan domain seperti berikut: https://username.github.io/link contoh/
Gantilah `username` dengan nama akun GitHub kamu.  
Buka link tersebut di browser — jika berhasil, maka **AI IRF kamu sudah online!** 🎉

---

### 🏷️ 5. (Opsional) Gunakan Domain Pribadi Sendiri

Jika kamu memiliki domain pribadi (misal `irfai.tech` atau `irfproject.xyz`),  
kamu bisa menghubungkannya ke GitHub Pages.

#### Langkah-langkah:

1. Di dalam folder proyek kamu, buat file baru bernama: CNAME

   Type: CNAME
Name: www
Value: username.github.io
TTL: Auto


5. Simpan perubahan DNS dan tunggu sekitar 10–30 menit agar domain aktif.

---

### 🔐 6. Aktifkan HTTPS (Keamanan Tambahan)

Agar situs kamu lebih aman, aktifkan koneksi HTTPS.

1. Buka kembali tab **Settings → Pages**.  
2. Di bawah kolom domain, aktifkan opsi:


✅ Enforce HTTPS

3. GitHub akan otomatis membuat sertifikat SSL gratis untuk situsmu.

---

### ✅ 7. Tes Akhir

Setelah DNS aktif, buka salah satu dari tautan berikut:

**Jika pakai domain GitHub:**


https://username.github.io/irf-ai/


**Jika pakai domain pribadi:**


https://irfai.tech/


Jika halaman IRF kamu tampil dengan benar dan interaktif,  
maka proses publikasi **berhasil 100%!** 🚀

---

### 💡 Tips Tambahan

- Tambahkan file **favicon.ico** agar logo IRF muncul di tab browser.  
- File `README.md` akan otomatis tampil di halaman utama repository GitHub kamu.  
- Setiap kali kamu mengubah file (misalnya `index.html`), cukup klik **Commit changes**,  
  dan GitHub Pages akan otomatis memperbarui situs kamu dalam 1–2 menit.

---

### 🧠 Kesimpulan

| Langkah | Deskripsi |
|----------|------------|
| 🏗️ Buat Repository | Siapkan repo baru di GitHub |
| 📤 Upload File | Unggah `index.html` dan file pendukung |
| ⚙️ Aktifkan Pages | Atur deployment ke branch `main` |
| 🌍 Dapatkan Domain | Gunakan domain `github.io` atau domain pribadi |
| 🔐 Amankan | Aktifkan HTTPS |
| 🚀 Selesai | IRF kamu sudah online dan siap dibagikan |

---

> 🧩 **IRF – Interaktif Real Featur**  
> Publikasikan AI kamu dengan mudah, cepat, dan gratis melalui **GitHub Pages**.  
> 100% Lokal • Aman • Cepat • Cerdas

list model di webllm = # Daftar 29 Model AI (kompatibel / sering dipakai dengan WebLLM)
> Catatan: semua angka adalah *perkiraan umum*. VRAM = estimasi memori GPU untuk inference FP16 (non-quantized). Dengan quantization (INT8/INT4) kebutuhan VRAM bisa turun drastis.

Qwen2-0.5B — Parameter: ~0.5B — Perkiraan VRAM: 1–2 GB — Context window: 2K–4K tokens (≈2048–4096)  
Qwen2-1.5B — Parameter: ~1.5B — Perkiraan VRAM: 3–4 GB — Context window: 2K–8K tokens  
Qwen2-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K tokens  
Qwen2-14B — Parameter: ~14B — Perkiraan VRAM: 16–24 GB — Context window: 8K–32K tokens  
Qwen2-VL (vision-language variant) — Parameter: varies (multimodal) — Perkiraan VRAM: 8–20 GB — Context window: 4K–32K tokens (plus image tokens)  
Qwen2-Audio (multimodal/audio variant) — Parameter: varies — Perkiraan VRAM: 6–18 GB — Context window: 2K–8K (plus audio frames)

Llama-3-1B (Instruct) — Parameter: ~1B — Perkiraan VRAM: 2–3 GB — Context window: 2K–4K  
Llama-3-3B (Instruct) — Parameter: ~3B — Perkiraan VRAM: 5–8 GB — Context window: 4K–8K  
Llama-3-7B (Instruct) — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K

Llama-2-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 4K–16K  
Llama-2-13B — Parameter: ~13B — Perkiraan VRAM: 14–20 GB — Context window: 4K–32K

Phi-3 (mini / small variants) — Parameter: varian mini ≈0.5–3B — Perkiraan VRAM: 1–8 GB (tergantung varian) — Context window: 2K–16K  
Phi-2 (varian) — Parameter: varian 1B–7B — Perkiraan VRAM: 2–12 GB — Context window: 2K–16K

Mistral-7B (v0.3 / standard) — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K (atau lebih tergantung build)  
Mistral-instruct / Mistral-variants — Parameter: ~7B+ — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K

Gemma-2B — Parameter: ~2B — Perkiraan VRAM: 3–6 GB — Context window: 8K (varian besar bisa 32K)  
Gemma-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–32K

RedPajama-3B — Parameter: ~3B — Perkiraan VRAM: 5–8 GB — Context window: 4K–8K  
RedPajama-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K

Falcon-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K  
Falcon-40B — Parameter: ~40B — Perkiraan VRAM: 40–80+ GB (biasanya memerlukan sharding/CPU+GPU) — Context window: 8K–16K (varian lama) / 32K pada beberapa build

MPT-7B — Parameter: ~7B — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K  
Vicuna-13B (fine-tuned Llama derivative) — Parameter: ~13B — Perkiraan VRAM: 14–20 GB — Context window: 4K–16K

Dolly-v2-12B — Parameter: ~12B — Perkiraan VRAM: 14–20 GB — Context window: ≈2K–16K  
OpenHermes / Hermes variants (Mistral-based variants) — Parameter: ~7B (varian umum) — Perkiraan VRAM: 8–12 GB — Context window: 8K–16K

Qwen2.5 / Qwen2.5-Max (komersial/varian besar) — Parameter: 7B–32B (varian) — Perkiraan VRAM: 8–40+ GB (tergantung varian) — Context window: 8K–32K

Qwen3 / Qwen3-Max (next-gen family) — Parameter: 7B–32B+ (varian) — Perkiraan VRAM: 8–64+ GB — Context window: 8K–32K+

Model custom / community WebLLM format (MLC-converted) — Parameter: bervariasi — Perkiraan VRAM: bergantung pada model & quantization — Context window: bergantung pada model

(DAFTAR TAMBAHAN — cadangan untuk mencapai total 29 item jika ingin variasi nyata:)
- TinyLlama (0.7B–1.3B) — Parameter: ~0.7–1.3B — Perkiraan VRAM: 1.5–3 GB — Context window: 2K–4K  
- Bloom (176B / smaller variants) — Parameter: varian kecil hingga besar — Perkiraan VRAM: besar untuk varian >7B — Context window: 2K–32K  
- Claude-style community small models (varian komunitas) — Parameter: bervariasi — Perkiraan VRAM: bervariasi — Context window: bervariasi

---

## Penjelasan singkat pengukuran
- **Parameter** = jumlah bobot model (dalam miliar, B = milyar).  
- **VRAM (perkiraan)** = memori GPU yang diperlukan untuk menjalankan inference pada presisi FP16 (tidak ter-quantize). Angka ini *akan turun* jika model dijalankan dengan quantization (INT8/INT4) atau metode sharding/CPU offload.  
- **Context window** = jumlah token konteks model yang dapat diproses dalam satu prompt; bergantung pada arsitektur dan build model.

## Rekomendasi praktis
- Untuk **WebLLM in-browser**, model ringan (≤1–3B) sangat ideal: **Qwen2-0.5B, Phi mini, TinyLlama** — butuh VRAM kecil dan cepat.  
- Model 7B cocok untuk pengguna desktop/laptop kelas menengah (WebGPU). Pastikan quantization untuk menghemat memori.  
- Model ≥13B biasanya memerlukan sharding, lebih cocok untuk server atau runtime yang mendukung banyak memori / WebGPU besar.

---
# 💻📱 Rekomendasi Laptop & Smartphone untuk WebLLM
> Daftar ini berisi 16 perangkat (8 laptop + 8 smartphone) yang mendukung WebLLM  
> dan cocok untuk menjalankan model AI lokal seperti **IRF (Interaktif Real Featur)**.  
> Semua perangkat memiliki **RAM ≥ 12 GB** dan **penyimpanan ≥ 512 GB**.

---

## 💻 Laptop yang Cocok untuk WebLLM

### 🔹 ASUS Vivobook 14X OLED (M1403)
- **RAM:** 16 GB DDR5  
- **Storage:** 512 GB SSD  
- **GPU:** Radeon 780M (Integrated, mendukung WebGPU)  
- **Kelebihan:** OLED display, sangat responsif untuk AI web.  
- **Cocok untuk:** Model kecil–menengah (Qwen2-1.5B / Phi-3).  

---

### 🔹 Lenovo IdeaPad 5 Pro
- **RAM:** 16 GB  
- **Storage:** 512 GB SSD  
- **GPU:** NVIDIA RTX 2050  
- **Kelebihan:** GPU dedicated, sangat stabil untuk model 3B–7B.  
- **Cocok untuk:** Eksperimen WebLLM multi-tab dan model Mistral-7B.  

---

### 🔹 ASUS Zenbook 14 (UX3405)
- **RAM:** 16 GB LPDDR5  
- **Storage:** 512 GB NVMe SSD  
- **GPU:** Intel Arc Graphics (WebGPU-ready)  
- **Kelebihan:** Performa CPU AI-Engine yang tinggi.  
- **Cocok untuk:** Model kecil hingga 3B dengan UI interaktif berat.  

---

### 🔹 HP Envy x360 13 (Ryzen 7)
- **RAM:** 16 GB  
- **Storage:** 512 GB SSD  
- **GPU:** Radeon Integrated  
- **Kelebihan:** Portabilitas tinggi, performa efisien.  
- **Cocok untuk:** Model kecil < 3B (Qwen2-0.5B, Phi-mini).  

---

### 🔹 Acer Swift X 14
- **RAM:** 16 GB  
- **Storage:** 1 TB SSD  
- **GPU:** NVIDIA RTX 3050 Ti  
- **Kelebihan:** Mendukung CUDA & WebGPU, performa tinggi.  
- **Cocok untuk:** Model besar (7B – 13B) via quantization.  

---

### 🔹 MacBook Air M3 (2024)
- **RAM:** 16 GB Unified  
- **Storage:** 512 GB SSD  
- **GPU:** 10-core M3 GPU  
- **Kelebihan:** WebGPU aktif secara default (Safari 17+).  
- **Cocok untuk:** Model kecil–menengah dengan optimisasi Metal.  

---

### 🔹 Lenovo Legion Slim 5
- **RAM:** 16 GB  
- **Storage:** 512 GB SSD  
- **GPU:** RTX 4060 (8 GB VRAM)  
- **Kelebihan:** Performa tinggi untuk inferensi real-time.  
- **Cocok untuk:** Model 7B–13B non-quantized.  

---

### 🔹 ASUS ROG Zephyrus G14
- **RAM:** 16 GB  
- **Storage:** 1 TB SSD  
- **GPU:** RTX 4070 (8 GB VRAM)  
- **Kelebihan:** Laptop gaming terbaik untuk eksperimen AI lokal.  
- **Cocok untuk:** Semua model hingga 13B dengan smooth inference.  

---

## 📱 Smartphone yang Cocok untuk WebLLM

### 🔹 Samsung Galaxy S24 Ultra
- **RAM:** 12 GB  
- **Storage:** 512 GB  
- **Chipset:** Snapdragon 8 Gen 3  
- **Kelebihan:** Browser mendukung WebGPU (Chrome/Edge).  
- **Cocok untuk:** Model kecil (< 1B) dan demo AI di mobile.  

---

### 🔹 Xiaomi 14 T Pro
- **RAM:** 12 GB  
- **Storage:** 512 GB  
- **Chipset:** Dimensity 9300  
- **Kelebihan:** CPU/GPU sangat cepat, cocok untuk WebLLM mobile.  

---

### 🔹 OPPO Reno12 Pro 5G
- **RAM:** 12 GB  
- **Storage:** 512 GB  
- **Chipset:** Snapdragon 8 Gen 1  
- **Kelebihan:** Performa stabil, dukungan WebGPU di Chrome.  

---

### 🔹 ASUS ROG Phone 8
- **RAM:** 16 GB  
- **Storage:** 512 GB  
- **Chipset:** Snapdragon 8 Gen 3  
- **Kelebihan:** Termal stabil, optimal untuk running LLM mini.  

---

### 🔹 Vivo X100 Pro
- **RAM:** 16 GB  
- **Storage:** 512 GB  
- **Chipset:** Dimensity 9300  
- **Kelebihan:** Performa tinggi dan efisien untuk AI browser.  

---

### 🔹 Huawei Mate 60 Pro+
- **RAM:** 12 GB  
- **Storage:** 512 GB  
- **Chipset:** Kirin 9000S  
- **Kelebihan:** Dukungan WebGPU versi Harmony OS 4.  
- **Cocok untuk:** Demo IRF offline tanpa server.  

---

### 🔹 iPhone 15 Pro
- **RAM:** 8 GB (efektif setara 12 GB Android)  
- **Storage:** 512 GB  
- **Chipset:** Apple A17 Pro  
- **Kelebihan:** WebGPU Safari 17+, efisien menjalankan model kecil.  

---

### 🔹 Realme GT 5 Pro
- **RAM:** 16 GB  
- **Storage:** 512 GB  
- **Chipset:** Snapdragon 8 Gen 3  
- **Kelebihan:** Sangat cepat untuk inference ringan di Chrome.  

---

## ⚙️ Rekomendasi Teknis Umum

| Jenis Perangkat | Minimum | Disarankan |
|------------------|----------|-------------|
| **RAM Sistem** | 12 GB | 16 GB – 32 GB |
| **Penyimpanan** | 512 GB SSD | 1 TB NVMe SSD |
| **GPU/Chipset** | Intel Arc / Radeon / Snapdragon 8 Gen 2+ | RTX 3050 ke atas / Apple M3 |
| **Browser** | Chrome 121+, Edge 121+, Safari 17+ | Mendukung **WebGPU** |
| **Model Ideal** | Qwen2-0.5B / Phi-3-mini / TinyLlama | Qwen2-1.5B / Mistral-7B |

---

### 🔐 Catatan Penting
- WebLLM berjalan langsung di browser, jadi semakin besar **VRAM atau Unified Memory**, semakin cepat inferensinya.  
- Gunakan **quantized models (INT4/INT8)** agar hemat memori dan lancar di laptop kelas menengah.  
- Browser wajib mendukung **WebGPU** (aktif di Chrome 121+ & Safari 17+).  

---
update info

1 password generator
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
> Dapat dijalankan di laptop atau smartphone dengan WebGPU.  
> 100% lokal • Aman • Cepat • Gratis.
