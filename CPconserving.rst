(******************************************************************)
(*     Restriction file for 2HDM.fr                               *)
(*                                                                *)                                            
(*     CP symmetry                                                *)
(******************************************************************)

M$Restrictions = {
          mixh2 -> 0,
          mixh3 -> 0,
          l7I -> 0,
          TH[1,3]->0,
          TH[2,3]->0,
          TH[3,1]->0,
          TH[3,2]->0,
          Conjugate[l7]->l7,
          Conjugate[l5]->l5,
          Conjugate[l6]->l6(*  ,
         
   (* G(L,D,U) have to be hermitian, together with the flavor symmetry, this reduce to  : *)      
        GLI[i_, i_] :> 0,
          GDI[i_, i_] :> 0,
          GUI[i_, i_] :> 0*)
}
