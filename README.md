# DrinfeldModules

  #IsomorphismClasses
  This algorithm is a part of the larger project titled "Isomorphism classes of Drinfeld modules over finite fields" authored by Karemaker, Katen,
  and Papikian.
  
  
  There are four main functions included:
  
  PicardGroupRepresentatives calculates a list of representatives for the elements of the Picard group of an order in a function field. This is a 
  simplified implementation of the algorithm described in the paper "Computing residue class rings and Picard groups of Orders" authored by Kluners
  and Pauli.
  
  ICM calculates a list of representatives for the elements of the ideal class monoid of an order in a function field. This is an implementation of
  the four-stage algorithm described in the paper "Computing the ideal class monoid of an order" authored by Marseglia.
  
  MinimalPolynomialOfFrobenius calculates the minimal polynomial of the Frobenius endomorphism of a Drinfeld module over a finite field. This is a
  basic yet efficient method I developed using linear algebra and built-in MAGMA function for computing greatest common divisors in multivariate
  polynomial rings with coefficients in finite fields.
  
  IsomorphismClasses computes, for a given Drinfeld module φ with minimal endomorphism ring, a list of images of T of a list of unique
  representatives for the isomorphism classes within the isogeny class of φ. The fact that this algorithm is correct is both an important conclusion
  of our project and a practically useful result to aid in the future research of Drinfeld modules over finite fields.

  What is needed to produce an output: 
    phi: RngUPolTwstElt is the image of T under the Drinfeld module for which we are computing the isomorphism classes.
    Fq: FldFin is the coefficient field.
    A: RngUPol is the polynomial ring Fq[T] such that phi is a Drinfeld module A->k{tau}.
    pp: RngUPolElt is the A-characteristic of phi.
    n: RngIntElt is the field extension degree [k:F_q].
    
    
