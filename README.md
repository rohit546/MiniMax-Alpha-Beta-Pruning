# MiniMax-Alpha-Beta-Pruning

Task 1:
Minimax is a method used to evaluate game trees. Implement an algorithm for calculating the optimal
move using Minimax—the move that leads to a terminal state with maximum utility, under the assumption
that the opponent plays in a 2 player game.
MAX
• Wants to maximize the result of the utility function
• Winning strategy if, on MIN's turn, a win is obtainable for MAX for all moves that MIN can make
MIN
• Wants to minimize the result of the utility function
• Winning strategy if, on MAX's turn, a win is obtainable for MIN for all moves that MAX can
make
Max = -∞
Min = +∞
Calculate the following:
• Complete Path
• Time Complexity
• Space Complexity

The pseudocode of MINIMAX is:
![image](https://github.com/rohit546/MiniMax-Alpha-Beta-Pruning/assets/100420859/b1cbae8a-455f-4f78-846b-a611d76a12ac)

Figure 1. Minimax Tree

![image](https://github.com/rohit546/MiniMax-Alpha-Beta-Pruning/assets/100420859/2ca7c41c-42ec-40a6-82aa-691857632ac7)



Task 2:
Exhaustively searching a game tree is not usually a good idea. We can use a branch-and-bound
technique to reduce the no. of states that must be examined to determine the value of a tree.
Branch-and-bound Technique:
• We keep track of a lower bound on the value of a maximizing node, and don’t bother
evaluating any trees that cannot improve this bound.
• Keep track of an upper bound on the value of a minimizing node. Don’t bother with any
sub-trees that cannot improve this bound.
To improve the task 1 you should implement MiniMax with Alpha-Beta pruning (prunes away search tree
nodes that are not necessary for finding an optimal solution) in a two player game. Use the same graph as
in task 1 for this task.
• At minimizing nodes, we stop evaluating children if we get a child whose value is less than the
current lower bound (alpha).
• At maximizing nodes, we stop evaluating children as soon as we get a child whose value is greater
than the current upper bound (beta).
Max = α = -∞
Min = β = +∞
α ≥ β
Calculate the following:
• Complete Path
• Time Complexity
• Space Complexity
