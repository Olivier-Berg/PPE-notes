#logics 
A)
1. $$\begin{array} {r|r} A & A \rightarrow A \\ \hline T & T\;\textbf{T}\;T \\ F & F\;\textbf{T}\;F \end{array}$$
2. $$\begin{array} {r|r} C & C \rightarrow \neg C \\ \hline T & T\;\textbf{F}\;F\;T \\ F & F\;\textbf{T}\;T\;F \end{array}$$
3. 

| A   | B   | $(A \leftrightarrow B) \leftrightarrow \neg (A \leftrightarrow \neg B)$ |
| --- | --- | ----------------------------------------------------------------------- |
| T   | T   | TTT**T**TTFFT                                                           |
| T   | F   | TFF**T**FTTTF                                                           |
| F   | T   | FFT**T**FFTFT                                                           |
| F   | F   | FTF**T**TFFTF                                                           |
![Documentscans](Answers%20Forallx%2040-41.pdf)

---
A)
Tautologies: 1, 3, 5, 6, 8
Contradiction: 7
neither: 2, 4, 9

![Documentscans 2](Answers%20Forallx%2046.pdf)

D)
1. Then whenever A is true, B is also true. And whenever A is false, B is also false. Therefore $A \leftrightarrow B$ is always true.
2. ![IMG_2645](Answer%20Forallx%2046%20D2.png)
	Whenever $(A \land B) \rightarrow C$ is True (the first one), then A, B and C are also true. So therefore $A, B \models C$ is correct. See also, TLM page 43.
3. There has to be a case where it is false, because they are tautologically inconsistent, they cannot always all be true. 
4. It is correct, anything follows from a contradiction, there is no case where all the premisses are true and the conclusion is false.
5. It is correct, there is no case where all the premisses are true and the conclusion is false.
6. It can be both true and false, whenever both A and B are true, $A \lor B$ is true, whenever both A and B are false, $A \lor B$ is false.
7. The same, there could still be a case where A and B are both false.

E)
Yes, because they have the same truth table.

---

**ASK WHETHER CHECKING FOR INCONSISTENCY ONLY REQUIRES A PARTIAL TRUTH TABLE**
**SAME GOES FOR EVERY OTHER ONE (example: C4, B3, A6)**
TLM: *"An argument is valid iff it does not have a counterexample."*, see also: page 44-45 TLM
![Answers Forallx 49-52](Answers%20Forallx%2049-52.pdf)
