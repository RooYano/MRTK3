# Mixed Reality Toolkit for Unity

![Mixed Reality Toolkit](https://user-images.githubusercontent.com/13754172/122838732-89ea3400-d2ab-11eb-8c79-32dd84944989.png)

![MRTK3 Banner](./Images/MRTK3_banner.png)

**MRTK3** is the third generation of the Mixed Reality Toolkit for Unity. It's an open source project designed to accelerate cross-platform mixed reality development in Unity. MRTK3 is built on top of [Unity's XR Interaction Toolkit (XRI)](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@2.1/manual/index.html) and OpenXR. This new generation of MRTK is intended to be faster, cleaner, and more modular, with an easier cross-platform development workflow enabled by OpenXR and the Unity Input System.

## Key improvements

### Architecture

* Built on Unity XR Interaction Toolkit and the Unity Input System.
* Dedicated to OpenXR, with flexibility for other XRSDK backends
* Open-ended and extensible interaction paradigms across devices, platforms, and applications

### Performance

* Rewrote and redesigned most features and systems, from UX to input to subsystems.
* Zero per-frame memory allocation.
* Tuned for maximum performance on HoloLens 2 and other resource-constrained mobile platforms.

### UI

* New interaction models (gaze-pinch indirect manipulation).
* Updated Mixed Reality Design Language.
* Unity Canvas + 3D UX: production-grade dynamic auto-layout.
* Unified 2D & 3D input for gamepad, mouse, and accessibility support.
* Data binding for branding, theming, dynamic data, and complex lists.

## Requirements

MRTK3 requires Unity 2021.3.21 or higher. In addition, you need the [Mixed Reality Feature Tool for Unity](https://aka.ms/mrfeaturetool) to find, download, and add the packages to your project.

## Getting started

[Follow the documentation for setting up MRTK3 packages as dependencies in your project here.](https://learn.microsoft.com/windows/mixed-reality/mrtk-unity/mrtk3-overview/getting-started/setting-up/setup-new-project) Alternatively, you can clone this repo directly to experiment with our template project. However, we *strongly* recommend adding MRTK3 packages as dependencies through the Feature Tool, as it makes updating, managing, and consuming MRTK3 packages far easier and less error-prone.

## Supported devices

| Platform | Supported Devices |
|---|---|
| OpenXR devices | Microsoft HoloLens 2 <br> Magic Leap 2 <br> Meta Quest 1/2 <br> Windows Mixed Reality (experimental) <br> SteamVR (experimental) <br> Oculus Rift on OpenXR (experimental) <br> Varjo XR-3 (experimental) <br> **If your OpenXR device already works with MRTK3, let us know!**
| Windows | Traditional flat-screen desktop (experimental)
| And more coming soon! |

## Versioning

In previous versions of MRTK (HoloToolkit and MRTK v2), all packages were released as a complete set, marked with the same version number (ex: 2.8.0). Starting with MRTK3 GA, each package will be individually versioned, following the [Semantic Versioning 2.0.0 specification](https://semver.org/spec/v2.0.0.html). (As a result, the '3' in MRTK3 is not a version number!)


Individual versioning will enable faster servicing while providing improved developer understanding of the magnitude of changes and reducing the number of packages needing to be updated to acquire the desired fix(es).

For example, if a non-breaking new feature is added to the UX core package, which contains the logic for user interface behavior the minor version number will increase (from 3.0.x to 3.1.0). Since the change is non-breaking, the UX components package, which depends upon UX core, is not required to be updated. 

As a result of this change, there is not a unified MRTK3 product version.

To help identify specific packages and their versions, MRTK3 provides an about dialog that lists the relevant packages included in the project. To access this dialog, select `Mixed Reality` > `MRTK3` > `About MRTK` from the Unity Editor menu.

![About MRTK Panel](Images/AboutMRTK.png)

# Getting started with MRTK

If you're new to MRTK or Mixed Reality development in Unity, we recommend you start at the beginning of our Unity development journey in the [Microsoft Docs](https://learn.microsoft.com/en-us/windows/mixed-reality/develop/unity/unity-development-overview?tabs=arr%2CD365%2Chl2). The Unity development journey is specifically tailored to walk new developers through the installation, core concepts, and usage of MRTK.

# Feature areas

| [![Input System](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_InputSystem.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/overview)<br/>[Input System](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/overview)<br/>&nbsp; | [![Hand Tracking<br/> (HoloLens 2)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_HandTracking.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/hand-tracking)<br/>[Hand Tracking<br/> (HoloLens 2)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/hand-tracking)<br/>&nbsp; | [![Eye Tracking<br/> (HoloLens 2)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_EyeTracking.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-main)<br/>[Eye Tracking<br/> (HoloLens 2)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-main)<br/>&nbsp; | [![Profiles](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_Profiles.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/configuration/mixed-reality-configuration-guide)<br/>[Profiles](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/configuration/mixed-reality-configuration-guide)<br/>&nbsp; | [![Hand Tracking<br/> (Ultraleap)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_HandTracking.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/supported-devices/leap-motion-mrtk)<br/>[Hand Tracking<br/>(Ultraleap)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/supported-devices/leap-motion-mrtk)<br/>&nbsp; |
| :--- | :--- | :--- | :--- | :--- |
| [![UI Controls](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_UIControls.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/#ux-building-blocks)<br/>[UI Controls](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/#ux-building-blocks)<br/>&nbsp; | [![Solvers](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_Solver.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/solvers/solver)<br/>[Solvers](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/solvers/solver)<br/>&nbsp; | [![Multi-Scene<br/> Manager](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_SceneSystem.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/scene-system/scene-system-getting-started)<br/>[Multi-Scene<br/> Manager](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/scene-system/scene-system-getting-started) | [![Spatial<br/> Awareness](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_SpatialUnderstanding.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/spatial-awareness/spatial-awareness-getting-started)<br/>[Spatial<br/> Awareness](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/spatial-awareness/spatial-awareness-getting-started) | [![Diagnostic<br/> Tool](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_Diagnostics.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/diagnostics/diagnostics-system-getting-started)<br/>[Diagnostic<br/> Tool](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/diagnostics/diagnostics-system-getting-started) |
| [![MRTK Standard Shader](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_StandardShader.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/rendering/mrtk-standard-shader)<br/>[MRTK Standard<br/>Shader](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/rendering/mrtk-standard-shader) | [![Speech & Dictation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_VoiceCommand.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/speech)<br/>[Speech](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/speech)<br/> & [Dictation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/dictation) | [![Boundary<br/>System](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_Boundary.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/boundary/boundary-system-getting-started)<br/>[Boundary<br/>System](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/boundary/boundary-system-getting-started)| [![In-Editor<br/>Simulation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_InputSystem.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input-simulation/input-simulation-service)<br/>[In-Editor<br/>Simulation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input-simulation/input-simulation-service) | [![Experimental<br/>Features](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK_Icon_Experimental.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/contributing/experimental-features)<br/>[Experimental<br/>Features](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/contributing/experimental-features)|

# UX building blocks

|  [![Button](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Button/MRTK_Button_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/button) [Button](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/button) | [![Bounds Control](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/bounds-control/MRTK_BoundsControl_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/bounds-control) [Bounds Control](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/bounds-control) | [![Object Manipulator](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/manipulation-handler/MRTK_Manipulation_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/object-manipulator) [Object Manipulator](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/object-manipulator) |
|:--- | :--- | :--- |
| A button control which supports various input methods, including HoloLens 2's articulated hand | Standard UI for manipulating objects in 3D space | Script for manipulating objects with one or two hands |
|  [![Slate](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Slate/MRTK_Slate_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/slate) [Slate](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/slate) | [![System Keyboard](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/system-keyboard/MRTK_SystemKeyboard_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/system-keyboard) [System Keyboard](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/system-keyboard) | [![Interactable](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Interactable/InteractableExamples.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/interactable) [Interactable](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/interactable) |
| 2D style plane which supports scrolling with articulated hand input | Example script of using the system keyboard in Unity  | A script for making objects interactable with visual states and theme support |
|  [![Solver](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Solver/MRTK_Solver_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/solvers/solver) [Solver](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/solvers/solver) | [![Object Collection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/object-collection/MRTK_ObjectCollection_Main.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/object-collection) [Object Collection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/object-collection) | [![Tooltip](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Tooltip/MRTK_Tooltip_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/tooltip) [Tooltip](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/tooltip) |
| Various object positioning behaviors such as tag-along, body-lock, constant view size and surface magnetism | Script for laying out an array of objects in a three-dimensional shape | Annotation UI with a flexible anchor/pivot system, which can be used for labeling motion controllers and objects |
|  [![Slider](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Slider/MRTK_UX_Slider_Main.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/sliders) [Slider](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/sliders) | [![MRTK Standard Shader](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK-Standard-Shader/MRTK_StandardShader.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/rendering/mrtk-standard-shader) [MRTK Standard Shader](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/rendering/mrtk-standard-shader) | [![Hand Menu](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Solver/MRTK_UX_HandMenu.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/hand-menu) [Hand Menu](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/hand-menu) |
| Slider UI for adjusting values supporting direct hand tracking interaction | MRTK's Standard shader supports various Fluent design elements with performance | Hand-locked UI for quick access, using the Hand Constraint Solver |
|  [![App Bar](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/app-bar/MRTK_AppBar_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/app-bar) [App Bar](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/app-bar) | [![Pointers](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Pointers/MRTK_Pointer_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/pointers) [Pointers](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/pointers) | [![Fingertip Visualization](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Fingertip/MRTK_FingertipVisualization_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/fingertip-visualization) [Fingertip Visualization](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/fingertip-visualization) |
| UI for Bounds Control's manual activation | Learn about various types of pointers | Visual affordance on the fingertip which improves the confidence for the direct interaction |
|  [![Near Menu](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/near-menu/MRTK_UX_NearMenu.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/near-menu) [Near Menu](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/near-menu) | [![Spatial Awareness](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/spatial-awareness/MRTK_SpatialAwareness_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/spatial-awareness/spatial-awareness-getting-started) [Spatial Awareness](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/spatial-awareness/spatial-awareness-getting-started) | [![Voice Command](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Input/MRTK_Input_Speech.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/speech) [Voice Command](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/speech) / [Dictation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/dictation) |
| Floating menu UI for the near interactions | Make your holographic objects interact with the physical environments | Scripts and examples for integrating speech input |
|  [![Progress Indicator](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/progress-indicator/MRTK_ProgressIndicator_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/progress-indicator) [Progress Indicator](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/progress-indicator) | [![Dialog](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Dialog/MRTK_UX_Dialog_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/dialog) [Dialog [Experimental]](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/dialog) | [![Hand Coach](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/hand-coach/MRTK_UX_HandCoach_Main.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/hand-coach) [Hand Coach](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/hand-coach) |
| Visual indicator for communicating data process or operation | UI for asking for user's confirmation or acknowledgement  | Component that helps guide the user when the gesture has not been taught |
|  [![Hand Physics Service](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/hand-physics/MRTK_UX_HandPhysics_Main.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/experimental/hand-physics-service) [Hand Physics Service [Experimental]](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/experimental/hand-physics-service) | [![Scrolling Collection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/scrolling-collection/ScrollingCollection_Main.jpg)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/scrolling-object-collection) [Scrolling Collection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/ux-building-blocks/scrolling-object-collection) | [![Dock](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/Dock/MRTK_UX_Dock_Main.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/experimental/dock) [Dock [Experimental]](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/experimental/dock) |
| The hand physics service enables rigid body collision events and interactions with articulated hands | An Object Collection that natively scrolls 3D objects | The Dock allows objects to be moved in and out of predetermined positions |
|  [![Eye Tracking: Target Selection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/eye-tracking/mrtk_et_targetselect.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-target-selection) [Eye Tracking: Target Selection](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-target-selection) | [![Eye Tracking: Navigation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/eye-tracking/mrtk_et_navigation.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-navigation) [Eye Tracking: Navigation](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/input/eye-tracking/eye-tracking-navigation) | [![Eye Tracking: Heat Map](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/eye-tracking/mrtk_et_heatmaps.png)](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/example-scenes/eye-tracking-examples-overview#visualization-of-visual-attention) [Eye Tracking: Heat Map](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/example-scenes/eye-tracking-examples-overview#visualization-of-visual-attention) |
| Combine eyes, voice and hand input to quickly and effortlessly select holograms across your scene | Learn how to auto-scroll text or fluently zoom into focused content based on what you are looking at | Examples for logging, loading and visualizing what users have been looking at in your app |


## Early preview packages

Some parts of MRTK3 are at earlier stages of the development process than others. Early preview packages can be identified in the Mixed Reality Feature Tool and Unity Package Manager by the `Early Preview` designation in their names.

As of June 2022, the following components are considered to be in early preview.

| Name | Package Name |
| --- | --- |
| Accessibility | org.mixedrealitytoolkit.accessibility |
| Data Binding and Theming | org.mixedrealitytoolkit.data |

The MRTK team is fully committed to releasing this functionality. It is important to note that the packages may not contain the complete feature set that is planned to be released or they may undergo major, breaking architectural changes before release.

We very much encourage you to provide any and all feedback to help shape the final form of these early preview features.

## Contributing

This project welcomes contributions, suggestions, and feedback. All contributions, suggestions, and feedback you submitted are accepted under the [Project's license](./LICENSE.md). You represent that if you do not own copyright in the code that you have the authority to submit it under the [Project's license](./LICENSE.md). All feedback, suggestions, or contributions are not confidential.

For more information on how to contribute Mixed Reality Toolkit for Unity Project, please read [CONTRIBUTING.md](./CONTRIBUTING.md).

## Governance

For information on how the Mixed Reality Toolkit for Unity Project is governed, please read [GOVERNANCE.md](./GOVERNANCE.md).
