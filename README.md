# Toggle Accelerator

A non-destructive Unity editor workflow for VRChat avatars that makes creating toggles, radial puppet sliders, clothing selectors, material swaps, shader animations, blendshapes, and props effortless.

Whether you prefer working completely **Standalone**, integrating with **Modular Avatar** or **VRCFury**, or baking raw assets in **Instant** mode, Toggle Accelerator lets you configure complex avatar interactions from a single inspector without manual animator wiring.

---

## What It Does

Toggle Accelerator eliminates manual animator layer editing, transition wiring, and expression parameter tracking. Define your controls and target objects in the inspector, and Toggle Accelerator generates all required Animator layers, transitions, parameters, and menus non-destructively at upload or play mode time.

### Key Features

- **Multi-Mode Control Groups:** Create standard on/off toggles, hold buttons, and continuous or stepped radial puppet wheels from one unified interface.
- **5 Versatile Target Modes:**
  - **Toggle (TG):** Toggle GameObjects, animate local transforms with scene gizmos, or toggle individual components (PhysBones, colliders, contacts, constraints, audio, lights).
  - **BlendShape (BS):** Drive blendshape weights, or set to `DEL` to permanently strip body mesh under clothing at build time.
  - **Material Swap (MS):** Swap material slots with renderer scopes (`THIS`, `SHAR`, `ALL`).
  - **Material Property (MP):** Animate float sliders, colors, or vectors directly without duplicating materials.
  - **World Freeze (WF):** Lock props, bone chains, or meshes in world space using VRChat parent constraints.
- **Smart Gating Logic:** Coordinate complex clothing combinations with `-Param` (gate closed/suppress) and `+Param` (gate open/force) modifiers to prevent clothing clipping without animator conflicts.
- **In-Tool Recording:** Record animation keyframes directly using automated clean avatar copies, or pose props visually in the 3D Scene view with real-time coordinate capture.
- **Parameter Optimizer:** Dynamic bit-width clamping, explicit `Value+Bits` allocation, and multiplexed parameter compression across rotating carrier channels to stay within VRChat's 256-bit limit.
- **Layer Optimizer:** Migrates non-animating logic layers from the FX controller to the Action controller at weight 0.0, reducing Mecanim evaluation overhead.
- **Submenus & Visual Customization:** Organize menus with forward slashes `/`, assign custom folder icons per level, and colorize menu labels with rich-text tags.
- **One-Click Test Clones:** Generate Quick Build or Full Build test copies directly in the scene to inspect and verify menus in Gesture Manager.

---

## Documentation

Full documentation, step-by-step guides, and tutorials are available at:  
[Toggle Accelerator Documentation](https://kitsuneba.github.io/docs/toggle-accelerator/)

---

## Installation via VCC or ALCOM

Add the repository listing directly to your package manager:  
https://kitsuneba.github.io/KitsuneBaTools/

Or add it manually:
1. Open **VRChat Creator Companion (VCC)** or **ALCOM**.
2. Go to **Settings -> Packages -> Add Repository**.
3. Paste the listing URL:
   ```text
   https://kitsuneba.github.io/KitsuneBaTools/index.json
   ```
4. Click **Add**.

---

## License

See [LICENSE.md](LICENSE.md) for terms of use.
