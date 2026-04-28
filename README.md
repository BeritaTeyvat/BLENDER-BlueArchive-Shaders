

https://github.com/user-attachments/assets/55c34cf5-9a57-44ff-adb9-f4eeaeced929

# 🎨 Blender Blue Archive Shaders

A custom **toon / cel shader** for Blender, inspired by the visual style of **Blue Archive**.
This project aims to replicate the clean, anime-style cel shading used in the game so it can be applied to 3D models inside Blender.

> ⚠️ **Status: Early Release / Work In Progress**
> Features, node setups, and file structure may change frequently. Feedback and contributions are welcome!

---

## 📽️ Preview

[<video src="https://github.com/BeritaTeyvat/BLENDER-BlueArchive-Shaders/raw/main/Preview/0001-0250.mp4" controls></video>](https://github.com/user-attachments/assets/3cf35198-ef29-412c-9d54-e3d3943bd6c4)

---

## ✨ Features

- Blue Archive–inspired toon / cel shading
- Custom light & shadow ramps
- Adjustable rim light and outline
- Compatible with Blender's **Eevee** renderer (Goo Engine recommended)
- Simple node group setup — easy to plug into any character model

---

## 📦 Requirements

- **Blender 4.0+** (tested on the latest stable release)
- A character model with **proper UVs** and **face/body textures**
- Datamined texture from the game

---

## 🚀 Getting Started

### Step 1 — Download the project

Clone or download this repository:

```bash
git clone https://github.com/BeritaTeyvat/BLENDER-BlueArchive-Shaders.git
```

Or click **Code → Download ZIP** on GitHub.

### Step 2 — Open the `.blend` file

Open the provided `.blend` file in Blender.
Inside, you'll find:

- A pre-configured **shader node group** (e.g. `BA_ToonShader`)
- A demo character / sample mesh (if included)
- Example light setup

### Step 3 — Append the shader into your own project

If you want to use the shader on your own model:

1. Open your own Blender file.
2. Go to **File → Append**.
3. Navigate into the downloaded `.blend` file.
4. Open the **`NodeTree`** folder.
5. Select the shader node group (e.g. `BA_ToonShader`) and click **Append**.

### Step 4 — Apply the shader to your model

1. Select your character mesh.
2. Open the **Shading** workspace.
3. Create a new material (or use an existing one).
4. Add a **Group** node → choose `BA_ToonShader`.
5. Connect the group's output to **Material Output → Surface**.
6. Plug your character's **base color texture, and mask texture** into the shader's input.

### Step 5 — Set up lighting
1. Select your mesh and add Light Vector geometry nodes for lighting

### Step 6 — Tweak the look

Inside the shader group you can adjust:

- **Shadow color / threshold** — controls where shadows fall
- **Rim light intensity** — edge highlight strength
- **Specular / highlight** — anime-style glossy spots
- **Outline thickness** (if outline modifier is included)

Play around with these until the result matches the Blue Archive vibe you want.

---

## 📁 Repository Structure

```
BLENDER-BlueArchive-Shaders/
├── Preview/              # Demo videos & screenshots
│   └── 0001-0250.mp4
├── Shaders/              # .blend files containing the shader
├── Examples/             # Example scenes / test models
└── README.md
```

> Structure may be updated as the project evolves.

---

## 🛠️ Roadmap

- [ ] Final shader node group cleanup
- [ ] Screen-space Outline
- [ ] Face SDF shadow support
- [ ] Dynamic Hair anisotropic highlight
- [ ] Documentation page with screenshots

---

## 🤝 Contributing

This is an early release — issues, suggestions and pull requests are very welcome.
If you find a bug or want to request a feature, please open an **Issue** on GitHub.
I made this based on material data and compressed shader file, if you have a renderdoc or a proper code
for unfinished feature, please give me a suggestions or make a pull requests for contributing on this project.

---

## 📜 License & Disclaimer

This is a **fan project** and is **not affiliated with Nexon, Yostar, or NAT Games**.
"Blue Archive" and all related assets are the property of their respective owners.
This shader is provided for **educational and non-commercial purposes** only.

---

## 💙 Credits

- Shader development: **[BeritaTeyvat](https://github.com/BeritaTeyvat)**
- Inspiration: **Blue Archive** by Nexon Games / Yostar
- AerthasVeras for dot product node setup and flipbook function
- Festivity's shader for cleanest shader graph workflow
- LooperHonstropy with their UmaMusume Blender shader

---

> If you use this shader in your renders, feel free to tag me — I'd love to see what you make!
