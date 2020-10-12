# Implementation and solver for tic-tac-two

### Game description:
- Two players take turns placing their pieces on a 3-by-3 grid (similar to regular tic-tac-toe)
- Player wins if they have 3 claimed squares in a line (horizontal, vertical, or diagonal)
- Player claims square when they are the first to get 2 of their own piece on the square
- Once per game, each player may move twice in a row.

### Current Solve:
```
Tic Tac Two analysis (symmetries removed):
Remote  Win      Lose     Tie      Total
----------------------------------------
20      0        7        0        7      
19      6        0        0        6      
18      0        47       0        47     
17      92       0        1        93     
16      0        314      24       338    
15      831      0        281      1112   
14      0        1765     1396     3161   
13      4814     0        4553     9367   
12      0        7510     12236    19746  
11      19733    0        24860    44593  
10      0        25653    46386    72039  
9       57785    0        68772    126557 
8       0        73263    92617    165880 
7       139885   0        98406    238291 
6       0        174476   93263    267739 
5       294673   0        69001    363674 
4       0        247917   43888    291805 
3       964667   0        22882    987549 
2       0        440580   10534    451114 
1       1175065  0        958      1176023
0       0        130219   48       130267 
------------------------------------------
Total   2657551  1101751  590106   4349408

```
```
Tic Tac Two analysis (symmetries not removed):
Remote  Win      Lose     Tie      Total
----------------------------------------
20      0        52       0        52     
19      48       0        0        48     
18      0        356      0        356    
17      724      0        1        725    
16      0        2480     118      2598   
15      6574     0        1891     8465   
14      0        13873    10224    24097  
13      37840    0        34750    72590  
12      0        58914    94957    153871 
11      155028   0        195183   350211 
10      0        202274   365938   568212 
9       455625   0        543872   999497 
8       0        577940   733167   1311107
7       1100011  0        778961   1878972
6       0        1376918  737732   2114650
5       2321914  0        545200   2867114
4       0        1951273  345512   2296785
3       7635647  0        179080   7814727
2       0        3471465  81448    3552913
1       9278322  0        6880     9285202
0       0        1007854  256      1008110
------------------------------------------
Total   20991733  8663399  4655170  34310302
```

### Tie-slowly solve (deprecated):
```
Tic Tac Two analysis (symmetries removed):
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
10/12/20 (brian): Switched to tie-quickly solve, added symmetry and non-symmetry solves to README.

10/3/20 (janise): fixed formatting for output and added capture of current output. will verify correctness and try to optimize -- currently solves in 58 seconds on my computer

10/2/20 (brian): Uploaded own base code, with possible TT2 implementation. No guarantee it actually works, and definetly not efficient.

9/30/20 (janise): uploaded tic tac toe, solver, and Game abstract class to use as base code
