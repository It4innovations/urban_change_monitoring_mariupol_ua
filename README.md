# Monitoring Urban Changes in Mariupol/Ukraine

This repository demonstrates the transferred ERCNN-DRS to monitor urban changes in Mariupol/Ukraine in 2022/23.

Maximum values over all detected urban changes, superimposed in red (Nov. 2021 - July 2023):
<p align="center">
  <img src="./images/s12_grid_Mariupol_comb_pred.png" />
</p>

Changes with moving half-year window (Nov. 2021 - July 2023):
<p align="center">
  <img src="./images/Mariupol_11_2021-07_2023.gif" />
</p>

Video file is located [here](./images/Mariupol_11_2021-07_2023.mp4).


The urban changes were detected and monitored with a transferred version of the pre-trained [ERCNN-DRS model](https://github.com/It4innovations/ERCNN-DRS_urban_change_monitoring) for Sentinel 1 & 2 missions.

The windowed observations were pre-processed with [rsdtlib](https://github.com/It4innovations/rsdtlib). This library downloads all Sentinel 1 & 2 observations from [Sentinel Hub](https://www.sentinel-hub.com/) and pre-processes the observations for time series analysis (windowing). This library was used for training and inference. We used as time frame November 2021 up to today (July 2023), with sliding windows of six month duration.

# Paper and Citation
TBD

# Contact
Should you have any feedback or questions, please contact the main author: Georg Zitzlsberger (georg.zitzlsberger(a)vsb.cz).

# Acknowledgments
This research was funded by the Ministry of Education, Youth and Sports from the National Programme of Sustainability (NPS II) project “IT4Innovations excellence in science - LQ1602” and by the IT4Innovations Infrastructure, which is supported by the Ministry of Education, Youth and Sports of the Czech Republic through the e-INFRA CZ (ID:90140), and via the Open Access Grant Competition (OPEN-25-24 and OPEN-27-1). This work was also supported by ESA Network of Resources Initiative to provide access to Sentinel Hub, and Airbus Pléiades.

We also would like to thank CESNET Meta Centrum for providing us access to a DGX H100 node.

# License
This project is made available under the GNU General Public License, version 3 (GPLv3).

# Disclaimer
This work and results is active research and subject of change. They hence are provided "as is", without guarantee of correctness or liability. Use at your own risk.

# Ethical Statement
Due to the ongoing Russian-Ukrainian war, the selection of locations of visual samples was done with care to minimize risks of influence and harm. To the best of our knowledge, we only selected locations and data that did not give direct insight to the ongoing war, but only documented the resulting (urban) changes. We also would like to underline that our monitoring methods used six-month windows and hence did not and shall not provide real-time information that could be used for military purposes. Our methods are optimized for inertial urban changes that manifest over longer periods.
