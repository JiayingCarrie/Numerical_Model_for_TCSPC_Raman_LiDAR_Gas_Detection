# Numerical Model for TCSPC Raman LiDAR Gas Detection
This Google Colaboratory notebook implements a numerical model for Time-Correlated Single-Photon Counting (TCSPC) signal processing, specifically applied to Raman LiDAR for the stand-off detection of hydrogen and nitrogen (H2 and N2). Developed by Jiaying Wang, Andrew Lockwood, and Charles N. Ironside (Curtin University), the code supports the analysis of experimental data and was developed for the paper "Time-correlated single-photon counting (TCSPC) Raman LiDAR for stand-off detection of hydrogen".

**LiDAR Equation Update:** The spatial sample distance $\Delta z$ in the LiDAR equation has been corrected to use the TCSPC range-bin length, $\delta z = c\delta t/2$, where $\delta t$ is the TCSPC time-bin width and $c$ is the speed of light. We now use $\Delta z$ to designate the range uncertainty. The range uncertainty is associated with the laser pulse width, $P_w$, which contributes to the spatial resolution, with a pulse-width-limited range resolution of $\Delta z = cP_w$. If $P_w>\delta t$, then the laser pulse width dominates the spatial resolution.

In summary, there are two contributions to the spatial resolution: the sample region length, $\delta z = c\delta t/2$, and the pulse-width-limited range resolution, $\Delta z = cP_w$. For the case discussed in the publication (see below), $\delta t=50 ps$ and $P_w=1.1 ns$, and so the spatial resolution is dominated by the laser pulse width.

**See the publication:** -
A. Lockwood, J. Wang, and C. N. Ironside, "Time-correlated single-photon counting (TCSPC) Raman LiDAR for stand-off detection of hydrogen," Optics & Laser Technology, vol. 203, p. 115721, 2026/11/01/ 2026, doi: https://doi.org/10.1016/j.optlastec.2026.115721.
