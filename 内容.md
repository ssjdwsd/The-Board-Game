# The-Board-Game
“Symmetry” is a new abstract strategy board game. The game rules are very simple, use the concept of symmetry, and result in a very challenging gameplay! “Symmetry” is an abstract 2-player game. Players need to create symmetrical patterns on the board to gain territory, while simultaneously preventing the opponent from creating symmetrical patterns on the board. The excact rules of Symmetry are as follows: -Black and White take turns putting stones on an NxN board (White starts). -When a stone placing causes a square on the board to be fully covered with stones, this square changes into the color of the last placed stone if the stone color pattern of the square in question has become horizontally or vertically ´mirror´ symmetric! -So ´diagonal´ symmetries will not cause any color change. -Symmetric squares can potentially have any size (2x2, 3x3, 4x4 etc). -Sometimes more than one square becomes a 'symmetry' by a move. All such squares change color. -The game ends when there are no empty fields left on the board. -The winner is the player who at the end has the most stones of their color on the board!
输入格式
从相对路径下文本文件1.in中读入双方每步走的位置。1.in的格式为：
第一行是一个正整数N，表示棋盘是N*N大小，N不大于10，其中左上角的坐标称为(1,1)，右下角的坐标称为(N,N)；
从第二行开始的N*N行，每行是黑白某一方的行棋坐标，以两个1~N之间的整数表示。白方先，白方黑方交替行棋。最终双方棋子将占满整个棋盘。
*人机对战模式下，输入格式可以自行调整。

输出格式
1、把每步运行后的棋盘依次输出到相对路径下文本文件1.out中，用1代表白棋，2代表黑棋，0代表空白。一个4*4的棋盘输出可能是这样的：
0000
0210
0120
0000
2、在打印棋盘前，要先输出一行Step n，其中n要用具体数字代入，表示当前是第几步之后的棋盘，n从1到N*N。
3、在打印棋盘后，要注明White: a  Black: b，其中a和b要用具体的数字代入，表示棋盘中有a个白子和b个黑子。
4、每张棋盘输出完后要有一行额外的空行，以与下一张棋盘间隔开。
5、当最后一步下完后，根据白子和黑子的数量，显示White Wins或者Black Wins。

输入样例（1.in的内容）
3
2 2
2 3
3 2
3 3
1 1
2 1
1 2
1 3
3 1

输出样例（1.out内容）
Step 1
000
010
000
White: 1  Black: 0

Step 2
000
012
000
White: 1  Black: 1

Step 3
000
012
010
White: 2  Black: 1

Step 4
000
022
022
White: 0  Black: 4

Step 5
100
022
022
White: 1  Black: 4

Step 6
100
222
022
White: 1  Black: 5

Step 7
110
112
022
White: 4  Black: 3

Step 8
122
122
022
White: 2  Black: 6

Step 9
111
111
111
White: 9  Black: 0

White Wins
