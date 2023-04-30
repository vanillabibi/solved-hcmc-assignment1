Download Link: https://assignmentchef.com/product/solved-hcmc-assignment1
<br>
Assignment 1 version 1.0

After completing this assignment, you will be able to

<ul>

 <li>define formally lexicon of a programming language.</li>

 <li>use ANTLR to implement a lexer for a programming language.</li>

 <li>define formally grammar of a programming language.</li>

 <li>use ANTLR to implement a recognizer for a programming language.</li>

</ul>

<h1><a name="_Toc2238"></a>1           Specification</h1>

In this assignment, you are required to write a lexer and a recognizer for a program written in BKIT. To complete this assignment, you need to:

<ul>

 <li>Install Python 3 if you have not installed it yet.</li>

 <li>Download initial.zip and unzip it.</li>

 <li>Download antlr-4.8-complete.jar from https://www.antlr.org/download.html, set the environment variable ANTLR_JAR to this file; install antlr4-python3-runtime (see instructions in section Python Targets of the above webpage).</li>

 <li>Remove all files in folders initial/src/main/bkit/utils, initial/src/main/bkit/astgen, initial/src/main/bkit/checker if any.</li>

 <li>Test the initial code again with just three following tructions:</li>

</ul>

python run.py gen python run.py test LexerSuite python run.py test ParserSuite

<ul>

 <li>Change folder initial into assignment1 To complete this assignment, you need to:</li>

 <li>read carefully the specification of language</li>

 <li>Modify BKIT.g4. in the initial code to describe formally BKIT language.Please fill in your id in the header of this file.</li>

 <li>Add more test in LexerSuite and ParserSuite in the initial code.</li>

</ul>

This assignment is divided two phases: lexer phase and recognizer phase. These phases are assessed independently.

<h2><a name="_Toc2239"></a>1.1           Phase 1: Lexer</h2>

In this phase, you are required to write a lexer for a program written in ANTLR. To complete this phase, you need to:

<ul>

 <li>Modify BKIT.g4 to detect tokens in BKIT language.</li>

 <li>Make 100 testcases for LexerSuite to test your code.</li>

 <li>For lexical errors, please return the following tokens together with specific lexemes:

  <ul>

   <li>ERROR_CHAR with &lt;unrecognized char&gt; lexeme: when the lexer detects an unrecognized character</li>

   <li>UNCLOSE_STRING with &lt;unclosed string&gt; lexeme: when the lexer detects an unterminated string. The &lt;unclosed string&gt; lexeme does not include the opening quote.</li>

   <li>ILLEGAL_ESCAPE with &lt;wrong string&gt; lexeme: when the lexer detects an illegal escape in string. The wrong string is from the beginning of the string (without the opening quote) to the illegal escape.</li>

   <li>UNTERMINATED_COMMENT without any lexeme: when the detects an unterminated comment.</li>

  </ul></li>

 <li>You can assume that there is only one error in each test case.</li>

</ul>

<h2><a name="_Toc2240"></a>1.2           Phase 2: Recognizer</h2>

In this phase, you are required to write a recognizer for a program written in BKIT. To complete this phase, you need to:

<ul>

 <li>Modify BKIT.g4.</li>

 <li>Make 100 testcases for ParserSuite to test your code.</li>

 <li>You can assume that there is at most one error in each test case.</li>

</ul>

<h1><a name="_Toc2241"></a>2           Requirements</h1>

Note that you must NOT compress your files when submit them. You MUST submit three files BKIT.g4, LexerSuite.py and ParserSuite.py in BKeL.

The deadline of both phases of assignment 1 is given in the assessment tool.

You must complete the assignment by yourself and do not let your work seen by someone else, otherwise, you will be punished by the university rule for plagiarism.

<h1><a name="_Toc2242"></a>3           Change Log</h1>