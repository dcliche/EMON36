SERIAL ?= /dev/ttyACM0

all:
	rshell -p $(SERIAL) rsync . /pyboard

run: all
	rshell -p $(SERIAL) "repl ~ import eemon42 ~ eemon42.EEMON42().run() ~"

.PHONY: all run
