# Design of High Speed Duty Cycle Corrector with 28 nm technology

## Table of Contents

- Abstract 
- Introduction
- Reference Circuit Design
- Expected waveform
- Circuit implementation of DCD
- Circuit implementation of Buffer
- Circuit implementation of DCA
- Simulation Results and Observations
- Observation and Conclusion
- Author
- Acknowledgements
- References
## Abstract
High Speed Duty Cycle Corrector (DCC) is
implemented with 28nm technology using MOSFETS. The
proposed duty cycle corrector is 50% correction format. The
range for the correction of the DCC lies between 20% to 80% of
the signal. Duty cycle corrector (DCC) locks the edge rates of the
signal to achieve the 50% duty cycle and avoid detection error in
clock signal for DDR reception. The High voltage level
corresponds to “1” and low to “0” respectively. For detecting the
voltage level AC coupled circuit or DC coupled circuit with
reference level are used. Its application varies from DDR
synchronous DRAM, Double sampling ADC and many more
with collaboration with Phase lock loops



## Introduction
Circuit being proposed in this paper consists of three major
components Duty cycle adjuster (DCA) buffered with Duty
cycle Detector (DCC).</br>

</br>
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/155891764-91fec4b1-6dc4-4238-af28-0ab5c1a4151f.png">
</p>
<p align="center">
Block diagram of the proposed circuit is
</p>


## Reference Circuit Design
- Duty Cycle Adjuster(DCA)</br>
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/155891857-50f9a78f-bfb5-41b3-b059-502c01ad1c0d.png">
</p>

- Buffer</br>
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/155891921-d5d1b5bb-bb6f-495e-8a3f-d87a0008fbab.png">
</p>

- Duty Cycle Detector( DCD)
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/155891962-a87b0441-cba7-416e-ae93-b9d0aca89d2b.png">
</p>

- Duty Cycle Corrector (DCC)</br>

<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/155892002-1e3623a1-0b2c-4766-ae21-62f97686010c.png">
</p>




## Circuit implementation of DCA.
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156123112-789b0da2-2559-439e-b673-d189e7744979.png">
</p>


## Circuit implementation of Buffer.
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156123294-b889795e-d15a-4dd5-a9ac-cad9b0215467.png">
</p>


## Circuit implementation of DCD.

<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156123459-df0a7c6b-432d-4a60-9749-556dab73402b.png">
</p>

## Circuit implementation of DCC.

<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156123597-db0b94bf-98bf-453a-bd06-a1b9d1c43d82.png">
</p></br>

## Simulation Results and Observations.


- CASE1</br>
DCC functionality is observed here . Waveform justifies that the 30% distortion in input waveform is  corrected by 46% at the output outwaveform. it has been verifed by the measurement tool.

<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156124066-437cc16c-6d56-409e-a323-9f16c4a72e1b.png">
  <img src="https://user-images.githubusercontent.com/100523474/156124170-ed9a35f4-f2fb-41ab-b8b0-c30cba1473fd.png">
</p></br>

- CASE2</br>
DCC functionality is observed here . Waveform justifies that the 30% distortion in input waveform is  corrected by 48% at the output outwaveform. it has been verifed by the measurement tool.
<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156124421-efc980b2-93d2-4065-b15f-7429974855e3.png">
  <img src="https://user-images.githubusercontent.com/100523474/156124494-7ffb47f3-58ff-4e75-9bcb-1b253a108f05.png">
</p></br>

- CASE3</br>
- DCC functionality is observed here . Waveform justifies that the 30% distortion in input waveform is  corrected by 50% at the output outwaveform. it has been verifed by the measurement tool.

<p align="center">
<img src="https://user-images.githubusercontent.com/100523474/156124611-a3b171af-5cd9-44f6-a15b-01256f470686.png">
  <img src="https://user-images.githubusercontent.com/100523474/156124675-c09c85f9-14da-4a9c-a956-c8d62d1a2f35.png">
</p></br>


## Observation and Conclusion
By increasing the width of the nmos and pmos it is correcting the duty cycle more efficiently with the cost of power and leakage.</br>
This duty cycle correction has the tendency to correct 30% to 70% distortion in the input  to almost 50% at the output. </br>
</br>
This Duty cycle Corrector circuit has been implemented with DCA, Buffer, DCD cascaded together with 28 nm cmos technology. 




## Author
Priyanka Tiwari, BTech., Govt. Engg. college Raipur (Department of electronics Engineering)



## Acknowledgements

- [Kunal Ghosh, Co-founder, VSD Corp. Pvt Ltd.](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3B0xcWjpLDThSEo6S9UPO9Tw%3D%3D)
- Chinmaya Panda, IIT Hyderabad
- [Synopsis Team/Company](synopsys.com/company/contact-synopsys/office-locations/india/about-synopsys-india.html)
- [IIT Hyderabad](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- Active and vibrant hackathon community

## References
[1] S. M. Metev and V. P. Veiko, Laser Assisted Microtechnology, 2nd 
ed., R. M. Osgood, Jr., Ed. Berlin, Germany: Springer-Verlag, 1998.
[2] J. Breckling, Ed., The Analysis of Directional Time Series: 
Applications to Wind Speed and Direction, ser. Lecture Notes in 
Statistics. Berlin, Germany: Springer, 1989, vol. 61.o-RF converter,” 
U.S. Patent 5 668
[3] Chien Yu Lin and Heng Shou Hsu, Design of high frequency DCC
with 20-80% correction range
[4] Y.min.c.jiong ,DCC, with DDR DRAM.


