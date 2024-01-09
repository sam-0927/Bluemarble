# Bluemarble

### Submitted to Signal Processing Letters (SPL-38529-2024)

## Abstract

<img src='architecture.png'>

In this paper, we introduce BlueMarble, a neural articulation-to-speech (ATS) system that synthesizes high-quality speech from articulatory recordings. Conventional ATS approaches are only available for high-resource datasets, which require parallel articulatory and speech signal pairs for network training. These approaches often treat acoustic feature estimation as a regression task, which can pose challenges in accurately mapping complex latent features to targets. We address this task by utilizing a finite learned codebook to limit the size of the uncertainty space.  Our model learns a mapping from electromagnetic articulography (EMA) signals to discrete speech tokens from a pretrained encoder-decoder model. Then, a decoder network utilizes the discrete EMA tokens to predict acoustic features, which are fed into a neural vocoder to synthesize speech. Experimental results show that our approach outperforms existing state-of-the-art methods in both qualitative and quantitative assessments. 

## Sample

[10]: "An improved model for voicing silent speech" in ACL, 2021 <br>
[11]: “Deep speech synthesis from articulatory representations” in INTERSPEECH, 2022 <br>
[12]: “Style modeling for multispeaker articulation-to-speech” in ICASSP, 2023 <br>

<!-- <audio controls><source src='./demo_sample/F01_B02_S60_R02_N.wav'></audio> -->
<!-- <table style="width: auto; table-layout: fixed; word-wrap: normal; text-align: center;" borded="1" border-collapse="collapse"> 
<tr>
  <td style="column-width: 300px; padding-left: 10px; padding-right: 10px"><strong>Reference</strong></td>
	<td style="column-width: 300px; padding-left: 10px; padding-right: 10px"><strong>[10]</strong></td>
	<td style="column-width: 300px; padding-left: 10px; padding-right: 10px"><strong>[11]</strong></td>
	<td style="column-width: 300px; padding-left: 10px; padding-right: 10px"><strong>[12]</strong></td>
	<td style="column-width: 300px; padding-left: 10px; padding-right: 10px"><strong>Bluemarble (Ours)</strong></td>
</tr> -->
<table style="width: 100%; word-wrap: normal; text-align: center;" borded="1" border-collapse="collapse">
<tr>
<td style="column-width: 20\%"><strong>Sample index</strong></td>
<td style="column-width: 20\%"><strong>1</strong></td>
<td style="column-width: 20\%"><strong>2</strong></td>
<td style="column-width: 20\%"><strong>3</strong></td>
<td style="column-width: 20\%"><strong>4</strong></td>
<td style="column-width: 20\%"><strong>5</strong></td>
<td style="column-width: 20\%"><strong>6</strong></td>
<td style="column-width: 20\%"><strong>7</strong></td>
<td style="column-width: 20\%"><strong>8</strong></td>
<td style="column-width: 20\%"><strong>9</strong></td>
<td style="column-width: 20\%"><strong>10</strong></td>
<td style="column-width: 20\%"><strong>11</strong></td>
<td style="column-width: 20\%"><strong>12</strong></td>
<td style="column-width: 20\%"><strong>13</strong></td>
<td style="column-width: 20\%"><strong>14</strong></td>
<td style="column-width: 20\%"><strong>15</strong></td>
<td style="column-width: 20\%"><strong>16</strong></td>
<td style="column-width: 20\%"><strong>17</strong></td>
<td style="column-width: 20\%"><strong>18</strong></td>
<td style="column-width: 20\%"><strong>19</strong></td>
<td style="column-width: 20\%"><strong>20</strong></td>
<td style="column-width: 20\%"><strong>21</strong></td>
<td style="column-width: 20\%"><strong>22</strong></td>
<td style="column-width: 20\%"><strong>23</strong></td>
<td style="column-width: 20\%"><strong>24</strong></td>
<td style="column-width: 20\%"><strong>25</strong></td>
<td style="column-width: 20\%"><strong>26</strong></td>
<td style="column-width: 20\%"><strong>27</strong></td>
<td style="column-width: 20\%"><strong>28</strong></td>
<td style="column-width: 20\%"><strong>29</strong></td>
<td style="column-width: 20\%"><strong>30</strong></td>
<td style="column-width: 20\%"><strong>31</strong></td>
<td style="column-width: 20\%"><strong>32</strong></td>
<td style="column-width: 20\%"><strong>33</strong></td>
<td style="column-width: 20\%"><strong>34</strong></td>
<td style="column-width: 20\%"><strong>35</strong></td>
<td style="column-width: 20\%"><strong>36</strong></td>
<td style="column-width: 20\%"><strong>37</strong></td>
<td style="column-width: 20\%"><strong>38</strong></td>
</tr>
<tr>
<td style="column-width: 20\%"><strong>Reference</strong></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S09_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S29_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S38_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B05_S49_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B02_S14_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B04_S48_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S15_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S12_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S52_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S37_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S06_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S44_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B06_S13_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B01_S43_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B02_S51_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S39_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S02_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B04_S57_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S08_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B02_S60_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B01_S26_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S02_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B04_S54_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S51_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B01_S10_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S13_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B07_S60_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S35_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S26_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B01_S53_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S24_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S22_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S17_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B02_S51_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B01_S16_R02_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S24_R01_F_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B06_S34_R01_N_target.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S54_R01_N_target.wav></audio></td>
</tr>

<tr>
<td style="column-width: 20\%"><strong>[10]</strong></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S35_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B01_S26_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B01_S43_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S24_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S02_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B04_S57_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B01_S10_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S17_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S51_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S06_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S02_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S15_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B06_S13_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B04_S54_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S24_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S13_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S26_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B07_S60_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B02_S51_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B01_S16_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S29_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S22_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B02_S60_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S39_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S12_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S09_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S38_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S52_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B04_S48_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B06_S34_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B02_S14_R01_F_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S37_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S54_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S44_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B05_S49_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B02_S51_R02_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S08_R01_N_base.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B01_S53_R01_N_base.wav></audio></td>
</tr>
<tr>
<td style="column-width: 20\%"><strong>[11]</strong></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S29_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S51_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S12_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S15_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B01_S26_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B01_S53_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B06_S34_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B01_S16_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S52_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S06_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B07_S60_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S02_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B02_S51_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S22_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B01_S43_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B02_S51_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S24_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S35_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B05_S49_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S02_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S26_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B06_S13_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S54_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B02_S60_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S08_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B02_S14_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B04_S48_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S44_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B04_S57_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S13_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S24_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S38_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B01_S10_R02_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S39_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S09_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S37_R01_N_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S17_R01_F_deep.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B04_S54_R01_N_deep.wav></audio></td>
</tr>
<tr>
<td style="column-width: 20\%"><strong>[12]</strong></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S09_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S26_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S02_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S39_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S37_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S13_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S29_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S06_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B02_S51_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B04_S48_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S54_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S44_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B06_S34_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B04_S57_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S12_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S22_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B01_S10_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B07_S60_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S52_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S51_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S24_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S38_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B01_S53_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S02_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B04_S54_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B02_S14_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B01_S16_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B06_S13_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S08_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S17_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B05_S49_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B02_S60_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S35_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S15_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B02_S51_R02_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B01_S43_R01_N_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B01_S26_R01_F_msota.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S24_R01_F_msota.wav></audio></td>
</tr>
<tr>
<td style="column-width: 20\%"><strong>Bluemarble (Ours)</strong></td>
 <td><audio controls><source src='./demo_sample/'M01_B02_S51_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B07_S60_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S02_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B04_S57_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S26_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S02_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B06_S34_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B01_S26_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S09_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S22_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B06_S13_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B05_S49_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B02_S14_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B06_S17_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B01_S53_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B04_S48_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S13_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S54_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S15_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B01_S16_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S06_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B01_S10_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B05_S08_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S38_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B05_S37_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B04_S54_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B02_S51_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B02_S60_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M03_B03_S24_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F04_B05_S12_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S51_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F02_B02_S24_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S44_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M02_B01_S52_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M04_B05_S39_R01_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F03_B02_S35_R01_F_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'F01_B05_S29_R02_N_recon.wav></audio></td>
 <td><audio controls><source src='./demo_sample/'M01_B01_S43_R01_N_recon.wav></audio></td>
</tr>
