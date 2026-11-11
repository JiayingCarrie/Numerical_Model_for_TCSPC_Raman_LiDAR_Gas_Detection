# Numerical Model for TCSPC Raman LiDAR Gas Detection
This Google Colaboratory notebook implements a numerical model for Time-Correlated Single-Photon Counting (TCSPC) signal processing, specifically applied to Raman LiDAR for the stand-off detection of hydrogen and nitrogen (H2 and N2). Developed by Jiaying Wang, Andrew Lockwood, and Charles N. Ironside (Curtin University), the code supports the analysis of experimental data and was developed for the paper "Time-correlated single-photon counting (TCSPC) Raman LiDAR for stand-off detection of hydrogen".

**LiDAR Equation Update:** The spatial interval $\Delta z$ in the LiDAR equation has been corrected to use the TCSPC range-bin thickness, $\delta z = c\delta t/2$, where $\delta t$ is the TCSPC time-bin width and $c$ is the speed of light. The laser pulse width contributes to the spatial resolution, with a theoretical pulse-width-limited range resolution of $\Delta z = cP_w/2$, where $P_w$ is the laser pulse width. The effective spatial resolution also depends on the detector timing response.

**See the publication:** -
A. Lockwood, J. Wang, and C. N. Ironside, "Time-correlated single-photon counting (TCSPC) Raman LiDAR for stand-off detection of hydrogen," Optics & Laser Technology, vol. 203, p. 115721, 2026/11/01/ 2026, doi: https://doi.org/10.1016/j.optlastec.2026.115721.
