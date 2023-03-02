# Estimating circles from corners

Welcome to this lab in the computer vision course [TEK5030] at the University of Oslo.

In this lab we will
- Create our own corner keypoint detector `CornerDetector`.
- Use detected corner keypoints and RANSAC to find a circle with the `CircleEstimator` class.

Start by cloning this repository on your machine. 
Then open the lab project in your editor.

The lab is carried out by following these steps:

1. [Get an overview](lab-guide/1-get-an-overview.md)
2. [Implement a corner feature detector](lab-guide/2-implement-a-corner-feature-detector.md)
3. [Detect circles from corners with RANSAC](lab-guide/3-detect-circles-from-corners-with-ransac.md)

You will find our proposed solution at https://github.com/tek5030/solution-corners.
But please try to solve the lab with help from others instead of just jumping straight to the solution ;)

Start the lab by going to the [first step](lab-guide/1-get-an-overview.md).

## Prerequisites
- [Ensure Conan is installed on your system][conan], unless you are not on a lab computer.
- Install project dependencies using conan:

   ```bash
   # git clone https://github.com/tek5030/lab-corners.git
   # cd lab-corners

   conan install . --install-folder=build --build=missing
   ```
- When you configure the project in CLion, remember to set `build` as the _Build directory_, as described in [lab_intro].

[TEK5030]: https://www.uio.no/studier/emner/matnat/its/TEK5030/
[conan]: https://tek5030.github.io/tutorial/conan.html
[lab_intro]: https://github.com/tek5030/lab-intro/blob/master/cpp/lab-guide/1-open-project-in-clion.md#6-configure-project