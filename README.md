# CAP5510 - Programming Assignment

## Group:
- Sudarshan Khasnis
- Sivalaya Gangavarapu
- Sri Hari Chandana Borra

## Instructions to run the code

## Tasks
- Sequence generator
  - Generates k-1 sequences closest to the input sequence
  - Mutates each sequence by replacing/deleting nucleotides with pre-computed probabilities
  
- Sequence partitioning
   - Creates partitions for sequences generated above
   - Each fragment has a random length within a specified range
   
- Sequence assembler
   - Performs dovetail alignment on two fragments and computes the score based on match score and penalties
   - Recursively merges sequences with maximum alignment score
   - Returns the longest fragemnt assembled
