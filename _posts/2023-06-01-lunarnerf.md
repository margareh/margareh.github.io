---
layout: post
title: Lunar NeRFs
published: true
permalink: /lunar-nerf/

image_link: /assets/nerf_view_env3.png
alt_text: Rendered image of synthetic lunar terrain
description: Neural radiance fields (<a href="https://www.matthewtancik.com/nerf">NeRFs</a>) are learned, neural representations of a density and color field that can be used to render novel views of a scene via volumetric rendering. Planetary robotics poses a challenge for such techniques due to the often extreme lighting conditions, lack of features in a scene, and limited motion of the image sensors, in addition to the problem of compute. This project seeks to assess the practicability of using NeRFs for modeling lunar terrain, with a focus on geometric aspects in addition to photometric.
---

<img style="float: right; margin-left: 30px;" src="/assets/nerf_view_env3.png"  width="30%" alt="Render of lunar terrain from a NeRF model." />

Neural radiance fields ([NeRFs](https://www.matthewtancik.com/nerf)) are learned, neural representations of a density and color field that can be used to render novel views of a scene via volumetric rendering. These techniques are a hot topic in the graphics community, but questions abound about their applicability to mobile robotics. Some algorithms capable of online learning of a scene have been proposed (see [iMAP](https://edgarsucar.github.io/iMAP/) and [NeRF-SLAM](https://github.com/ToniRV/NeRF-SLAM) for examples), but these are very new methods that model room-scale scenes and require high-quality GPUs. Planetary robotics poses a challenge for such techniques due to the often extreme lighting conditions, lack of features in a scene, and limited motion of the image sensors, in addition to the problem of compute. This project seeks to assess the practicability of using NeRFs for modeling lunar terrain, with a focus on geometric aspects in addition to photometric.
