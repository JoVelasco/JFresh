#Makefile for JFresh by Christian Daley
CC = gcc
ifeq ($(BUILD),debug)
CFLAGS = -g -Wall
else
CFLAGS = -Ofast -DNDEBUG
endif

all: JFresh

JFresh: main.o Attack.o Bitmask.o Bitscan.o Board.o Debug.o Eval.o Fen.o History.o Killer.o Log.o MagicMoves.o MagicNumberGen.o Move.o MoveGen.o Perft.o Search.o SearchOptions.o SearchResults.o Sort.o Thread.o TT.o Uci.o UciOptions.o Undo.o
	$(CC) $(CFLAGS) -o JFresh main.o Attack.o Bitmask.o Bitscan.o Board.o Debug.o Eval.o Fen.o History.o Killer.o Log.o MagicMoves.o MagicNumberGen.o Move.o MoveGen.o Perft.o Search.o SearchOptions.o SearchResults.o Sort.o Thread.o TT.o Uci.o UciOptions.o Undo.o

clean:
	$(RM) JFresh *.o *~

debug:
	make "BUILD=debug"