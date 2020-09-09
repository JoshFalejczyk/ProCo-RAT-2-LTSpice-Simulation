# ProCo-RAT-2-LTSpice-Simulation

This is an LTSpice circuit simulation of the ProCo RAT 2, a guitar pedal that produces a wide range of distortion audio effects, from overdrive, to traditional distortion, and to fuzz.  As a guitarist, it is a personal favorite pedal of mine, and as I've gotten more into Audio Signal Processing and circuit design, I chose to simulate it as an intro to LTSpice.  As this was a self-taught project, along much trial and error, I learned about concepts related to general circuit design like feedback loops, low/high-pass filters, op-amp topologies, the inner workings and various types of potentiometers, and AC Analysis.  This also served as an excellent way to learn how to design and import new LTSpice component models, using both the Hierarchal Block and Cell methods.
Included in the repository is the LTSpice schematic (Proco Rat Schematic.asc), a text file where notes on and decisions made related to the circuit's construction can be found (Rat 2 Schematic Notes.txt), and the input WAV file of an electric guitar's E2 note (E-Note-Dry.wav).  In terms of analysis and output, the schematic is currently set to output at the settings of 50% Distortion, 0% Filter, and 50% Volume, which I included an example of (LTSpice D50 F0 V50.wav).  However, for auditory comparison, I've also provided two other WAV files.  One is a sample of the same E2 note ran through the actual ProCo RAT 2 pedal (Real Life D50 F0 V50.wav), and the other makes note of the fact that the LTSpice output is without running through a guitar amplifier and speakers (like the real life sample), and so these variables were further simulated and outputted (Bias Amp D50 F0 V50.wav).  The Audacity DAW and Positive Grid Bias Amp VST was utilized to simulate the guitar amplifier and speakers from the real life sample.  The LTSpice output was inputted to Audacity/Bias Amp, and the "American Bass" amp was selected with Gain at 7, all EQ/Presence controls halfway, and Master Volume at 7.  For the guitar cabinet in Bias Amp, the "1x12 Tweed Lux" and SM57 microphone were selected, with the microphone being placed between the speaker's center and the right side of the speaker cone's rim.  Total effect output in Bias Amp was at about "1:00".  These were the only settings changed, and the rest were kept default.  When comparing the real life output to the Bias Amp output, it is in my personal opinion that while simulated version bears some harshness and noise and is not spot-on to the real thing, it is undeniably close nevertheless.  Finally, AC Analysis on the LTSpice schematic was done, where an octave sweep was performed at 100 points and plotted (ProCo-Rat-2-AC-Frequency-Analysis.png).  It can be compared to the frequency response curve plot of the same ElectroSmash article I based the circuit off of, which is also included (ElectroSmash Frequency Response.png).  It should, however, be noted that ElectroSmash analyzes the original ProCo RAT, while I have analyzed the ProCo RAT 2, which bears some differences (different op-amp and diodes, modified resistors/capacitors for filtering, and so on).  However, the plots are still somewhat similar, which is expected.  All in all, I am very happy with this project, and felt obligated to share it here.

Credit:
1. ElectroSmash.com provided much inspiration, a schematic of the original ProCo Rat which I used as a base, as well as a frequency response curve plot for comparison to my own analysis.
2. Aron Nelson provided an information-filled schematic detailing the ProCo Rat circuit and changes in components over different versions, which I used to convert my ElectroSmash Rat schematic to a Rat 2.
3. All other files and work are of my own.
