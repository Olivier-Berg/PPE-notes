#class #logics
[[Week 4.pdf]]
[[Topic 4]]
YOU SHOULD UNDERSTAND THE DIFFERENCE BETWEEN $\exists x (Ax \land Bx)$ and $\exists x (Ax \rightarrow Bx)$, and $\forall x (Ax \rightarrow Bx)$ and $\forall x (Ax \land Bx)$.

"In TLM it says "the upper index is called the predicate letter's 'arity-index' [...] The number of strings of dots must always correspond the the arity-index of the predicate letter." (p. 76-77)
Then what arity-index would this get (two strings of dots but only one predicate needed):
$P^?$: $..._1$ loves $..._1$ (themselves)

Why can only P, Q and R be predicate letters? page 82
why only a, b, c constants
and only xyz variables

p. 91: why can't "... has a computer" not just be a predicate, why does it have to be "... has ..."
... and why is it different for 'is' p. 78, 
**Because for "is ..."  the "..." is usually a adjective, so then there is no way to fill it. It makes sense for "is a scrooge".**
"... has ..." usually is an existential claim: "for all x (if x is a person, then for at least one y (y is a soul and x has y))"


in TLM there is no mention of a domain, does that mean that the domain is just always "everything"

---

"In the definition of formulae (Def'n. 4.7), TLM does not include forallx's restriction (on p. 83) on the formulae to which quantifiers can be prepended to produce other formulae. However, a restriction like that is ultimately needed (implicitly) for TLM's definition of an _L_2-sentence (Def'n. 4.10). I will discuss what I take to be a more elegant version of this restriction in class." what do you mean?

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

-----------------------

Pc ∨ ∃z Qzz

  

"I apply the rule for eliminating ∀ by deleting

∀z and by replacing all free occurrences of z

in the formula by the constant c.”

  

Here, Volker Halbach only talks about replacing the free occurrences, so perhaps he regards variables captured by ∃z as different from the variables captured by ∀z. Also, the fact that he uses ∀z (Pz ∨ ∃z Qzz) as an example should mean that he regards it as a sentence of L2 (he gives it a truth value). Or am I not seeing something here? See you tomorrow!

  

Kind regards,

Olivier