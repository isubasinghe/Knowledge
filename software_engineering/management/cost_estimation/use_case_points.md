# Use case points (UCP)

## Basic idea

A FP-style sizing technique driven by use cases instead of requirements specs. Sums weighted use-case counts and actor counts, then scales by technical and environmental complexity factors. Developed in 1993 for OO methodology.

## Key formulas

- $UCP = (UUCW + UAW) \times TCF \times ECF$
- $UUCW = 5 N_s + 10 N_a + 15 N_c$ (simple / avg / complex use cases)
- $UAW  = 1 N_s + 2 N_a + 3 N_c$ (simple / avg / complex actors)
- $TCF = 0.6 + 0.01 \sum w_i F_i$ (13 technical factors)
- $ECF = 1.4 - 0.03 \sum w_i F_i$ (8 environmental factors)

Is a software estimation technique used the measure the software size with Use cases Developed in 1993 for sizing and estimating projects using OO methodology The concept of UCP is similar to FP

Use cases describe the functionality of the system Use cases model the dialog between the actors and the system Primary purpose is to document functional requirements but also used for testing purposes

1. Compute unadjusted use case weight (UUCW)
2. Compute unadjusted actor weight (UAW)
3. Compute technical complexity factor (TCF)
4. Compute environmental complexity factor (ECF)
5. Compute the final size estimate

## Compute UUCW

Count the number of simple, average, complex use cases based on the number of transactions as per table below.

| Use case classification | Type of actor       | Weight |
| :---------------------: | ------------------- | ------ |
|          Simple         | 1 to 3 transactions | 5      |
|         Average         | 4 to 7              | 10     |
|         Complex         | 8 or more           | 15     |

UUCW = N\_s _5 + N\_a_ 10 + N\_c \* 15

## Compute UAW

Count the number of simple, average, complex actors

| Actor classification | Type of Actor                                        | Weight |
| :------------------: | ---------------------------------------------------- | ------ |
|        Simple        | External system interacting using a well defined API | 1      |
|        Average       | External system using a standard protocol            | 2      |
|        Complex       | Human actor using GUI                                | 3      |

UAW = N\_s _1 + N\_a_ 2 + N\_c \* 3

## Compute TCF

![TCF](<../../../.gitbook/assets/tcf (2) (2).png>)

## Compute ECF

![ECF](<../../../.gitbook/assets/ecf (2) (2).png>)

## Compute final UCP

UCP = (UUCW + UAW) _TCF_ ECF

## Advantages of UCP

* UCP are based on use cases and can be measured very early in the project life cycle
* UCP based estimates are found to be close to actuals when estimation is performed by experienced people
* UCPs are easy to use and do not call for additional analysis
* Use cases are being used vastly as a method of choice to describe requirements

## Disadvantages of UCP

* UCP can be used only when requirements are written in the form of use cases
* Dependant on goal oriented, well written use cases
* Technical and environmental factors have high impact on UCP
* Not as well established as FPs
