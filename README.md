# EDC310_Practical-2
# Implementation By: Mohamed Ameen Omar

# EDC

# Practical Assignment 2

## 28 August 2018

Compiled by Herman Myburgh and Alistair Yan


## Scenario

You are to develop a simulation platform^1 for a BPSK communication system over an
additive white Gaussian noise (AWGN) multipath channel.

Use the BPSK simulation platform developed inPractical 1to develop a simulation plat-
form that includes the effect of multipath in the received signal, where the channel impulse
response (CIR) length isL= 3. Determine thekth received symbol by

```
rk=skc 0 +sk− 1 c 1 +sk− 2 c 2 +σGauss(); (1)
```
whereskis thekth transmitted symbol andc={c 0 ,c 1 ,c 2 }is the CIR. Moreover,σis the
noise standard deviation andGauss() is the function used to generate zero mean unity
variance Gaussian random variables.

Use the Viterbi MLSE algorithm and decision feedback equalization (DFE) to develop
two equalizers that can determine the most probable sequence of transmitted symbols.
The length of the transmitted symbol sequence, excluding tail symbols, isN= 300

For this practical you must also compare the effect of a linearly declining CIR to that
of a randomly generated CIR. Use a CIR ofc={ 0. 89 , 0. 42 , 0. 12 }. for the linearly declin-
ing CIR, and generate a random CIR by using the following formula

```
c={
```
```
RNG(σ)
√ 23 ,
RNG(σ)
√ 23 ,
RNG(σ)
√ 23 } (2)
```
where RNG is the normally distributed number generator you created in Practical 1
andσ= 1.

Generate a new CIR for each data block (N = 300) you tranmit. Compare the
effectiveness of DFE to Viterbi for both the linearly declining CIR and the randomly
generated CIR. Report on your findings. Provide a detailed analysis. Be concise and use
proper grammar.

## Deliverables

- Write a report using LATEX. Reports that are not written using LATEXwill not be marked.
- Include your code as an appendix using double columns.

(^1) All software must be developed inP ython.
EDC320 – Practical Assignment 2 1


## Instructions

- All reports must be in PDF format and be named report.pdf
- Place the software in a folder called SOFTWARE and the report in a folder called
    REPORT
- Add the folders to a zip-archive and name it studnrEDC310prac2.zip.
- All reports and simulation software must be e-mailed toedc310.2018@gmail.com no
    later than 28 September 2018. No late submissions will be accepted.
- Submit your hard copy in class or at the Eng III 7-31.

## Additional Instructions

- Do not copy! The copier and the copyee (of software and/or documentation) will receive
    zero for both the software and the documentation. Z-e-r-o.
- For any questions or to make an appointment, email me atu14006007@tuks.co.za
- Make sure that you discuss the results that are obtained. This is a large part of writing
    a technical report

## Marking

Your report will be marked as follows:

- 50% will be awarded for the full implementation of the practical and the subsequent
    results in the report. For partially completed practicals, marks will be awarded as seen
    fit by the marker.
- 50% will be awarded for the overall report. This includes everything from the report
    structure, grammar and discussion of results.

EDC320 – Practical Assignment 2 2


