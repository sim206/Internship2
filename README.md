<h1>Designing a tensile benchtop test in collaboration with Residual stress measurement with the laser ultrasonic method</h1>

<h2>Description</h2>
In this paper, the design of a small-scale hydraulic tensile benchtop test rig in collaboration with residual stress measurement using the laser ultrasonic method was discussed. Two designs were proposed: Design 1, a standard mechanical rig, and Design 2, a hydraulic rig. The cost and materials for each design were provided.

Based on the discussion and analysis, it was determined that Design 2, the hydraulic rig, was a more suitable and simplified option for the experimental setup. However, further modifications and improvements are needed to account for the weight of adjustable plates and potential bending forces. Finite element analysis can be conducted to evaluate the effects and optimize the rig design.

An initial lab trial was conducted using the laser ultrasonic method to measure residual stress. The experimental setup and methodology were described, and the results showed a decrease in longitudinal and shear wave velocities as the load was applied to the sample. The results supported the detectability of residual stress using the laser ultrasonic method.

Future work should focus on refining the rig design, conducting further experiments with different materials and stress levels, and validating the results through comparison with other established residual stress measurement methods. Additionally, efforts can be made to automate the data analysis process using advanced algorithms and software tools.

Overall, the combination of the hydraulic tensile benchtop test rig and laser ultrasonic method for residual stress measurement holds great potential for evaluating the structural integrity of materials and components. It can contribute to improved design processes and better understanding of the effects of residual stress on material behavior..
<br />


<h2>Languages and Utilities Used</h2>

- <b>SolidWorks</b> 
- <b>Excel (Bill of Materials)</b>
- <b>Matlab</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Project walk-through:</h2>

**1. Initial Lab Trial**

The following application of ultrasound is a non-destructive method for measuring residual stress.

<p align="center">
<img src="https://i.imgur.com/SI6xZYD.png" alt="Internship"/>
<br/>
</p>

**2. Experimental setup and scan**

- The experiment used a clamp to apply a maximum load of 25kN on an Aluminum alloy sample.
- The clamp was mounted on a pneumatic table, and optical lenses were adjusted accordingly.
- A Quentel laser operating at 30% power with a 0.5mm pitch was used.
- Data capture involved 100 elements for pre-load and post-load of Aluminum samples 3 and 4.
- Aluminum sample 3 was inserted into the clamp without any load applied.
- A line source laser was focused on the samples, and scans were taken (Figures 8, 9, and 10).


<p align="center">
<img src="https://i.imgur.com/Yn0dyUE.png" alt="Internship"/>
<br/>
</p>

<p align="center">
<img src="https://i.imgur.com/efahE1L.png" alt="Internship"/>
<br/>
</p>

**3. Methodology**

- A MATLAB script was developed to calculate longitudinal and shear wave arrival times and velocities for both pre-loaded and loaded samples.
- The script used sample thickness, pre-load and post-load information, and waveform arrival times.
- Waveform velocities were plotted for each point, representing shear and longitudinal waves.
- Figures 11(a) and 12(a) show wave velocities plotted against element positions in "B scans - No load" and "B scans - load" images.
- Figures 11(b) and 12(b) include noise in the velocity versus element position plots.
- Polynomial curve fitting was applied to the wave points, omitting noise, and the maximum velocity was determined using peak finding.
- The third MATLAB script compared the best-fit lines for longitudinal and shear waves in the samples, plotted in Figure 13.

According to literature, a conventional aluminium alloy has a longitudinal velocity of 6320(m/s) and a shear velocity of 3130(m/s). This is calculated from the speed of sound of a material, thus longitudinal waves travel approximately twice as fast as shear waves.

**4. Results**

<p align="center">
<img src="https://i.imgur.com/LZHYpCz.png" alt="Internship"/>
<br/>
</p>


<p align="center">
<img src="https://i.imgur.com/1bCVVFD.png" alt="Internship"/>
<br/>
</p>


<p align="center">
<img src="https://i.imgur.com/rKz0UCY.png" alt="Internship"/>
<br/>
</p>

**5. Discussion and Conclusion**

The developed MATLAB scripts accurately calculated wave velocities and compared best fit lines for longitudinal and shear waves. The results demonstrated a decrease in velocities as load was applied, confirming the detectability of residual stress using the laser ultrasonic method. However, assumptions and limitations in the experiment led to a conservative approach and the possibility of sample expansion in the middle of the loaded specimen. To address this, a tensile machine with specified standards and a non-linear analysis using finite element analysis are recommended. The tested tensile benchtop rig designs offer a cost-effective solution for in-situ residual stress monitoring with potential for further development. It is advised to repeat the experiment for result validation and consider attaching digital callipers and data logging with an Arduino to account for gradual sample expansion.
