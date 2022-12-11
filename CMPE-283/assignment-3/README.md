# Assignment 3
 

* 2. Explain the process on a high level?
* Go to the same GCP instance created for assignment-2

* Modify the cpuid.c file for the below leaf nodes
  * Write the code to print the exits and cycles under an if condition for %eax=0x4FFFFFFE and 0x4FFFFFFF
* Write the test code and run in it virtual environment
* verify the outputs

* 3. Comment on the frequency of exits – does the number of exits increase at a stable rate? Or are there 
more exits performed during certain VM operations? Approximately how many exits does a full VM 
boot entail?

       No, the number of exits do not increase in a stable rate. Some of the exits increase, while the others stay same. The increment depends on the exit type. Approximately 1037272 exits.
    
* 4. Of the exit types defined in the SDM, which are the most frequent? Least?
  * EXIT_REASON_EPT_VIOLATION(48),EXIT_REASON_MSR_READ(31) happens the most frequent.
  * EXIT_REASON_DR_ACCESS(29),EXIT_REASON_EPT_VIOLATION(48) are least frequently occuring.
