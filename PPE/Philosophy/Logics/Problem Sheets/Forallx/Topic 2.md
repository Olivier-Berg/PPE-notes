#logics 
a)

1. ¬M

2. (M v ¬M)

3. ((C v G )^¬(C ^ G)) (but they cannot be both, it cannot be both a gorilla and a chimpansee at the same time)

4. -(C v G)

5. (C -> -(M v G))

6. (M v (C v G))

b)

1. (A v E)

2. (A -> C)

3. (E -> -C)

4. (B v D)

5. (C -> D)

6. (F -> C)

7. (-F -> (C v B))

8. (A <-> -E)

9. (D v E)

10. (A -> F)

11. (C -> -B)

12. D

C)

1. (E1 ^ E2)
2. (F1 -> S1)
3. (F1 v E1)
4. (E2 ^ -S2)
5. $\neg(E_1\lor E_2)$
6. $((E_1 \land E_2) \land \neg (S_1 \lor S_2))$
7. $(S_2 \implies F_2)$
8. $(\neg E_1 \implies \neg E_2)\land(E_1 \implies E_2)$
9. $(S_1 \iff \neg S_2)$
10. $((E_2 \land F_2) \implies S_2)$
11. $\neg (E_2 \land F_2)$
12. $((F_1 \land F_2) \iff \neg (E_1 \lor E_2))$

D)

S1 = Alice is a spy
S2 = Bob is a spy
C = The code has been broken
G = German embassy will be in uproar
1. $(S_1 \land S_2)$
2. $((S_1 \lor S_2) \implies C)$
3. $(\neg (S_1 \lor S_2) \implies \neg C)$
4. $(G \lor C)$
5. $((C \lor \neg C) \land G)$
6. $((S_1 \lor S_2) \land \neg (S_1 \land S_2))$

E)
P = There is food to be found in de pridelands
R = Rafiki will talk about squashed bananas
S1 = Simba is alive
S2 = Scar will remain as king

1. $(P \implies R)$
2. $(R \lor S_1)$
3. $((R \lor \neg R) \land P)$
4. $(S_2 \iff P)$
5. $(S_1 \implies \neg S_2)$

F)

P = Dorothy plays piano in the morning

C = Roger wakes up cranky

D = Dorothy is distracted

R = It will rain on tuesday

S = It will snow on tuesday

N1 = Neville will be sad

N2 = Neville will be cold

Z = Zoog remembered to do his chores

T1 = Things are clean

T2 = Things are neat

1. $(P \rightarrow C), ((P \lor D) \land \neg (P \land D)) \therefore (\neg C \rightarrow D)$
2. $(R \lor S), (R \implies N_1), (S \implies N_2)\therefore(N_1 \lor N_2)$
3. $(Z \implies (T_1 \land \neg T_2)), (\neg Z (\neg T_1 \land T_2))\therefore((T_1 \lor T_2) \land \neg (T_1 \land T_2))$

G)
$$
(\neg (P \land Q) \land \neg (\neg P \land \neg Q))
$$
$$
((\neg P \leftrightarrow Q) \land (\neg Q \leftrightarrow P))
$$
No, it is not possible

---
A)

1. yes
2. yes
3. yes
4. no
5. yes
6. yes
7. yes
8. yes

B)

All the parts (2-6) rely on A already being a tfl sentence. THe only way for A to be a tfl sentence is with part 1 of the defenition. Therefore every tfl sentence contains at least one atomic sentence.

C)
$$(H \implies I), [(H \implies I) \lor (I \implies H)], (I \implies H), [(H \implies I) \lor (I \implies H)] \land (J \lor K), (J \lor K)$$
D)

The count will always already be 1 when you start (because a sentence starts with a bracket), so the first connective will be the main logical operator. However, if the first logical operator is inside nested brackets then the count will return to 1 after you have passed those brackets, so you will always get the right operator.