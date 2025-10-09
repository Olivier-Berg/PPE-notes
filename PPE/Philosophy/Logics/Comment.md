Last year, Sam Fletcher was wrong about something, so make sure he isn't this year again:
He said that you can't put a quantifier over for instance x if there is already a quantifier over x:
$$
\exists x \forall x (Px \land Qx)
$$
He thought that this was not allowed, but it is allowed, so I think he updated his stuff about it. Though also notice that doing this is useless, the first quantifier does not do anything. See below why it is allowed:

---

Dear Sam,

I have a question about one of the things you pointed out last week. On the Sharepoint it says: 

"In the definition of formulae (Def'n. 4.7), TLM does not include forallx's restriction (on p. 83) on the formulae to which quantifiers can be prepended to produce other formulae. However, a restriction like that is ultimately needed (implicitly) for TLM's definition of an _L_2-sentence (Def'n. 4.10). I will discuss what I take to be a more elegant version of this restriction in class.”

I was wondering why it is ultimately needed. Forallx talks about a variable not serving multiple masters, but can I not just do:

Domain: {0}

G: {⟨0, 0⟩}

And then say:

∀x∃xGxx

This was also the example that Ronya gave to show that it was possible. So what exactly is the problem in this sentence?

Thanks in advance!

Kind regards,

Olivier

---

Dear Olivier,

Ultimately, the issue concerns the interaction between the semantics and proof system for _L_2. The quickest way to see this is to look at some of the exposition in TLM:

> In general, what _α_ assigns to variables not occuring freely in a formula _ϕ_ does not impinge on whether _α_ satisfies _ϕ_ in _A_. ... If _ϕ_ is a sentence, that is, if no variable occurs freely in _ϕ_, then [the truth value of _ϕ_ under a variable assignmen _α_] does not depend on the variable assignment _α_ in any way at all. (p. 104)

If you apply this to your expression,∀x∃xGxx, then we learn that it must have the same truth value as ∃xGxx. Thus, the two are logically equivalent. (Note the same would be true if the main connective were, say, a y-quantifier rather than an x-quantifier.)

However, the proof system that we will learn for _L_2 does not let us infer ∀x∃xGxx from ∃xGxx. The relevant rule is ∀ introduction, and has the following feature:

> in application of the rule, one has to make sure that the variable of the newly introduced quantifier is not caught by a quantifier that is already in the formula. (p. 137)

This means that there is a semantically valid argument for which there is no proof, meaning that the proof system cannot be complete as stated, if ∀x∃xGxx is taken to be a sentence of _L_2. (Note how this issue does not arise if the universal quantifier were, say, a y-quantifier!)

I hope that helps explain what I see the issue to be.

Best wishes,

---

Dear Sam,

Thank you very much for the explanation! However, I think that Volker Halbach has a slightly different interpretation. In his lecture last week, he actually used the following example to showcase the ∀-elimination rule (also see the attached screenshot from his lecture slides):

To prove: ∀z (Pz ∨ ∃z Qzz) ⊢ Pc ∨ ∃z Qzz

∀z (Pz ∨ ∃z Qzz)

\-------------------

Pc ∨ ∃z Qzz

"I apply the rule for eliminating ∀ by deleting

∀z and by replacing all free occurrences of z

in the formula by the constant c.”

Here, Volker Halbach only talks about replacing the free occurrences, so perhaps he regards variables captured by ∃z as different from the variables captured by ∀z. Also, the fact that he uses ∀z (Pz ∨ ∃z Qzz) as an example should mean that he regards it as a sentence of L2 (he gives it a truth value). Or am I not seeing something here? See you tomorrow!

Kind regards,

Olivier

![[Scherm­afbeelding 2024-11-25 om 00.15.22.png]]

---


Dear Olivier,

Yes, the direction involving∀-elimination is okay; the problem comes in the other direction, with ∀-introduction, when one tries to show the logical equivalence of the sentences discussed in our previous email exchange.

All best,


---

Dear Sam,

Of course, but the same would then also be true for ∀-introduction, I also asked this this morning to Volker Halbach to make sure that my interpretation of him was correct and he pointed out that he had specifically accounted for this scenario in another definition.

The problem of course was that on page 137 he says:

"in application of the rule, one has to make sure that the variable of the newly introduced quantifier is not caught by a quantifier that is already in the formula.”

The rule is of course:

    ⋮

 φ[t/v]

\----------∀Intro

 ∀vφ

However, when he introduces the notation for substitution, he explicitly states:

_“DEFINITION 6.12. Assume v is a variable, t a constant, and ϕ an L2-formula with at most v occurring freely. Then  φ[t/v] is the sentence obtained by replacing all free occurrences of v in ϕ by t.”_ (p. 131)

So, φ[t/v] is the sentence obtained by only replacing all _free_ occurrences of v in ϕ by t. As there are no free occurrences of x in ∃xGxx, all the free occurrences are already replaced by a constant. Therefore, one can add ∀x to ∃xGxx to get ∀x∃xGxx according to the ∀Intro rule. Therefore there is a valid proof of ∃xGxx ⊦ ∀x∃xGxx, which makes the proof system complete.

Volker Halbach also explains this further on the bottom of page 132, with the ∀-Elim rule (but it shows the same thing):

“The following example explains why only free occurrences of the variable are replaced:

∀y(Py∧∃yQy)

-----------------∀Elim

 Pb5 ∧∃yQy

If one were allowed to replace also the last occurrence of y, which is bound, one would to get to Pb ∧∃yQb, which is logically equivalent to Pb ∧Qb. This step is clearly not sound: from ∀y(Py∧∃yQy) it does not follow that b is Q. Intuitively speaking, only occurrences of y in ∀y (Py ∧ ∃y Qy) that are ‘caught’ by the universal quantifier ∀y can be replaced by the constant; the last occurrence of y belongs to the existential quantifier and must be left alone."

So, I think what he means with the restriction on page 137 for the introduction rule is that one cannot infer for instance:

Qc ∧ ∃xRcx

\----------------

∀x(Qx ∧ ∃xRxx)

Which would of course not be a valid proof (he explains this on page 134-135). So what he means with that a variable is not already caught by another quantifier is here that the variable x (when one replaces c with x) is already caught by the ∃x quantifier, so it would get the wrong scope. Here is ∃xRxx the scope but the intended scope was the entire sentence (see page 134-135).

I hope that makes sense!

Kind regards,

Olivier

---

