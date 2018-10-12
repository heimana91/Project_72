# Project_72

Authors: Heimana Palmer and Sanath Vettivel 
The University of Auckland.

>This repository contains the entirety of our research project compendium. It's contents are:

>Bollinger Bands.zip (Code for this decision algorithm discussed in our research reports)

>Box and Whisker.zip (Code for this decision algorithm discussed in our research reports)

>MATLAB Algorithm and Excel Results.zip (Kalpesh's MATLAB algorithm after we had made our modifications. Also results from the three
decision algorithms and the excel template used to calculate charging station costs. See formatingResultsREADME.txt inside.

>Neural Network.zip (Code for this decision algorithm discussed in our research reports)

>Poster-72-2.pdf (Project Exhibition Poster)

>seminar.pptx (Project Seminar Slides)

------------------------------------------------------------------------------------------------------------------------------

Note: For a visual platform to run or edit the function block environment then use Microsoft Visual Studio 2013 (as used for this Research Project). The rest of this README describes how to use the decision algorithms.

Note: Kalpesh Chaudhari is a Ph.D. student who worked on the use of the Bollinger Bands for ESS mode of operation selection.

His Matlab code, which uses hardcoded mode of operation selection, is attached. 

------------------------------------------------------------------------------------------------------------------------------
MATLAB Algorithm 

Changes were made to ensure energy demanded at the charging station were always met by energy supplied by the grid and/or energy storage system.

Commenting was added by us to allow someone to understand the basic concepts.

We matched the results of his related work using the IEC-61499 Function Blocks Standard.

Our Function Block implementation which matches the results of his Matlab algorithm is located inside the Bollinger Bands project. This was to verify our function block environment worked.

All that is needed is to "swap the Basic Function Block (BFB) called "bfb_off_peak_types" within the Composite Function Block (CFB) called "cfb_controller.cfb" with seven other BFB called "bfb_(XXdayHereXX)_classifier.fb"(i.e. bfb_sat_classifier) then make sure it is connected to the needed ports from the CFB to the BFB called "bfb_controller_um"

------------------------------------------------------------------------------------------------------------------------------
Bollinger Bands  (Decision Algorithm One)

Step 1: Download Bollinger Bands.zip

Step 2: Extract files

Step 3: Open Command Prompt, Navigate to the "run" file inside Bollinger Bands (Bollinger Bands\blokide_evstation\Generated\Run)

Step 4: Compile using " gcc *.c -o top.exe "

Step 5: Run code using " ./top.exe " or " top.exe "

Step 6: Results can be found in the "run" folder called "Results.csv"


------------------------------------------------------------------------------------------------------------------------------

Box & Whisker (Decision Algorithm Two)

Step 1: Download Box and Whisker.zip

Step 2: Extract Files

Step 3: Open Command Prompt, Navigate to the "run" file inside Box and Whisker (Box and Whisker\blokide_evstation\Generated\Run).

Step 4: Compile using " gcc *.c -o top.exe "

Step 5: Run code using " ./top.exe " or " top.exe "

Step 6: Results can be found in the "run" folder called "Results.csv"

------------------------------------------------------------------------------------------------------------------------------

Artificial Neural Network (Decision Algorithm Three)

Note: when working with Microsoft Studio if the Neural Network is re-compiled then 
include this following library #include "../run_ann.h" in the file called "BasicFunctionBlock1.c" in the run folder (Neural Network\blokide_evstation\Generated\Run)

Step 1: Download Neural Network.zip

Step 2: Extract Files

Step 3: Open Command prompt and Navigate to the "run" file inside Neural Network (Neural Network\blokide_evstation\Generated\Run)

Step 4: Compile using " gcc *.c ../*c ../libfixmath/*.c -o top.exe "

Step 5: Run code using " ./top.exe " or " top.exe "

Step 6: Results can be found in the "run" folder called "Results.csv"

------------------------------------------------------------------------------------------------------------------------------
