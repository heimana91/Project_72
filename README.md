# Project_72

Authors: Heimana Palmer and Sanath Vettivel (University of Auckland).

Note: For a visual platform to run or edit the function block environment then use Microsoft Visual Studio 2013 (as used for this Research Project).

------------------------------------------------------------------------------------------------------------------------------
Bollinger Bands  (Decision Algorithm One)

Step 1: Download Bollinger Bands.zip

Step 2: Extract files

Step 3: Open Command Prompt, Navigate to the "run" file inside Bollinger Bands (Bollinger Bands\blokide_evstation\Generated\Run)

Step 4: Compile using " gcc *.c -o top.exe "

Step 5: Run code using " ./top.exe " or " top.exe "

Step 6: Results can be found in the "run" folder called "Results.csv"

Note: Kalpesh Chaudhari is a Ph.D. student who worked on the use of the Bollinger Bands for ESS mode of operation selection.

His Matlab code, which uses hardcoded mode of operation selection, is attached. Changes were made to ensure energy demanded at the charging station was always met by energy supplied by the grid and/or energy storage system.

We matched the results of his related work using the IEC-61499 Function Blocks Standard.

Our Function Block implementation which matches the results of his Matlab algorithm is located inside the Bollinger Bands project. This was to verify our function block environment worked.

All that is needed is to "swap the Basic Function Block (BFB) called "bfb_off_peak_types" within the Composite Function Block (CFB) called "cfb_controller.cfb" with seven other BFB called "bfb_(XXdayHereXX)_classifier.fb"(i.e. bfb_sat_classifier) then make sure it is connected to the needed ports from the CFB to the BFB called "bfb_controller_um"

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
