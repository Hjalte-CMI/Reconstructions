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

   % User       - The scientist name as written in the folder name on the LABDATA drive, eg. 'Simon'.
   % Study      - The Name of the study wishing to be reconstructed
   % Scan       - A .txt file listing the files needed to be reconstructed
   % TMx        - Binary choice. 0 = No TMx wanted, 1 = TMX  or if no TMx is supplied
   %               a standard Transformation matrix will be used (sTMx)
   % atnOut     - Binary choice for attenuation map

The function itself has no output but will save the generated .uPetRecon file in a folder on the N-drive:

::

   % Output

   %            - saves the generated file in the folder 'N:\LABDATA\CMI-DATA\Cardiac_imaging\microQ\submitted\'
   %             as a .uPetRecon file.

Further description can be found in the function itself which is commented.



SubmitPETHisto
--------------

submitPETHisto is a function which creates a .uPetHist file which the IAW can use to make the histogram.

::

    % Inputs:

    % User      - The scientist name as written in the folder name on the LABDATA drive, eg. 'Simon'.
    % study     - The study name corresponding to the folder name in which the scans lie
    % scan      - The folder name of the indiviual scan
    % timing    - a string of numbers containing the time indexes for the reconstructions ...
    %            as per Siemens convention. Example '[1,45,1,350,1,120].
    %           To get a gated sinogram, use number of bins and a 'B', eg. '8B'.
    %           Less than 4 frames is considered 'static', and 4 or more frames yields ...
    %           a 'dynamic' sinogram.

The function itself has no output but will save the generated .uPetHist file in a folder on the N-drive:

::

    % Output

    % Generate a .UPetHist file in the folder 'N:\LABDATA\CMI-DATA\Cardiac_imaging\microQ\submitted\'

The dynamic sinogram will take much longer to reconstruct than a static image.


SubmitPETRecon
---------------

SubmitPETRecon is the final function of the reconstruction. It creates a text file, with which the IAW can make a reconstructed PET image.

::

    % INPUTS
    %   user:           The scientist name as written in the folder name on the LABDATA drive, eg. 'Simon'.
    %   study:          The study name corresponding to the folder name in which the scans lie
    %   scan:           The folder name of the indiviual scan
    %   scan_type:      Can be GAT (gated) or UNG (ungated)
    %   frames:         Either a vector for one image or amount of bins for "GAT", e.g.
    %                    '8B' for eight bins
    %   use_atten:      Choose whether attenuation map should be used (0 or 1)
    %   make_scatter:   Whether scatter correction should be used (0 or 1)
    %   resolution:     Number of pixels in the x and y directions, eg. 128

This function, just like the others, don't have an output but will save the file in a folder on the N-drive

::

    % Output

    % Generate a file in the folder 'N:\LABDATA\CMI-DATA\Cardiac_imaging\microQ\submitted\'




Co-registration
----------------

This feature is currently not working, but the idea is that the script will generate the TMx by itself, instead of the current solution where it is
generated scan by scan.
