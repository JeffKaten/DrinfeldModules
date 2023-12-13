# DrinfeldModules
  #IsomorphismClasses
  There are four functions included:
  PicardGroupRepresentatives calculates a list of representatives for the elements of the Picard group of an order in a function field.
  ICM calculates a list of representatives for the elements of the ideal class monoid of an order in a function field.
  MinimalPolynomialOfFrobenius calculates the minimal polynomial of the Frobenius endomorphism of a Drinfeld module over a finite field.
  IsomorphismClasses computes a list of images of T of a list of unique representatives for the isomorphism classes within the isogeny class of phi.

  What is needed to produce an output: 
    phi: RngUPolTwstElt is the image of T under the Drinfeld module for which we are computing the isomorphism classes.
    Fq: FldFin is the coefficient field.
    A: RngUPol is the polynomial ring Fq[T] such that phi is a Drinfeld module A->k{tau}.
    pp: RngUPolElt is the A-characteristic of phi.
    n: RngIntElt is the field extension degree [k:F_q].
    
    
