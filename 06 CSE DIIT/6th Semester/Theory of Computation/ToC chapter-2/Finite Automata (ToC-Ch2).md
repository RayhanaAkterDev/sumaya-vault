1. *What is finite automata?* #board_2021 #board_2020 
2. *What is the utility of finite automata in respect of hardware and software?* #board_2021 
3. *Define NFA and DFA.* #board_2018 #board_2019  
4. *What do you mean by transition table and transition diagram?* #board_2021 
5. *Difference between DFA and NFA*. #board_2022 #board_2021 #board_2019 #board_2017 

| DFA                                                                                                                                                 | NFA                                                                                                    |
| --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| DFA is a FA in which there is only one path for specific input from current state to next state. There is a unique transition on each input symbol. | NFA is the one in which there exists many paths for a specific input from current state to next state. |
| DFA can not use empty string.                                                                                                                       | NFA can use empty string transition.                                                                   |
| DFA can be understood as one machine.                                                                                                               | NFA can be understood as multiple little machines computing at the same time                           |
| For every symbol of the alphabet, there is only one state transition in DFA.                                                                        | We do not need to specify how the NFA reacts according to some symbol.                                 |
| DFA is difficult to design and construct.                                                                                                           | NFA is easier to design and construct.                                                                 |
| Backtracking is allowed in DFA.                                                                                                                     | In NFA, backtracking is not always possible.                                                           |
| Requires more space in DFA.                                                                                                                         | Requires less space.                                                                                   |
| A string accepted by a DFA, if it transits to a final states.                                                                                       | A string is accepted by a NFA, if at least one of all possible transitions ends in a final state.      |
| The language of DFA, L(M) = {W\|}                                                                                                                   | The language of DFA,                                                                                   |
   
   
6. *Design DFA's that accepts: *
	1. Strings starting with $aba$ #board_2021 
	2. Strings containing even number of $0's$ and even number of $1's$ #board_2021 
	3. String start with one and ends with zero #board_2020 
	4. String with aa & bb, $\sum\left\lbrace a,b\right\rbrace$ #board_2020 
	   
7. *Convert to a DFA the following NFA:* #board_2021 
	1. Figure provides on chapter 2 question no. 29]
	2. Figure provides on chapter 2 question no. 27]
		- Convert the following NFA to an equivalent DFA. Here 0 is starting and 10 is final state. #board_2021 #board_2019 
	3. Figure provides on chapter 2 question no. 22]
	   
8. Convert the following NFA to DFA. #board_2022 

|     | 0     | 1   |
| --- | ----- | --- |
| ➡️p | {p,q} | {p} |
| q   | {r}   | {r} |
| r   | {s}   | ∅   |
| *s  | {s}   | {s} |

|     | 0   | 1   |
| --- | --- | --- |
| ➡️A | B   | F   |
| B   | G   | C   |
| *C  | A   | C   |
| E   | H   | F   |
| F   | C   | G   |
| G   | G   | E   |
| H   | G   | C   |

8. Prove that if $D=\left(Q_{D},\sum,\delta_{D,}\left\lbrace q_0\right\rbrace,F_{D}\right)$ is the DFA constructed from NFA $N=\left(Q_{N},\sum,\delta_{N,}\left\lbrace q_0\right\rbrace,F_{N}\right)$ by the subset construction then $L(D) = L(N)$ #board_2021 
9. Prove that, A language L is accepted by some DFA if and only if L is accepted by some NFA. #board_2020 #board_2019 



