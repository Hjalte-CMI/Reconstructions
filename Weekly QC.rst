Weekly QC
=========

PET/CT
^^^^^^

PET
----
.. Image:: Images/PETCT_PET.png

1.	 MM emb -> Shutdown (embedded pc) -> Turn off scanner on the back of the gantry -> wait 10 sec. -> turn on scanner.
2.	 Restart  Host computer.
3.	 Mount 38 mm Pallet.
4.	 Put in position 2.
5.	 Tape the fantom (GE-68) to the pallet.
6.	 Open Inveon Acquisition Workplace (IAW).
7.	 Turn on the laser by clicking the 4th icon from the left.
8.	 Use the controlpanel on the scanner to adjust the fantom horizontally and vertically.
9.	 Open the rear shield by clicking on the button at the control panel – check to see if it opens.
10.	 Choose PET on the PET/CT monitor.
11.	 Put in position 3. -> click “center FOV”.
12.  Click on the first icon from the left (PET daily quality control) -> perform QC -> change to current -> start.
13.	 Verify if the result is adequate.
14.	 Place the fantom back in the container – the pallet can be left on.

CT
---
.. Image:: Images/PETCT_CT.png

1.	 click the 2nd icon from the left ( CT calibration panel).
2.	 De-mark all the protocols.
3.	 Mark “Perform source conditioning” and “Evaluate X-ray hardware”.
4.	 Close the rear shield.
5.	 Close the Interlock by gently pushing down until it “clicks”.
6.	 Click Run.
7.	 Verify that the result is satisfying.


Mikro-PET
^^^^^^^^^^
..Image:: Images/MikroPET.png

..Image:: Images/MikroPETGO.png

1.	 Restart computer.
2.	 Restart scanner by flipping the switch at the back and waiting 10 sec. before turning it back on.
3.	 Mount Mikroscan Pallet.
4.	 Tape the fantom to the pallet.
5.	 Open up MicroPET Manager.
6.	 Turn on the laser in Tomograph -> Toggle laser power.
7.	 Click on Motion Control and adjust the fantom horizontally, either with the Manager or at the scanner.
8.	 Press the laser to the left of the fantom and adjust vertically.
9.	 In the Motion Control, click “Center FOV”.
10.	 Close down MicroPET Manager and open MicroPETSSD.
11.	 Click Setup system/Diagnostics-> aquire -> Quick scan.
12.	 After 

.. Image:: Images/MikroPETResult.png


SPECT/CT
^^^^^^^^

**Never restart or shut-down computer or scanner!**

X-ray Run Up
-------------


Before running any scans the X-ray Run Up must be completed.

1.	 Open Nucline nanoscan
2.	 Choose icon 5 from the left (Gantry) -> Click "X-ray Run Up" -> Then start.

The Run Up usually takes around 26 minutes.

Integrated CT Calibration
--------------------------

.. Image:: Images/Integrated_Calibration.png

1.	 Click on the first icon from the left (Worklist).
2.	 Click “QC”.
3.	 Under CT, click “Integrated Calibration”.
4.	 Click the first one, “cleaning support”, click “prepare”, then “GO”.
5.	 When it’s done, repeat the process with “Offset Calibration”. This will trigger the next 4 to run automatically.
6.	 Repeat for “Blank Scan Quality Check” when step 6 is finished running.

HU Calibration
---------------
.. Image:: Images/HU_start.png

1.	 Start by changing to the Mouse pallet M. Click on “Pallet Exchange” -> “start” when the pallet is free to move -> “ok” -> choose “MC Mouse M”
2.	 Refill the fantom with purified water if any air bubbles are present.
3.	 Tape fantom to the pallet
4. 	 click on the first icon from the left, “Worklist” ->click “QC”, then “Hounsfield Quality Check”
5.	 Adjust the frame and take a picture from the side by clicking “prepare”, then “Go”.
6.	 Repeat this with a picture from the top
7.	 Now go to “Hounsfield Quality Check” and adjust the 2 blue boxes so that the vertical axis in the middle aligns with the intersection between the water and air.
8.	 Now click ”Prepare”, then “Run”
9.	 When the scan is completed, check the results with table values to ensure the scanner is working correctly.

.. Image:: Images/HU_BlueBox.png

Dosis Calibrator
^^^^^^^^^^^^^^^^^

.. Image:: Images/Dosis.png

.. Image:: Images/Radioaktive.png 

1.	 Put on gloves.
2.	 Click ”Daily” on the dosis calibrator.
3.	 Follow the instructions given by the calibrator.
4.	 When you get to “Accuracy” insert the CS-137 source into the chamber. CS-137 is in a red metal tube. When done, press the white box to continue.
5.	 When you get to “autoconstancy”, click ”Home” – the calibration is complete.
6.	 Remember to put the CS-137 back into the red metal tube.

Wellcounter
^^^^^^^^^^^

.. Image:: Images/Wellcounter.png

The racks and Iodine 129 needed to run the calibration is below the Wellcounter itself.

1. Place the background- and stop-rack in the Wellcounter and press the run button on the monitor. This will take 5 minutes.

2. Put on gloves, and place the Iodine 129 into the test-rack and into the Wellcounter with a stop-rack next to it. Press run again.

3. Remember to replace the STOP-, Background and test-rack along with the Iodine 129 back into the metal incasing.

4. When the calibration is finished, insert the harddrive into the Wellcounter.

5. Click “Exit” on the monitor followed by “Close the Software”.

6. The Wellcounterdata folder is in the C drive.

7. Copy the entire folder onto the harddrive and remove the harddrive.

8. Insert the harddrive in the laptop out in the scanning room and copy the folder to /N:/LABDATA/CMI-DATA/WellCounter_Data_Current/Backup_Wellcounter/WellcounterData.

9. Remember to replace the harddrive after transfer.

