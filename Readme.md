# Entropy Penalised - Semi Definite Programming

This project implements a numerical method to approximately solve the Max-Cut program (an NP-hard graph problem)

Max Cut : split graph nodes into two groups so that number of edges crossing between the groups in maximized.

This model is published in 2019 (attached above)

More clear explanation is attached in the code files. 

## Flow of solving : 

Rank 1 solution (NP Hard) -> Semi Definite Programming -> Entropy penalised SDP

we are relaxing a hard constraint to high rank then adding entropy to it to get better solving time. 

Entropy Function : Tsalli's entropy

We convert the result matrix back to 0, 1 using Goemans - Williamson rounding.

## Run: 

```python
python max_cut_epsdp.py
```
