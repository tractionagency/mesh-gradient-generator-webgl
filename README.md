# Gradient Mesh Generator 🌊

A high-performance, WebGL-based tool for generating fluid, animated gradient backgrounds. Unlike standard CSS gradients, this tool uses GLSL shaders (via the OGL library) to create complex, organic visual effects like "Water," "Plasma," and "Aurora."

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://tractionagency.github.io/mesh-gradient-generator-webgl/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## ✨ Features

This tool currently supports the following configurations:

*   **3 Visual Styles:** Switch between **Water**, **Plasma**, and **Aurora** math models to change the movement and blending behavior of the mesh.
*   **3-Color Palette:** Pick exact colors for the background, mid-tones, and highlights using hex codes or the native color picker.
*   **Film Grain Control:** A slider to adjust the intensity of a noise overlay, adding texture to the gradient.
*   **Code Export:**
    *   **Copy HTML:** Generates a self-contained `.html` file (including the OGL library via CDN) ready to run.
    *   **Copy React:** Generates a snippet for React integration.

## 🚀 How to Use

1.  **Select a Style:** Click the buttons in the "Style" section to change the animation algorithm (Water flows horizontally, Plasma pulses, Aurora creates vertical banding).
2.  **Adjust Colors:** Modify the 3 color inputs. The gradient updates in real-time.
3.  **Add Texture:** Use the "Grain" slider to increase or decrease the noise effect.
4.  **Export:** Click "Copy HTML" to get the full file code or "Copy React" for a component snippet.

## 💡 Why is this useful to developers?

*   **Performance:** This uses WebGL (GPU acceleration), meaning complex animations won't lag your main thread like heavy JavaScript or CSS animations might.
*   **Aesthetics:** Creates organic, "mesh-like" visuals that are impossible to achieve with standard linear or radial CSS gradients.
*   **Portability:** The export feature wraps the shader code and dependencies into a single snippet, making it easy to drop a professional-looking background into any project without setting up a WebGL build pipeline.

## 🛠️ Tech Stack

*   **HTML5 & CSS3:** For the glassmorphism UI overlay.
*   **JavaScript (ES Modules):** Logic and state management.
*   **WebGL (OGL):** The tool uses [ogl@1.0.11](https://github.com/oframe/ogl) (loaded via esm.sh) to handle the WebGL context and rendering.

## 📍 Roadmap / Next Update

We are actively improving this tool. The next update will include:

*   **📥 Direct Download:** We will add a button to download the code as an `.html` file directly to your computer, removing the need to copy-paste from the clipboard.

## 📝 License

This project is open source and available under the [MIT License](LICENSE).