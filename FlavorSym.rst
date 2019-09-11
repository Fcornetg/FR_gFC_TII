(******************************************************************)
(*     Restriction file for SM.fr                                 *)
(*                                                                *)                                            
(*     The CKM matrix is diagonal                                 *)
(******************************************************************)

M$Restrictions = {
            CKM[i_,i_] -> 1,
            CKM[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            cabi -> 0,
            
            GLR[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GLI[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GDR[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GDI[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GUR[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GUI[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            
            GL[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GD[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j),
            GU[i_?NumericQ, j_?NumericQ] :> 0 /; (i =!= j)
            }

