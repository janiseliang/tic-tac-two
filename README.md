# Implementation and solver for tic-tac-two

### Game description:
- Two players take turns placing their pieces on a 3-by-3 grid (similar to regular tic-tac-toe)
- Player wins if they have 3 claimed squares in a line (horizontal, vertical, or diagonal)
- Player claims square when they are the first to get 2 of their own piece on the square

### Current Solve:
```Tic Tac Two analysis (symmetries removed):
Remote  Win      Lose     Tie      Total
----------------------------------------
27      0        0        1        1      
26      0        0        3        3      
25      0        0        9        9      
24      0        0        70       70     
23      0        0        147      147    
22      0        0        820      820    
21      0        0        1346     1346   
20      0        7        4074     4081   
19      6        0        6364     6370   
18      0        47       13918    13965  
17      92       0        19399    19491  
16      0        314      33204    33518  
15      831      0        39743    40574  
14      0        1765     56273    58038  
13      4814     0        57906    62720  
12      0        7510     70765    78275  
11      19733    0        61905    81638  
10      0        25653    65951    91604  
9       57785    0        47292    105077 
8       0        73263    44244    117507 
7       139885   0        25358    165243 
6       0        174476   21272    195748 
5       294673   0        9431     304104 
4       0        247917   6682     254599 
3       964667   0        2407     967074 
2       0        440580   1076     441656 
1       1175065  0        398      1175463
0       0        130219   48       130267 
------------------------------------------
Total   2657551  1101751  590106   4349408
```

### Updates:
10/3/20 (janise): fixed formatting for output and added capture of current output. will verify correctness and try to optimize -- are there too many positions??

10/2/20 (brian): Uploaded own base code, with possible TT2 implementation. No guarantee it actually works, and definetly not efficient.

9/30/20 (janise): uploaded tic tac toe, solver, and Game abstract class to use as base code
