# Ray Tracing Renderer

A C++ implementation of a ray tracing renderer that simulates light physics to create realistic 3D scenes.

## Features

- Realistic lighting simulation with ambient, diffuse, and specular components
- Support for reflective surfaces with configurable reflectivity
- Shadow calculation for realistic light occlusion
- Multiple object types (spheres and planes)
- Customizable materials with various properties (color, shininess, reflectivity)
- Animation capabilities for creating video sequences

### Prerequisites
- C++ compiler with C++11 support
- Visual Studio 2019 or later

### Creating Videos from Frames
After generating animation frames, you can create a video using ffmpeg:
ffmpeg -framerate 30 -i frame_%d.ppm -c libx264 -pix_fmt yuv420p animation.mp4

## Project Structure

- `Color.h/cpp`: Color representation and operations
- `Material.h/cpp`: Material properties like color, reflectivity
- `Vector3D.h/cpp`: 3D vector operations
- `Ray.h/cpp`: Ray representation 
- `Sphere.h/cpp`: Implementation of spheres
- `Plane.h/cpp`: Implementation of planes
- `Light.h/cpp`: Light source representation
- `Scene.h/cpp`: Scene management
- `Raytracer.h/cpp`: Core ray tracing algorithm

## Acknowledgments

- This project was created as part of a computer graphics course
