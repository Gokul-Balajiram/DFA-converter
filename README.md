INTRODUCTION

Deterministic finite automation (DFA) is a fundamental concept in automata theory and formal language theory, widely used in various fields such as computer science, linguistics and artificial intelligence. DFA’s are mathematical models of computation that recognize regular languages, which are subset of formal languages with simple and regular grammars.
In this case study ,  we focus on the design and implementation of a DFA generator in Python. The objective of this project is to develop a tool that takes input strings and generates the corresponding DFA state diagram in matrix form . The input string represents a language consisting of strings with a base array and power array, where the power array represents the number of times the alphabet in the base array repeats in the language.



ALGORITHM

The algorithm begins by obtaining the set of input alphabets and the corresponding base characters along with their powers. It then constructs a base string by repeating each base character according to its power value.

Next, it initializes a Deterministic Finite Automation (DFA) matrix and creates states based on the generated base string. Each state represents a substring of the base string, and transitions between states are determined by the input alphabet.

To complete the DFA, missing transitions in the matrix are filled in. This is achieved by examining each cell of the DFA matrix. If a transition is missing, the algorithm either assigns an existing state or creates a new trap state, ensuring that every possible transition is accounted for.

 A state array is maintained to track the properties of each state. This includes initializing, creating, and updating state properties as necessary.

The final output is a fully constructed DFA matrix representing the deterministic finite automaton capable of recognizing strings conforming to the specified language. A DFA diagram will be generated using the DFA matrix with the help of the python library : GraphViz
