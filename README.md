# 🏺 Singing Bowl of Jingdezhen · 景德镇唱歌碗

**Turn your fingertip into a brush that makes porcelain sing.**  
**把你的指尖变成让瓷器歌唱的画笔。**

This interactive web experience uses your webcam to track your hand in real time. As you trace the rim of a virtual porcelain bowl with your finger, it produces a continuous, resonant tone — just like a master craftsman making a real porcelain bowl “sing” by rubbing its rim with a wet finger.

本项目是一个实时交互的网页应用，它通过摄像头追踪您的手部动作。当您用手指沿着虚拟瓷碗的边缘摩擦时，它会发出持续、共鸣的音调——就像工匠用湿手指摩擦薄胎瓷碗边缘，使其发出清脆的“歌声”一样。

---

## ✨ What It Does · 功能特色

- **Hand‑tracked musical instrument** – Your index finger becomes the player; no keyboard, no mouse, just movement.  
  **手部追踪乐器** – 您的食指就是演奏者；无需键盘鼠标，只需移动手部。

- **Porcelain bowl simulation** – The bowl is drawn as an elegant porcelain form with decorative blue patterns inspired by Jingdezhen’s centuries‑old craftsmanship.  
  **瓷碗模拟** – 碗身呈现典雅的瓷器形态，并带有源自景德镇数百年工艺的蓝色装饰纹样。

- **Pitch and timbre control** – Moving your finger around the rim changes the pitch; moving it up/down adjusts brightness (filter); faster movements add harmonics and accents.  
  **音高与音色控制** – 手指沿碗边移动改变音高，上下移动调节明亮度（滤波器），快速动作增加泛音和重音。

- **Real‑time audio synthesis** – Powered by Tone.js, using FM synthesis with delay and reverb to create a warm, resonant “singing” quality.  
  **实时音频合成** – 基于 Tone.js 的 FM 合成，配合延迟和混响，营造温暖、共鸣的“歌唱”质感。

- **Visual feedback** – See your mirrored hand skeleton, glowing rim, motion particles, and a live (mirrored) webcam preview.  
  **视觉反馈** – 显示镜像手部骨架、发光碗边、运动粒子，以及实时（镜像）摄像头预览。

---

## 🎯 How to Use · 使用方法

1. **Open** the page in a modern browser (Chrome, Edge, Firefox).  
   **打开** 页面（推荐 Chrome、Edge、Firefox 等现代浏览器）。

2. **Allow camera access** when prompted.  
   **允许** 摄像头访问权限。

3. **Click anywhere** to unlock the audio (required by browser security).  
   **点击任意位置** 以启用音频（浏览器安全策略要求）。

4. **Show your hand** to the camera – make sure your index finger is visible.  
   **将手展示** 在摄像头前 – 确保食指清晰可见。

5. **Move your finger along the bowl’s rim** – the sound changes instantly. Try different speeds and positions to explore the full range.  
   **沿着碗边移动手指** – 声音会即时变化。尝试不同速度和位置，探索全部音域。

6. **Enjoy the ritual** – no touch, no keyboard, just you and the porcelain.  
   **享受这场仪式** – 无需触摸，无需键盘，只有您和瓷器。

---

## 🧱 Technical Stack · 技术栈

- **Hand Tracking** – MediaPipe Tasks Vision (HandLandmarker) – 21 landmarks, GPU accelerated.  
  **手部追踪** – MediaPipe Tasks Vision (HandLandmarker) – 21 个关键点，GPU 加速。

- **Visuals** – Canvas 2D – orange mirrored skeleton, green interference waves, ghost trails, motion particles.  
  **可视化** – Canvas 2D – 橙色镜像骨架、绿色干涉波、残影轨迹、运动粒子。

- **Audio** – Tone.js – FM synthesis with filter, delay, reverb; pitch mapped to hand position.  
  **音频** – Tone.js – FM 合成器配合滤波器、延迟、混响；音高映射到手部位置。

- **Mirroring** – All landmarks are mirrored horizontally for a natural mirror reflection.  
  **镜像** – 所有关键点水平镜像，呈现自然的镜面反射。

---

## 🏺 About Jingdezhen Porcelain · 关于景德镇瓷器

Jingdezhen, known as the “Porcelain Capital” for over a thousand years, is famous for its high‑temperature porcelain. One of its most enchanting traditions is the “singing bowl” – a thin, vitrified bowl that produces a clear, bell‑like tone when its rim is rubbed with a moistened finger. This digital experience pays homage to that ancient craft, blending traditional aesthetics with modern interactive technology.

景德镇，被誉为“千年瓷都”，以其高温瓷器闻名于世。其中最令人着迷的传统之一便是“唱歌碗”——一种薄胎瓷碗，用湿手指摩擦碗边时能发出清脆如铃的声音。本数字体验向这一古老技艺致敬，将传统美学与现代交互技术相融合。

---

## 📁 File Structure · 文件结构

- `index.html` – Single‑file application (HTML/CSS/JavaScript).  
  `index.html` – 单文件应用（包含 HTML/CSS/JavaScript）。

- `hand_landmarker.task` (optional) – The MediaPipe model file (~10–15 MB). You can download it from Google’s storage and host it locally for faster loading (update the `modelAssetPath` accordingly).  
  `hand_landmarker.task`（可选）– MediaPipe 模型文件（约 10–15 MB）。可下载并自托管以加快加载速度（相应更新 `modelAssetPath`）。

---

## ⚡ Performance Notes · 性能说明

- The MediaPipe model is loaded from Google’s CDN. In regions with restricted access, you may experience slow loading. Self‑hosting the `.task` file is recommended.  
  MediaPipe 模型从 Google CDN 加载。在访问受限的地区可能加载缓慢，建议自托管 `.task` 文件。

- Audio requires a user click (browser autoplay policy). The synth engine starts only after the first click.  
  音频需用户点击启动（浏览器自动播放策略），合成引擎仅在首次点击后启动。

---

## 🙏 Credits · 致谢

- **MediaPipe** by Google
- **Tone.js** by Yotam Mann
- Concept and code by Signal Ritual v2 (adapted for Jingdezhen singing bowl)
- Inspired by the artisans of Jingdezhen and their timeless porcelain craft.

---

## 📄 License · 许可证

MIT – free to use, modify, and share.  
MIT 许可证 – 可自由使用、修改和分享。

---

**Enjoy the ritual. ✨**  
**享受这场仪式。✨**
