Technical Batch Reconstruction
===============================

Technical Description
^^^^^^^^^^^^^^^^^^^^^^^
Here you can find a more detailed description of the individual scripts, which reconstruct batches of scans.



submitCTRecon
--------------

The function `submitCTRecon.m` creates a .uPetRecon file which the IAW can use for reconstruction. The functions works the following way:

.. highlight:: matlab

:: 

   % Inputs:
   
   % User       - The name of the user which corresponds to the reconstructions being done           
   % Study      - The Name of the study wishing to be reconstructed
   % Scan       - A .txt file listing the files needed to be reconstructed
   % TMx        - Binary choice. 0 = No TMx wanted, 1 = TMX  or if no TMx is supplied a standard Transformation matrix will be used (sTMx)
   % atnOut     - Binary choice for attenuation map

The function itself has no output but will save the generated .txt file in a folder on the N-drive:

:: 

   % Output
   
   % saves the generated file in the folder 'N:\LABDATA\CMI-DATA\Cardiac_imaging\microQ\submitted\' as a .uPetRecon file.




SubmitPETHisto
--------------



SubmitPETRecon
---------------



Co-registration
----------------

