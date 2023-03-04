JAVACC=javacc
JAVAC=javac
JAVA=java
ifeq ($(OS),Windows_NT)
	# Comando para Windows
	RM = del /Q
else
	# Comando para Linux e macOS
	RM = rm -f
endif

.SUFFIXES: .jj .java .class

.jj.java:
	$(JAVACC) $*.jj

.java.class:
	$(JAVAC) $*.java

LEXER=Ruby
TEST_FILE=$(word 2,$(MAKECMDGOALS))

.PHONY: all clean run

all: $(LEXER).class

run: $(LEXER).class
	$(JAVA) $(LEXER) $(TEST_FILE)

clean:
	$(RM) *.class
	$(RM) *.java
