# ControllableSD

**ControllableSD** is a customizable workflow built on top of [ComfyUI](https://github.com/comfyanonymous/ComfyUI), allowing controllable image transformations such as weather manipulation using depth, segmentation, edges and custom masks.

## 🚀 Features

- Weather manipulation with controllable intensity
- Fine-tuning transformations via denoising strength
- Leverages state-of-the-art tools like Segment Anything and Ultimate SD Upscale
- Compatible with ComfyUI `v0.2.2`

---

## 📦 Installation

### 1. Install ComfyUI

Follow the installation instructions in the official [ComfyUI GitHub repository](https://github.com/comfyanonymous/ComfyUI).

> 💡 Note: This workflow was tested with `ComfyUI v0.2.2`. Compatibility with later versions is not guaranteed.

---

### 2. Install Required Custom Nodes

Clone or download the following custom nodes into your ComfyUI `custom_nodes/` directory:

- [ComfyUI Segment Anything](https://github.com/storyicon/comfyui_segment_anything)
- [ComfyUI_UltimateSDUpscale](https://github.com/ssitu/ComfyUI_UltimateSDUpscale)
- [ComfyUI-Marigold](https://github.com/kijai/ComfyUI-Marigold)
- [masquerade-nodes-comfyui](https://github.com/BadCafeCode/masquerade-nodes-comfyui)
- **DepthMapModifier** (located in this project repository)

---

## ▶️ Getting Started

### 3. Start the Server

1. Run the ComfyUI server:
   ```bash
   python main.py
   ```
2.	Load the provided workflow.json into the UI.
3.	Upload your input image.
4.	Enter your prompt and queue the job.

---

🎛️ Controlling Weather Intensity

You can adjust the weather intensity of the output by changing the Denoising Strength parameter in the UI:
	•	Low Denoising Strength → Subtle changes
	•	High Denoising Strength → Strong transformations

---

🖼️ Example Use Cases
	•	Turning a clear day into a snowy scene
	•	Visualizing how weather affects architecture or street scenes
	•	Synthetic data generation for training ML models

---

📂 License

This project is released under the MIT License.
