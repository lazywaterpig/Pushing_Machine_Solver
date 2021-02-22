=========================================

board size 8*6 (or N*M later)

Machine (not stretched): (pushing) U(up) D(down) L(left) R(right)
Machine (stretched): u(up), d(down), l(left), r(right) 
Machine (arms): A
Machine (endpoint): M

Blocks (not push-able): #
Boxes (push-able): X
Positions Boxes should be placed: -
Positions Boxes occupied: O
Positions Machines occupied: N(up/north) S(down/south) W(left/west) E(right/east) (nswe) a(machine arms) m(machine endpoint) but with positions boxes should be placed
list of positions that non-boxes occupied

Blank space: .

=========================================

Example boards(8*6):
~Difficulty=Easy(amateur-1)
#####D
##DD..
#...#.
#..X..
##..#.
##....
##RRX.
..-L.-

~Difficulty=Normal(skilled-24)
...DL#
..XWO#
..#.O#
.....#
UXR..#
...DX-
..-X.#
.##-##

~Difficulty=Hard(impossible-1)
##D###
#DX###
#..-..
-XRL..
#RN#X#
#...X-
#UXOO#
##-###

=========================================

class board(box pos/num machine pos/num(not useless))
isimpossibletosolve
isdeadlocked(2*2)
isreducible(deadlocked with positions that boxes occupied)
isdeadlocked(no more boxes/machines that each can push)
ispushable
issolved
ispossibletosolve
possiblemovechecker
possiblemovelister

