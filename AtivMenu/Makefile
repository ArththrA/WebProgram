all: build run

build:
	@javac -d bin Main.java
	@javac -d bin aulas/*.java
	@javac -d bin libs/*.java
	@javac -d bin modelo/*.java

run: build
	@java -cp bin Main

clear:
	@rm -r bin

teste:
	#1001
	@java -cp bin Main < testes/1.in > saida.tmp
	@echo "Saida:"
	@cat saida.tmp
	@echo "Esperado:"
	@cat testes/1.out
	@rm saida.tmp

c:
	git config --global user.email ian.arthur.yw@gmail.com
	git config --global user.name Arthur

ativLista: buildL1 runL1

buildL1:
	@javac -d bin atividadeLista/Atividadelistas.java

runL1: 
	@java -cp bin atividadeLista