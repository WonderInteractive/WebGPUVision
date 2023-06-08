
## WebGPUVision - NOT YET RELEASED PUBLICLY. This repo currently exists for feedback before release.

## Overview

WebGPUVision is a multi-platform graphics debugging and profiling tool designed specifically for WebGPU. It combines powerful debugging capabilities with innovative features, such as live remote viewing, profiling data, and AI-assisted call graph optimization, offering unparalleled insights and improvements for your rendering code. It is designed to operate even within a browser environment, offering unprecedented flexibility and utility.

## Goals
- Be lightweight
- Be easy to mod and extend, promoting collaboration on development
- Run anywhere WebGPU is supported
- Written in C++20
- Quick and light weight serialization and deserialization of calls
- Build process should be as simple and as quick as possible

## Features

- [x] **Frame Capture**: Captures individual frames from a running application, offering a granular view of your rendering code in action.
    
- [x] **Debugging and Profiling**: Provides a comprehensive debugging suite, along with rich profiling data to enhance performance and optimization.
    
- [x] **Live Frame Recording and Playback**: Can enable automatic N frame capturing with compression, so you don't miss a frame.

- [x] **Live Remote Debugging**: Enables live remote debugging of WebGPU frames, offering real-time insights no matter where you are.
    
- [x] **Multi-Platform Support**: 
	- [x] Windows
	- [ ] Linux
	- [ ] macOS
	- [x] Firefox, Safari and Chromium browsers
    
- [x] **Shader Editing**: Supports live shader editing, promoting iterative testing.

- [ ] **Shader Debugging**: Supports live shader debugging.
    
- [x] **Texture and API Inspection**: Offers detailed views of the textures used in rendering the frame and insightful scrutiny of API calls.

- [x] **Detailed Resource Usage Reporting**: Provides comprehensive reports on resource usage, enabling developers to optimize their applications efficiently.

- [x] **Customizable UI**: Allows users to tailor the user interface to their personal preferences and workflow.
    
- [ ] **Benchmarking Tool**: A built-in feature to allow users to benchmark and compare the performance of different versions of their code or different rendering techniques.
    
- [ ] **Cross-API Comparison**: Offers a comparison tool between equivalent WebGPU and WebGL (or others) calls to aid developers transitioning between APIs.
    
- [ ] **Collaborative Debugging**: Allows multiple users to view and debug a rendering in real-time, promoting team collaboration and learning.
    
- [ ] **Interactive Tutorials and Guides**: Provides interactive guides that explain the tool's features and how to utilize them effectively.
    
## Maybes

- [ ] **AI-Assisted Call Graph Optimizer**: Leverage the power of artificial intelligence to get rendering optimization tips to reduce bottlenecks and improve efficiency.

## Installation

WebGPUVision has currently been built and tested for Windows 11 x64 and Chrome (using Emscripten).
- Building for windows

	    cmake -G "Visual Studio 17 2022"
	    cmake --build . --config [Debug or Release]
	    or
	    cmake -G "Ninja" -DCMAKE_BUILD_TYPE=[Debug or Release]
	    cmake --build .
	    

- Building for the browser

	    emcmake cmake -G "Ninja" -DCMAKE_BUILD_TYPE=[Debug or Release]
	    cmake --build .

In browser demo here: [DEMO](https://theimmersiveweb.com/experiments/WebGPUVisionDemo)

## Usage

WebGPUVision provides a user interface for frame capturing and inspecting applications locally or remotely. It also allows direct embedding into your application via its API for seamless integration and on-demand captures.

For a comprehensive guide on how to use WebGPUVision, please refer to our official documentation.

## Contributing

As an open-source project, WebGPUVision encourages community involvement. From reporting bugs, requesting features, to direct code contributions, your participation is highly valued. More information on contributing can be found in our CONTRIBUTING.md file.

## License

WebGPUVision is licensed under the Apache License, Version 2.0. For detailed information, please see our LICENSE.md file.
