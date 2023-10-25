---
title:  ENS210 - Computational Biology
author: Ogun Adebali
geometry: margin=2cm
---


# Lab 3

**Deadline:** You need to submit (push) your task by the end of lab hours.

## Introduction to Python

* Please write your code to given spaces in `answers.py`.
* Commit after each task.
* You only need to commit `answers.py` and `quizanswers.jpeg`.
* If you do not answer the questions as stated in the answers of the quiz, 25% of the grade for the question will be deducted even if the answer is correct.
* Submit (`git push`) by the end of lab session.
* You don't need to do anything to `test.py` file, it's only there for grading purposes. (However, you can manually check your answers by running `pytest test.py`)
* Your script will be checked with Python3. Make sure that your code is compatible with Python3 syntax. (If your code fails to run, you will get -2 points)
* You will use the given DNA sequence to test the functions you will write.

### Task #1 (1pts)
* Write a function converting DNA to RNA. T -> U

```
def DNAtoRNA(inputDNA):
    '''Converts DNA string to RNA by changing Thymines to Uracils'''
```

### Task #2 (3 pts)

* Write a function returning percentages of four nucleotides (A, C, T, G) of given DNA.
(Percentages only contain two decimal points. i.e: 20.33, NOT 20.3276)

```
def getNucleotidePercentages(inputDNA):
    '''Returns a dictionary containing Nuclotide percentages. The keys of the output dictionary must be written EXACTLY as 'A', 'C', 'T' and 'G' '''
```
* Write a function that counts purine and pyrimidine bases in that DNA sequence. 

```
def count_Pur_Pyr(inputDNA):
    '''Returns a dictionary containing the number of purine and pyrimidine bases. The keys of the output dictionary must be written EXACTLY as 'Number of purine bases' and 'Number of pyrimidine bases' '''
```
### Task #3 (2 pts)

* Write a function returning complementary strand of given DNA.

```
def getComplementaryDNA(inputDNA):
    '''Returns complementary strand of a given DNA'''
```

### Task #4 (1 pts)

* Write a function returning reverse complementary strand of given DNA by using the function that you wrote in `Task #3`.

```
def getReverseComplementaryDNA(inputDNA):
    complementaryDNA = getComplementaryDNA(inputDNA)
    '''Returns reverse complementary strand of a given DNA'''
```

### Task #5 (3 pts)

* Transcription factors bind certain DNA elements with their DNA binding domains and regulate gene expression. Many of the DNA motifs are known and publicly available now. One of the most known motif is TATA-box, which is recognized by the TBP (TATA-Box Binding Protein) and crucial for transcription to start. The consensus motif of TATA-box is  5'-TATA(A/T)A(A/T)-3'. Please do not forget that opposite strand of the DNA also may include these motifs too. 

In light of the knowledge that the inputDNA sequence is assumed to be in the 5' -> 3' direction, write a function that counts the occurrences of the probable motifs. 

```
def find_motifs(inputDNA):
    '''Returns just the number of the occurence of the motif at a given DNA sequence.'''
```


