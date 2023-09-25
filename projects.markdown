---
layout: projects
title: Projects
id: projects
order: 1
permalink: /projects/

projects:
 - name: Lunar NeRFs
   image_link: 
   alt_text: 
   description: Neural radiance fields (<a href="https://www.matthewtancik.com/nerf">NeRFs</a>) are learned, neural representations of a density and color field that can be used to render novel views of a scene via volumetric rendering. These techniques are a hot topic in the graphics community, but questions abound about their applicability to mobile robotics. Some algorithms capable of online learning of a scene have been proposed (see <a href="https://edgarsucar.github.io/iMAP/">iMAP</a> and <a href="https://github.com/ToniRV/NeRF-SLAM">NeRF-SLAM</a> for examples), but these are very new methods that model room-scale scenes and require high-quality GPUs. Planetary robotics poses a challenge for such techniques due to the often extreme lighting conditions, lack of features in a scene, and limited motion of the image sensors, in addition to the problem of compute. This project seeks to assess the practicability of using NeRFs for modeling lunar terrain, with a focus on geometric aspects in addition to photometric. 

 - name: Spectral Mixture Ergodic Search
   image_link: /assets/sm_es_cuprite_crop.gif
   alt_text: GIF of map and trajectory
   description: Spectral mixture kernels are covariance kernels for methods such as Gaussian process regression that are capable of theoretically learning any stationary covariance structure by representing the inverse Fourier transform of the kernel as a Gaussian mixture model. Ergodic search likewise relies on Fourier decomposition to compute the loss metric used in its optimization procedure, typically relying on a pre-determined set of frequencies and knowledge of the information distribution over which search is to occur. This project seeks to use the Fourier decompositions present in both methods to link the two such that as a spatial distribution is learned via Gaussian process regression with spectral mixture kernels, the ergodic search algorithm is adapted to use the frequencies found to be important for describing the distribution.

 - name: Range-based GP Maps
   image_link: /assets/rover_graphic.png
   alt_text: Graphic of rover observing terrain
   description: This work was borne out of a recognition that one main method to model spatial correlations in terrain - Gaussian process regression - is typically only applied to elevation, especially in the context of planetary rovers. Elevation-based models work well for orbital images, since the sensor noise is well aligned with the terrain height. However, for a ground-based rover, perception sensors will record data at an oblique angle to the terrain, meaning the sensor uncertainty also has components in the x and y directions. Range-based Gaussian process maps model range measurements directly as a function of the inclination and azimuth of the ray along which an observation was taken, enabling correct modeling of uncertainty along with incorporation of spatial correlations. Work has thus far focused on local mapping for LiDAR sensors.
   
 - name: MoonRanger
   image_link: /assets/morphin.jpg
   alt_text: Prototype rover in test bed
   description: <a href="https://labs.ri.cmu.edu/moonranger/">MoonRanger</a> is a microrover designed by Astrobotic to search for volatiles (ice) at the south pole of the moon. As part of this project, I designed, authored, and tested the mapping component of the flight software, in addition to being an active participant in integrated testing of the autonomous navigation software on a prototype rover. The mapping software is based on older designs that rely on terrain meshes, with improvements such as edge detection in disparity images to ensure higher preservation of points of interest. Integrated testing occurs in the Moonyard test bed in the Planetary Robotics Lab at CMU and has included such diverse tasks as using motion capture to track ground-truth location of the robot, validating the mapping system against dense ground truth information produced by a FARO scanner, and performing repeated iterations of parameter modification and testing.
---

