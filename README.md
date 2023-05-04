Download Link: https://assignmentchef.com/product/solved-csci-446-artificial-intelligence-assignment-1-search
<br>
In this assignment, you will build general-purpose search algorithms and apply them to solving puzzles. You will be in charge of a “Pacman” agent that needs to find paths through mazes looking for the “food pellet” (star).

As stated in the beginning of the course, <strong>you are free to use any high-level programming language you are comfortable with</strong>. This includes (but is not limited to) Java, C++, and Python. The focus of this course is on problem solving, not programming, and the grading will primarily be based on the quality of your solutions and your analysis, as evidenced by your <strong>written report</strong>.

<strong>You have the option of working in groups of up to three people.</strong>  Needless to say, working in a group will not necessarily make your life easier, as the overhead of group coordination can easily outweigh the benefits.

<h1>Description</h1>

<h2>1.1 Basic pathfinding</h2>

Consider the problem of finding the shortest path from a given start state to the one star or “food pellet”. The image at the top of this page illustrates the simple scenario of a single food pellet, which in this case can be viewed as the unique goal state. The maze layout will be given to you in a simple text format, where ‘%’ stands for walls, ‘P’ for the starting position, and ‘*’ for the food pellet/star.  All step costs are equal to one.

Implement the state representation, transition model, and goal test needed for solving the problem. For the state representation, besides your current position in the maze, is there anything else you need to keep track of? Next, implement a unified top-level search routine that can work with all of the following search strategies, as covered in class:

<ul>

 <li>Depth-first search;</li>

 <li>Breadth-first search; Greedy best-first search;</li>

 <li>A* search.</li>

</ul>

For this part of the assignment, use the Manhattan distance from the current position to the goal as the heuristic function for greedy and A* search.

Run each of the four search strategies on the following inputs:

<ul>

 <li><u>Medium maze</u>;</li>

 <li><u>Big maze</u>; <u>Open maze</u>.</li>

</ul>

For each problem instance and each search algorithm, include the following in your report:

<ul>

 <li>The solution, displayed by putting a ‘.’ in every maze square visited on the path.</li>

 <li>The path cost of the solution, defined as the number of steps taken to get from the initial state to the goal state.</li>

 <li>Number of nodes expanded by the search algorithm. <strong>Tips </strong></li>

 <li>In your implementation, make sure you get all the bookkeeping right. This includes handling of repeated states (in particular, what happens when you find a better path to a state already on the frontier) and saving the optimal solution path. These topics have been extensively covered during the lectures.</li>

 <li>Pay attention to tiebreaking. If you have multiple nodes on the frontier with the same minimum value of the evaluation function, the speed of your search and the quality of the solution may depend on which one you select for expansion. Make sure you implement a unified top-level search algorithm that can take each of the four strategies as special cases. In particular, while DFS can be implemented very compactly using recursion, we want you to avoid this approach for the sake of the assignment (among other things, you can much more easily exceed the maximum depth of the recursion stack than if you explicitly represent the frontier as a stack).</li>

 <li>You will be graded primarily on the correctness of your solution, not on the efficiency and elegance of your data structures. For example, we don’t care whether your data structure or repeated state detection uses brute-force search, as long as you end up expanding (roughly) the correct number of nodes and find the optimal solution. So, feel free to use “dumb” data structures as long as it makes your life easier and still enables you to find the solutions to all the inputs in a reasonable amount of time.</li>

</ul>

<h1>Report Checklist</h1>

Your report should briefly describe your implemented solution.  Your description should focus on the most “interesting” aspects of your solution, i.e., any non-obvious implementation choices (including programming language chosen) and parameter settings, and what you have found to be especially important for getting good performance. Feel free to include pseudocode (DO NOT PUT CODE IN YOUR

REPORT) or figures if they are needed to clarify your approach. Your report should be self-contained and it should (ideally) make it possible for us to understand your solution without having to run your source code. For full credit, in addition to the algorithm descriptions, your report should include the following

For every algorithm (DFS, BFS, Greedy, A*) and every one of the three mazes (medium, big, open): give the maze with the computed path, the solution cost, and the number of expanded nodes (12 cases total).

<strong>Statement of individual contribution: </strong>

<ul>

 <li>All group reports need to include a write up from each group member on what you were responsible for and what you found hard, interesting, unexpected, etc. We reserve the right to contact group members individually to verify this information.</li>

</ul>

<strong><em>WARNING: You will not get credit for any solutions that you have obtained, but not included in your report!</em></strong> For example, if your code prints out path cost and number of nodes expanded on each input, but you do not put down the actual numbers in your report.




<h1>Submission Instructions</h1>

By the submission deadline, <strong>one designated person from the group</strong> will need to upload the following to D2L/Brightspace:

<ol>

 <li>A <strong>report</strong> in <strong>PDF format</strong>. Be sure to put the <strong>names</strong> of all the group members at the top of the report. The name of the report file should be <strong>pdf</strong> (based on the name of the designated person).</li>

 <li>Your <strong>source code</strong> compressed to a <strong>single ZIP file</strong>. The code should be well commented, and it should be easy to see the correspondence between what’s in the code and what’s in the report. You don’t need to include executables or various supporting files (e.g., utility libraries) whose content is irrelevant to the assignment. If we find it necessary to run your code in order to evaluate your solution, we will get in touch with you. INCLUDE YOUR OUTPUT FILE IN THIS ZIP FILE.</li>

</ol>




The name of the code archive should be <strong>lastname_firstname_a1.zip</strong>.

Multiple attempts will be allowed but only your last submission before the deadline will be graded. <strong>We reserve the right to take off points for not following directions.</strong>

<strong>Late policy:</strong> You must submit by Midnight of Oct 8 the full package (report and source code).  No exceptions.


