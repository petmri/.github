# petmri

Welcome to the **petmri** GitHub organization — home of open-source tools for DCE-MRI processing, analysis, and machine learning.

🌐 **[petmri.github.io](https://petmri.github.io)**

---

## Projects

### [dce2bids](https://github.com/petmri/dce2bids)
Convert DCE-MRI DICOM scans to BIDS format with the help of an AI coding assistant (requires Claude Code, ChatGPT Codex, or equivalent). No coding required, just a single prompt. Handles dynamic DCE series, VFA flip-angle scans, and structural scans. After an initial AI-assisted setup for your scanner and protocol, subsequent conversions run with a single command — no AI required.

### [AutoAIF](https://github.com/petmri/AutoAIF)
Automatic detection of the arterial input function (AIF) for brain DCE-MRI in multi-site cohorts. Uses a 3D U-Net (Keras/TensorFlow) with pretrained weights. Predicts a vascular function curve and a 3D mask, resampled back to original image dimensions.

> Saca, L., et al. [Automatic detection of arterial input function for brain DCE-MRI in multi-site cohorts](https://onlinelibrary.wiley.com/doi/10.1002/mrm.70020). *Magnetic Resonance in Medicine*, 94(6), 2732–2744 (2025).

### [AIFArtist](https://github.com/petmri/AIFArtist)
A desktop app for streamlined **manual** AIF annotation on 4D MRI NIfTI data. Designed for high-volume review sessions with minimal clicks: draw a 3D ROI, inspect mean signal-intensity curves over time, save BIDS-style derivatives, and move on to the next image. Supports multiple raters and auto-resumes at the first unreviewed image.

### [ROCKETSHIP](https://github.com/petmri/ROCKETSHIP)
A flexible and modular toolbox for processing and analyzing parametric MRI and DCE-MRI data. Supports many DCE models (Patlak, Tofts, Ex Tofts, 2CXM, others), and batch processing of large amounts of BIDS formatted data. Developed at the Biological Imaging Center at Caltech and Loma Linda University.

> Ng, T.S.C., et al. [ROCKETSHIP: a flexible and modular software tool for the planning, processing and analysis of dynamic MRI studies](https://doi.org/10.1186/s12880-015-0062-3). *BMC Medical Imaging*, 15, 19 (2015).

### [Gpufit](https://github.com/petmri/Gpufit)
Implementation of Levenberg–Marquardt curve fitting in CUDA. Adds MRI-relevant pharmacokinetic models: Patlak, Tofts, Extended Tofts, Tissue Uptake, 2CXM, and T1 FA Exponential. Includes pre-built binaries for Windows, Linux, and macOS. Library code that can be used to accelerate a DCE implementation, automatically installed with ROCKETSHIP.

> Gpufit manuscript: [Scientific Reports](https://www.nature.com/articles/s41598-017-15313-9)
