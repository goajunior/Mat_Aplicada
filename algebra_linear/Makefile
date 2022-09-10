#!/bin/sh

all: build release

build:
	pdflatex -interaction=nonstopmode main.tex

projectname = $(shell pwd|awk -F'/' '{print $$NF}' )
# projectname = $(shell pwd | awk -F'/' '{print $NF}')

release:
	(cp main.pdf ../release/$(projectname).pdf)
