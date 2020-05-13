# ventaid
## *An Open Source Ventilator Aid Project*

VentAid is meant to assist in Ventilation of the Patients who are in need of such attention where Proper Medical Ventilators are busy in Supporting Patients with more Critical Condition & will be available later but not immediately. VentAid desires to act as a ‘Stop Gap’ Arrangement made with Readily Available Modules/Components. That’s it’s Sole Purpose. It’s not & won’t ever be the Replacement of a A Proper Medical Ventilator.

## Goal:
- Low Cost
- Easy to Manufacture/Assemble (very short Turn Around Time)
- Very Basic in Nature (but with Provision of Future
Expansion   using Modules)
- Manual Mechanical Inlet Air Pressure Control
- Flow Control (Inhalation/Exhalation Timing Control)
- Repetition Rate (Breathing Rate) Control
- Safe (built-in Alarm System)

## Limitation:
- Not Ready for Intensive Care Use
- Patient Flow Pattern can’t be Programmed
- No Backup Power (but System Failure Alarm using Battery Power can be added.)
- Uses Pressurized Air/O2 Supply available in Most of the Modern Hospitals, thus does not have own Air/O2 Source (can be used with any other Pressurized Air Source including Air Compressor though.)

E-Vent by M.I.T. Team is One of the Best Open Source ‘Proper’ Ventilators available at Present & should be the Preferable Option if Need arises. However the Device Presented here tries to solve the Problem from Different Angle with Minimum Sustainable Functionality & not Directly Comparable with E-Vent or any such Efforts.

VenAid Consists of 2 sub-systems; Mechanical (the Breathing Circuit) & Electrical (the Controller, uses a Pair of Famous & Cheap 555). Breathing circuit is primarily responsible for delivering the compressed air supply to the patient but it’s under the supervision of the controller for timing & monitoring purpose. VentAid is pressure (Positive Pressure) controlled mechanical ventilator (P.C.V.) in nature.

VentAid can be Built from Scratch or Readily Available 555 based P.W.M. & Timer Modules can be Modified to meet VentAid's Purpose.

## Key Specification:

- Breaths per Minute (B.P.M.): Min. ~5 to Max. ~15 (Continuously Variable)
- Inhalation to Exhalation Ratio (I:E): Min. ~1:1 to *Max.*
- Fault Indication/Detection:
	- Controller O/P Stuck at ‘High’ (Inhalation Cycle)
	- Required Air Pressure not available in Breathing Circuit
- Alarm: Visual Indication via L.E.D. but a Small Piezo Buzzer can be used in Place of L.E.D. for Auditory Indication
- Power Supply: 9V (can be Battery Powered)

## Possible Improvements:

- Edge Triggered Alarm (for detecting both ‘Stuck High’ & ‘Stuck Low’ O/P Condition of the Controller)
- Self Latching Alarm (Alarm won’t Reset itself once Triggered)
- Duty Cycle Control using Pin 5 (CONT) of 555
- Delivery of Certain Volume of Air/O2 by Pulse Width Modulated control of the Solenoid Valves (within it’s Mechanical Operating Bandwidth) with the help of a ‘Flow Sensor’ in Breathing Circuit (& Comparator & other Necessary Electronics).

VentAid's Design is no where near Perfect but should be able to do the Basic Job of A Mechanical Ventilator when needed.

VentAid is an Independent Effort. If this Design has something Good in it; you’re Free to use it as it is or may use it in your own Design, if there’s something Horribly Wrong, Probably that’s due to me & you’re Free to make the Necessary Correction (& let me know if Possible.). Doucuments Provided here are not Completely Error Free & will be Corrected/Updated in Later Relese.

Prototype System Building & Characterization is under Progress as of May, 2020. Updates will be Notified here.

This was A Brief Introduction to VentAid. Please refer Documentation Provided for Further Details.

#### Current Release: Rev. 1.0 *(as of May, 2020)*

### Directory Organization:
- docs: VentAid Design Document (in pdf)
- ltspice: LTSpice related Files (.asc, .bom & .net)
- schematics: Controller/Alarm Unit Schematic (in png)

### Tools/Software Used:
- Dell Latitude E6330 (my Primary Driver)
- Ubuntu 16.04
- WPS Office (for Documentation)
- Joplin (as Markdown Editor)
- git (for Version Control)
- VirtualBox (for running Windows 10 VM)
- LTSpice (on Windows 10 VM, for Design & Simulation of the Elctronics)
- Lots of Coffee!

### Reference:
- https://www.e-vent.mit.edu/
- https://www.youtube.com/watch?v=oqRgISFuE0k&t=459s
- https://accessmedicine.mhmedical.com/content.aspx?bookid=520&sectionid=41692239%20
- https://f1000research.com/articles/9-218
- https://www.hackster.io/news/open-source-ventilator-openlung-projects-aim-to-address-the-covid-19-ventilator-shortfall-c7a5ee2f8e58
- NA/NE/SA/SE 555 Datasheet from TI

& Departing Note at Last. My Country (India) is going through Nation Wide Lockdown due to COVID-19 Outbreak at Present (May, 2020) & I’m away from my Lab. & I'm really Missing Her (& Her Rb Standard., & Her Voltage Standard., &... Sorry, I was just getting carried away.).

Stay Safe, Stay Informed & Stay Innovative.
