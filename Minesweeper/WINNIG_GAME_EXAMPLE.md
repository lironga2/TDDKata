```python
# game setup
game = Minesweeper()
game.createFeild(3,8)
game.layMine(1, 1)
game.layMine(0, 2)

# game play
game.printField();
". . . . . . . . "
". . . . . . . . "
". . . . . . . . "


game.play(0, 4)
game.printField();
". . . + + + + + "
". . . + + + + + "
". . . + + + + + "

game.play(0, 0)
game.printField();
"1 . . + + + + + "
". . . + + + + + "
". . . + + + + + "

game.play(1, 0)
game.printField();
"1 . . + + + + + "
"2 . . + + + + + "
". . . + + + + + "

game.play(0, 1)
game.printField();
"1 1 . + + + + + "
"2 . . + + + + + "
". . . + + + + + "

game.play(0, 2)
game.printField();
"1 1 1 + + + + + "
"2 . . + + + + + "
". . . + + + + + "

game.play(1, 2)
game.printField();
"1 1 1 + + + + + "
"2 . 1 + + + + + "
". . . + + + + + "

game.play(2, 2)
game.printField();
"1 1 1 + + + + + "
"2 . 1 + + + + + "
". . 1 + + + + + "

game.play(1, 2)
game.printField();
"1 1 1 + + + + + "
"2 * 1 + + + + + "
"* 2 1 + + + + + "

game.status();
"WIM"
```