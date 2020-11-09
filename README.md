# pairwise-parallelization
This repository is dedicated to help using the parallelization procedure exposed in the following paper:
....
To compile the code just run make in the folder after changing the pathes in the file 
  makefile
The program can be run directly on a command line:
/YourPath/SPAPCA #ofindivudals /YourPath/fileresult.txt
Where #ofindivudals is the number of indivudals and /YourPath/fileresult.txt the name of the file to store the result
Alternatively the script SPAPCA.sh can be run modified and ran
The program is currently limited to a number of individuals of 400,000,000 but we don t recomand running it for that many inidvudals as the file with the composition of all subsets will be too big.
As a toy example, we give here the composition of the 132 subsets for 100 individuals 
0 1 2 3 4 5 6 7 8 9 10 

11 12 13 14 15 16 17 18 19 20 21 
22 23 24 25 26 27 28 29 30 31 32 
33 34 35 36 37 38 39 40 41 42 43 
44 45 46 47 48 49 50 51 52 53 54 
55 56 57 58 59 60 61 62 63 64 65 
66 67 68 69 70 71 72 73 74 75 76 
77 78 79 80 81 82 83 84 85 86 87 
88 89 90 91 92 93 94 95 96 97 98 
99 100 

0 11 22 33 44 55 66 77 88 99 
1 12 23 34 45 56 67 78 89 
2 13 24 35 46 57 68 79 90 
3 14 25 36 47 58 69 80 91 
4 15 26 37 48 59 70 81 92 
5 16 27 38 49 60 71 82 93 
6 17 28 39 50 61 72 83 94 
7 18 29 40 51 62 73 84 95 
8 19 30 41 52 63 74 85 96 
9 20 31 42 53 64 75 86 97 
10 21 32 43 54 65 76 87 98 
0 12 24 36 48 60 72 84 96 
1 13 25 37 49 61 73 85 97 
2 14 26 38 50 62 74 86 98 99 
3 15 27 39 51 63 75 87 88 100 
4 16 28 40 52 64 76 77 89 
5 17 29 41 53 65 66 78 90 
6 18 30 42 54 55 67 79 91 
7 19 31 43 44 56 68 80 92 
8 20 32 33 45 57 69 81 93 
9 21 22 34 46 58 70 82 94 
10 11 23 35 47 59 71 83 95 
0 13 26 39 52 65 67 80 93 
1 14 27 40 53 55 68 81 94 
2 15 28 41 54 56 69 82 95 
3 16 29 42 44 57 70 83 96 
4 17 30 43 45 58 71 84 97 99 
5 18 31 33 46 59 72 85 98 100 
6 19 32 34 47 60 73 86 88 
7 20 22 35 48 61 74 87 89 
8 21 23 36 49 62 75 77 90 
9 11 24 37 50 63 76 78 91 
10 12 25 38 51 64 66 79 92 
0 14 28 42 45 59 73 87 90 
1 15 29 43 46 60 74 77 91 
2 16 30 33 47 61 75 78 92 
3 17 31 34 48 62 76 79 93 
4 18 32 35 49 63 66 80 94 
5 19 22 36 50 64 67 81 95 
6 20 23 37 51 65 68 82 96 99 
7 21 24 38 52 55 69 83 97 100 
8 11 25 39 53 56 70 84 98 
9 12 26 40 54 57 71 85 88 
10 13 27 41 44 58 72 86 89 
0 15 30 34 49 64 68 83 98 
1 16 31 35 50 65 69 84 88 
2 17 32 36 51 55 70 85 89 
3 18 22 37 52 56 71 86 90 
4 19 23 38 53 57 72 87 91 
5 20 24 39 54 58 73 77 92 
6 21 25 40 44 59 74 78 93 
7 11 26 41 45 60 75 79 94 
8 12 27 42 46 61 76 80 95 99 
9 13 28 43 47 62 66 81 96 100 
10 14 29 33 48 63 67 82 97 
0 16 32 37 53 58 74 79 95 100 
1 17 22 38 54 59 75 80 96 
2 18 23 39 44 60 76 81 97 
3 19 24 40 45 61 66 82 98 
4 20 25 41 46 62 67 83 88 
5 21 26 42 47 63 68 84 89 
6 11 27 43 48 64 69 85 90 
7 12 28 33 49 65 70 86 91 
8 13 29 34 50 55 71 87 92 
9 14 30 35 51 56 72 77 93 
10 15 31 36 52 57 73 78 94 99 
0 17 23 40 46 63 69 86 92 
1 18 24 41 47 64 70 87 93 99 
2 19 25 42 48 65 71 77 94 100 
3 20 26 43 49 55 72 78 95 
4 21 27 33 50 56 73 79 96 
5 11 28 34 51 57 74 80 97 
6 12 29 35 52 58 75 81 98 
7 13 30 36 53 59 76 82 88 
8 14 31 37 54 60 66 83 89 
9 15 32 38 44 61 67 84 90 
10 16 22 39 45 62 68 85 91 
0 18 25 43 50 57 75 82 89 
1 19 26 33 51 58 76 83 90 
2 20 27 34 52 59 66 84 91 
3 21 28 35 53 60 67 85 92 99 
4 11 29 36 54 61 68 86 93 100 
5 12 30 37 44 62 69 87 94 
6 13 31 38 45 63 70 77 95 
7 14 32 39 46 64 71 78 96 
8 15 22 40 47 65 72 79 97 
9 16 23 41 48 55 73 80 98 
10 17 24 42 49 56 74 81 88 
0 19 27 35 54 62 70 78 97 
1 20 28 36 44 63 71 79 98 
2 21 29 37 45 64 72 80 88 
3 11 30 38 46 65 73 81 89 
4 12 31 39 47 55 74 82 90 
5 13 32 40 48 56 75 83 91 99 
6 14 22 41 49 57 76 84 92 100 
7 15 23 42 50 58 66 85 93 
8 16 24 43 51 59 67 86 94 
9 17 25 33 52 60 68 87 95 
10 18 26 34 53 61 69 77 96 
0 20 29 38 47 56 76 85 94 
1 21 30 39 48 57 66 86 95 
2 11 31 40 49 58 67 87 96 
3 12 32 41 50 59 68 77 97 
4 13 22 42 51 60 69 78 98 
5 14 23 43 52 61 70 79 88 
6 15 24 33 53 62 71 80 89 
7 16 25 34 54 63 72 81 90 99 
8 17 26 35 44 64 73 82 91 100 
9 18 27 36 45 65 74 83 92 
10 19 28 37 46 55 75 84 93 
0 21 31 41 51 61 71 81 91 
1 11 32 42 52 62 72 82 92 
2 12 22 43 53 63 73 83 93 
3 13 23 33 54 64 74 84 94 
4 14 24 34 44 65 75 85 95 
5 15 25 35 45 55 76 86 96 
6 16 26 36 46 56 66 87 97 
7 17 27 37 47 57 67 77 98 
8 18 28 38 48 58 68 78 88 
9 19 29 39 49 59 69 79 89 99 
10 20 30 40 50 60 70 80 90 100 


