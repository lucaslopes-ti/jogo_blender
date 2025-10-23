ℹ Note: I'm slowly making a new and improved version of the Lightmapper. It's currently located in the "Lightmapper-One" branch, but keep in mind, it's very early and WIP - Naxela.
<br>

## The Lightmapper

![](img/a.png)

### Description

The Lightmapper is an addon for Blender that implements lightmapping and denoising capabilities for global illumination texture baking with support for 32-bit HDR Lightmaps. 
Baking is done through Cycles, and includes automatic material setup, automatic UV setup, encoding options, format options and advanced postprocess filtering. The setup is object-centric, meaning that you can customize the settings for each individual object, providing you with the easiest and most versatile lightmapping solution for Blender.

![](img/i.jpg)

### Features - Version 0.3
- Automated lightmap baking

The addon automates everything you need to bake, ranging from scaling, material setup, uv-layering, uv-unwrapping and more:

![](img/d.jpg)

- Per-object settings

Each object can have it's own settings and be customized in terms of resolution, uv margin and unwrap mode:

![](img/j.jpg)

- Multi-material support

Add as many materials to each object as you want:

![](img/b.png)

- AI-based Denoising

Integrated denoising as well as support for faster CPU OIDN denoising and GPU Optix denoising:

![](img/c.jpg)

- Performance and speed

Baking presets automatically adjusts sampling, quality and tile settings based on situation and CPU/GPU:

![](img/e.jpg)

- Postprocess filtering

Additional filtering to give your lightmaps an extra edge and quality through OpenCV:

![](img/f.png)

- Background-baking

Is your baking going to take a long time? Try background baking, which let's you continue working on your scene:

![](img/g.png)

- Easy material management

Apart from automatic material setup, resetting materials is easy and baking without material setup too for external engines:

![](img/h.jpg)

### Installation

Installation of The Lightmapper is straight forward. All you need to do is download the latest release, and install as a .zip file from inside Blender. For more information, please refer to the wiki section: COMING SOON

### Usage

To lightmap, the scene needs to be saved to disk.

To enable lightmapping for single objects, go to object properties/The Lightmapper and enable it.

![](https://user-images.githubusercontent.com/5429817/228257743-33487019-a2d3-40c3-a318-270f98ccd219.png)

If you want to bake the whole scene, you can enable lightmapping for all objects by going to Utilities and click "Enable for set" - By default it will apply this to all the objects in the scene.

![](https://user-images.githubusercontent.com/5429817/228258206-3a75f64e-d483-4c9f-9cc7-fc7ccec9d4a4.png)



For more information, please refer to the wiki section: COMING SOON

### Documentation

The wiki page is under construction, and documentation is in the process of being written.

### Images and Videos

[![Watch the video](img/prev.jpg)](https://www.youtube.com/watch?v=RaWNQrSaymo)

[![Watch the video](img/k.gif)](https://vimeo.com/447551701)

*HTML5 lightmap examples - Powered by Armory3D*

http://laboratory.naxela.info/experiment_1/

http://laboratory.naxela.info/experiment_2/

http://laboratory.naxela.info/experiment_3/

http://laboratory.naxela.info/experiment_4/

http://laboratory.naxela.info/experiment_5/

http://laboratory.naxela.info/experiment_7/

http://laboratory.naxela.info/experiment_8/

http://laboratory.naxela.info/experiment_11/

http://laboratory.naxela.info/experiment_12/

http://laboratory.naxela.info/experiment_13/

----

*3rd Party addon compatibility*

- OpenCV:
https://pypi.org/project/opencv-python/

- Blender Xatlas by Mattedicksoncom:
https://github.com/mattedicksoncom/blender-xatlas
