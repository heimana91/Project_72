# Project_72

Important note
For a visual platform to run or edit the function block then use Microsoft Visual Studio 2013.


Bollinger Bands 

Step 1: Download Bollinger Bands.7z
Step 2: Unzipped 
Step 3: Open Command prompt Navigate to the "run" file inside Bollinger Bands 
Step 4: Compile it using " gcc *.c -o top.exe "
Step 5: Run the code using " ./top.exe " or " top.exe "
Step 6: the Data is in the "run" folder called "Results.csv"

Note: Kalpesh is a PHD student who worked on the use of the Bollinger Bands for ESS mode of operation selection.

His Matlab code, which uses hardcoded mode of operation selection, is attached. Changes were made to ensure energy demanded at the 
charging station was always met by energy supplied by the grid and/or energy storage system.

We matched the related work that he has done using the IEC-61499 Function Blocks Standard.

Our Function Block implementation which matches the results of his Matlab algorithm 
is located inside the Bollinger Bands project. This was to verify our function block environment worked.

All that is needed is to "swap the Basic Function Block called
"bfb_off_peak_types" within the Composite FB called "cfb_controller.cfb"
with seven other Basic FB called "bfb_(whatever day)_classifier.fb"(i.e. bfb_sat_classifier) then make
sure it is connected to the needed information from the CFB to the BFB called "bfb_controller_um"


Box & Whisker

Step 1: Download Box and Whisker.7z
Step 2: Unzipped 
Step 3: Open Command prompt Navigate to the "run" file inside Box and Whisker
Step 4: Compile it using " gcc *.c -o top.exe "
Step 5: Run the code using " ./top.exe " or " top.exe "
Step 6: the Data is in the "run" folder called "Results.csv"

Artificial Neural Network

Important note when working with Microsoft Studio if the Neural Network is re-generated then 
include this following library #include "../run_ann.h" in the file called "BasicFunctionBlock1.c" in the run folder

Step 1: Download Neural Network.7z
Step 2: Unzipped
Step 3: Open Command prompt and Navigate to the "run" file inside Neural Network
Step 4: Compile it using " gcc *.c ../*c ../libfixmath/*.c -o top.exe "
Step 5: Run the code using " ./top.exe " or " top.exe "
Step 6: the Data is in the "run" folder called "Results.csv"
