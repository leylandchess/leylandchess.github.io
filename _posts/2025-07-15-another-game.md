---
title: Game
layout: with-pgn
---

Example PGN display.

Some other game

{% capture pgn_text %}

[Event "Budapest"]
[Site "Budapest HUN"]
[Date "1952.03.18"]
[EventDate "1952.03.03"]
[Round "9"]
[Result "1-0"]
[White "Laszlo Szabo"]
[Black "Paul Keres"]
[ECO "E19"]
[WhiteElo "?"]
[BlackElo "?"]
[PlyCount "79"]

1.c4 Nf6 2.d4 e6 3.Nf3 b6 4.g3 Bb7 5.Bg2 Be7 6.O-O O-O 7.Nc3
Ne4 8.Qc2 Nxc3 9.Qxc3 Be4 10.Bf4 d6 11.Qe3 Bb7 12.Rfd1 Nd7
13.b4 Nf6 14.a4 Qd7 15.a5 b5 16.Ne5 dxe5 17.dxe5 Qc8 18.exf6
Bxf6 19.Rac1 Bxg2 20.Kxg2 e5 21.Bg5 Bxg5 22.Qxg5 Qb7+ 23.Kg1
Rae8 24.cxb5 Qxb5 25.Rxc7 {great move!} Qxe2 26.Qd2 Qa6 27.Qd3 Qe6 28.Rxa7
e4 29.Qe3 Rd8 30.Rxd8 Rxd8 31.Qd4 Qe8 32.Qc5 Rc8 33.Qe7 Qxe7
34.Rxe7 f5 35.a6 h5 36.a7 h4 37.Rb7 Kh7 38.Kg2 e3 39.fxe3 Rc2+
40.Kf3 1-0

{% endcapture %}



{% include pgn-board.html pgn=pgn_text %}
