# Tic-Tac-Toe Activity Flatpak

Tic-tac-toe, also known as noughts and crosses or Xs and Os, is a classic two-player game played on a 3x3 grid. The objective of the game is to be the first player to form a line of three of their symbols (either X or O) horizontally, vertically, or diagonally on the grid.

To know more refer https://github.com/sugarlabs/tictactoe

## How to build

To build this run the following command in terminal

```bash
https://github.com/SudoSu-bham/org.sugarlabs.TicTacToe.git
cd org.sugarlabs.TicTacToe
flatpak -y --user install org.gnome.{Platform,Sdk}//44
flatpak-builder --user --force-clean --install build org.sugarlabs.TicTacToe.json
```


## Check for updates
Install the flatpak external data checker

```bash
flatpak --user install org.flathub.flatpak-external-data-checker
```
To update every Single module to the latest stable version use

```bash
cd org.sugarlabs.TicTacToe
flatpak run --filesystem=$PWD org.flathub.flatpak-external-data-checker org.sugarlabs.TicTacToe.json
```
