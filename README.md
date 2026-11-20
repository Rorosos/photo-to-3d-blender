# Photo to 3D for Blender

Generate textured 3D assets from reference photos with TRELLIS.2 and Hunyuan3D, then import or export them from Blender.

*This project is pure vibe coding.*

[Project website](https://rorosos.github.io/photo-to-3d-blender/) · [Download for Windows](./photo-to-3d-windows.zip) · [Component terms](./THIRD_PARTY_NOTICES.md)

![Rendered TRELLIS.2 reconstruction of a burger on a plate](./burger-render.png)

## What it does

- Generate from one JPG or PNG, or use front, left, and back references with Hunyuan3D.
- Add JPG or PNG files by dragging them from File Explorer onto **Choose photo** or a photo preview in the Blender sidebar.
- Queue jobs and seed variants, see progress, and import finished models into a scene.
- Export FBX, preview images, and available textures to each job folder.
- Install the engine environments and model weights you need from Blender's sidebar.

![Generated chair in Blender with Hunyuan3D and TRELLIS.2 previews in the job queue](./blender-chair-queue.png)

## Install

1. Use Blender 5.3 or later on Windows x64 with a compatible NVIDIA CUDA GPU and driver.
2. In Blender, choose **Edit → Preferences → Add-ons → Install from Disk** and select `photo-to-3d-windows.zip`.
3. In the 3D Viewport, press **N** and open **Photo to 3D**. Set your language and engine.
4. Click **Download components**. Use **Components** to install individual weights or add an engine later.
5. In **Generate → Single photo**, use **Choose photo** or drop images onto the button or a photo preview. Click **Add to queue**. When generation finishes, use **Import into scene** or open the job folder from the queue.

Enable online access in **Preferences → System → Network** for downloads. The compact ZIP includes the TRELLIS.2 example and Python source. To download gated DINOv3 or RMBG-2.0 weights, request access on their Hugging Face pages and supply a read token from the Components tab. The token is used within the current Blender session. RMBG-2.0 is optional if background removal is disabled.

Interface languages include English, Russian, Simplified Chinese, Hindi, Spanish, Arabic, French, Bengali, Portuguese, Indonesian, Urdu, and German.

## Maintainer

[Rorosos](https://github.com/Rorosos). See [third-party notices](./THIRD_PARTY_NOTICES.md) for model terms and demo attribution.
