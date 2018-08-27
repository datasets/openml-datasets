The resources for this dataset can be found at https://www.openml.org/d/3

Author: Alen Shapiro
Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Chess+(King-Rook+vs.+King-Pawn))    
Please cite: [UCI citation policy](https://archive.ics.uci.edu/ml/citation_policy.html)  

1. Title: Chess End-Game -- King+Rook versus King+Pawn on a7
    (usually abbreviated KRKPA7).  The pawn on a7 means it is one square
    away from queening.  It is the King+Rook's side (white) to move.
 
 2. Sources:
     (a) Database originally generated and described by Alen Shapiro.
     (b) Donor/Coder: Rob Holte (holte@uottawa.bitnet).  The database
         was supplied to Holte by Peter Clark of the Turing Institute
         in Glasgow (pete@turing.ac.uk).
     (c) Date: 1 August 1989
 
 3. Past Usage:
      - Alen D. Shapiro (1983,1987), "Structured Induction in Expert Systems",
        Addison-Wesley.  This book is based on Shapiro's Ph.D. thesis (1983)
        at the University of Edinburgh entitled "The Role of Structured
        Induction in Expert Systems".
      - Stephen Muggleton (1987), "Structuring Knowledge by Asking Questions",
        pp.218-229 in "Progress in Machine Learning", edited by I. Bratko
        and Nada Lavrac, Sigma Press, Wilmslow, England  SK9 5BB.
      - Robert C. Holte, Liane Acker, and Bruce W. Porter (1989),
        "Concept Learning and the Problem of Small Disjuncts",
        Proceedings of IJCAI.  Also available as technical report AI89-106,
        Computer Sciences Department, University of Texas at Austin,
        Austin, Texas 78712.
 
 4. Relevant Information:
       The dataset format is described below.  Note: the format of this
     database was modified on 2/26/90 to conform with the format of all
     the other databases in the UCI repository of machine learning databases.
 
 5. Number of Instances: 3196 total
 
 6. Number of Attributes: 36
 
 7. Attribute Summaries:
     Classes (2):  -- White-can-win ("won") and White-cannot-win ("nowin").
           I believe that White is deemed to be unable to win if the Black pawn
           can safely advance.
     Attributes: see Shapiro's book.
 
 8. Missing Attributes: --  none
 
 9. Class Distribution:
     In 1669 of the positions (52%), White can win.
     In 1527 of the positions (48%), White cannot win.
 
 The format for instances in this database is a sequence of 37 attribute values.
 Each instance is a board-descriptions for this chess endgame.  The first
 36 attributes describe the board.  The last (37th) attribute is the
 classification: "win" or "nowin".  There are 0 missing values.
 A typical board-description is
 
 f,f,f,f,f,f,f,f,f,f,f,f,l,f,n,f,f,t,f,f,f,f,f,f,f,t,f,f,f,f,f,f,f,t,t,n,won
 
 The names of the features do not appear in the board-descriptions.
 Instead, each feature correponds to a particular position in the
 feature-value list.  For example, the head of this list is the value
 for the feature "bkblk".  The following is the list of features, in
 the order in which their values appear in the feature-value list:
 
 [bkblk,bknwy,bkon8,bkona,bkspr,bkxbq,bkxcr,bkxwp,blxwp,bxqsq,cntxt,dsopp,dwipd,
  hdchk,katri,mulch,qxmsq,r2ar8,reskd,reskr,rimmx,rkxwp,rxmsq,simpl,skach,skewr,
  skrxp,spcop,stlmt,thrsk,wkcti,wkna8,wknck,wkovl,wkpos,wtoeg]
 
 In the file, there is one instance (board position) per line.
 
 
 Num Instances:     3196
 Num Attributes:    37
 Num Continuous:    0 (Int 0 / Real 0)
 Num Discrete:      37
 Missing values:    0 /  0.0%

     name                      type enum ints real     missing    distinct  (1)
   1 'bkblk'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   2 'bknwy'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   3 'bkon8'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   4 'bkona'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   5 'bkspr'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   6 'bkxbq'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   7 'bkxcr'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   8 'bkxwp'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
   9 'blxwp'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  10 'bxqsq'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  11 'cntxt'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  12 'dsopp'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  13 'dwipd'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  14 'hdchk'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  15 'katri'                   Enum 100%   0%   0%     0 /  0%     3 /  0%   0% 
  16 'mulch'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  17 'qxmsq'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  18 'r2ar8'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  19 'reskd'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  20 'reskr'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  21 'rimmx'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  22 'rkxwp'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  23 'rxmsq'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  24 'simpl'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  25 'skach'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  26 'skewr'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  27 'skrxp'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  28 'spcop'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  29 'stlmt'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  30 'thrsk'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  31 'wkcti'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  32 'wkna8'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  33 'wknck'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  34 'wkovl'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  35 'wkpos'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  36 'wtoeg'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0% 
  37 'class'                   Enum 100%   0%   0%     0 /  0%     2 /  0%   0%