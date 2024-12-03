Dear Sam,

I had a thought about quantifiers and I wanted to confirm whether it is correct. Is it true that the exists quantifier is just an infinite string of 'or’-statements appended together, and the universal quantifier an infinite string of ‘and’-statements. So you would then get:
∃xPx = Pa ∨ Pb ∨ Pc ∨ Pa1 ∨ Pb1 ∨ Pc1 ∨ Pa2 ∨ Pb2 ∨ Pc2 ∨ Pa3 ∨ Pb3 ∨ Pc3 ... 
∀xPx = Pa ∧ Pb ∧ Pc ∧ Pa1 ∧ Pb1 ∧ Pc1 ∧ Pa2 ∧ Pb2 ∧ Pc2 ∧ Pa3 ∧ Pb3 ∧ Pc3 …
where the constants would take up every possible value in the domain. And that you could then prove all the ∃- and ∀-introduction and -elimination rules with the ∧- and ∨-rules (because they are essentially the same rules):
- So for the ∀-Intro rule one could prove it by saying that it is exactly the same as the ∧-Intro rule (where you can put things together if you have proven them individually) and the restrictions on the arbitrary variable make sure that the proof would be valid for every single atomic sentence in the infinite string of ∧-statements.
- And the ∀-Elim rule with the ∧-Elim rule because the ∧-Elim would say you could get any single one of the constituent atomic sentences in the endless string of ∧-statements.
- The ∃-Intro rule would be the same as the the ∨-Intro rule, because you could add an endless amount of ‘or’s when you have a single one.
- And finally the  ∃-Elim rule with the ∨-Elim rule because the restrictions on the arbitrary variable make sure that the proof would be valid for every single constituent atomic sentence in the infinite string of ∨-statements.

It seems like the quantifier-rules are exactly the same as the or- and and-rules. Is it correct to think of the quantifiers this way or am I not seeing something?

Kind regards,

Olivier

---

Dear Olivier,


That's a perceptive suggestion, although there are a few issues:

- You would have to modify the syntax of _L2_ to allow for infinite sentences, and would have to deal with the technical issues that arise from this. (For example, what is the new recursive definition of sentences?) Nevertheless, logicians have considered such [infinitary logics](https://plato.stanford.edu/entries/logic-infinitary/ "https://plato.stanford.edu/entries/logic-infinitary/").
    
- "where the constants would take up every possible value in the domain": this is a constraint on an _L2_-structure, and so this interpretation would have to modify the semantics of _L2_ as well. This would also have the consequence of restricting the semantics to countable domains—those no larger than the counting numbers—since even an infinite string of atomic sentences wouldn't be able to render a sentence like "all real numbers are self-identical". (There are too many real numbers for them to be put one-to-one in correspondence with the counting numbers.)
    
- If you didn't modify the semantics, then the result would not have the same truth conditions as the quantifiers, for there's no guarantee that every object in the domain of some _L2_-structure is the semantic value for a constant. Still, logicians have considered these so-called[substitutional quantifiers](https://plato.stanford.edu/entries/quantification/#SubQua "https://plato.stanford.edu/entries/quantification/#SubQua").
    
- To reduce the quantifier proof rules to the conjunction and disjunction proof rules, you'd have to allow for infinitary proofs, of course.

---

Dear Sam,

Thank you very much! However, could you not say that the syntax of L2 is already modified by allowing for the quantifiers. And that the quantifiers are conceptually exactly the infinite ‘or’s and ‘and’s? Because, when we are defining the quantifiers, is it not exactly this what we are doing, at least on a conceptual level? So then it would not have to have any implications for L2 itself.

Kind regards,

Olivier

---
