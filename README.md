# CAP5510 - Programming Assignment

## Group:
- Sudarshan Khasnis
- Sivalaya Gangavarapu
- Sri Hari Chandana Borra

&nbsp;

## Instructions to run the code in command prompt
- All source files are placed in the folder 'src' while the executable files remain in the main directory
- 'inputDNA.fasta' is the input to hw1.py
- Run hw1.exe using the command ```hw1 inputDNA.fasta 5 0.5 outputDNA.fasta```
- The output of hw1.py viz., 'outputDNA.fasta' is used as the input to hw2.py
- Run hw2.exe using the command ```hw2 outputDNA.fasta 20 60 46 outputSeqPart.fasta```
- The output of hw2.py viz., 'outputSeqPart.fasta' is used as the input to hw3.py
- Run hw3.exe using the command ```hw3 outputSeqPart.fasta 1 -1 -2 outputSeqAssemble.fasta```
- 'outputSeqAssemble.fasta' is the final output file that contains the final merged sequence in fasta format

**_NOTE:_** All input files must be in the same folder as the application

&nbsp;

## Tasks
- Sequence generator
  - Reads file in fasta format
  - Generates k-1 sequences closest to the input sequence
  - Mutates each sequence by replacing/deleting nucleotides with pre-computed probabilities
  - Output each mutated sequence along with original in fasta format
  
- Sequence partitioning
   - Reads file in fasta format
   - Creates partitions for sequences generated above
   - Each fragment has a random length within a specified range
   - Each fragment is given a number and outputted in fasta format 
   
- Sequence assembler
   - Reads each fragment from fasta formatted input file
   - Performs dovetail alignment between each fragment and computes the score based on match score and penalties
   - Recursively merges sequences with maximum alignment score
   - Returns the longest fragemnt assembled in fasta formatted output file
