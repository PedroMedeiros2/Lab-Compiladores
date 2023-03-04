
# Analisador Léxico Ruby

Este programa de computador tem como objetivo analisar a estrutura léxica de um programa escrito na linguagem Ruby. Com o uso de um gerador automático de parser léxico JavaCC, o programa é capaz de identificar todas as unidades léxicas (lexemas/tokens) da linguagem Ruby, tornando mais fácil a compreensão da estrutura sintática do programa em questão.

## Como utilizar

Para utilizar o analisador léxico Ruby, siga os passos abaixo:

1.  Faça o download do código fonte do programa.
2.  Certifique-se de ter o JavaCC e o JDK instalados em sua máquina.
3.  Abra o terminal e navegue até o diretório onde o código fonte foi baixado.
4.  Execute o comando `make` para gerar os arquivos .java necessários para o programa.
5.  Execute o comando `make run <arquivo>` para realizar a análise léxica do arquivo de entrada. Substitua `<arquivo>` pelo nome do arquivo que deseja analisar.
6.  Execute o comando `make clean` para remover os arquivos .class gerados durante a compilação.

## Arquivos

-   `Ruby.jj`: arquivo de definição do parser léxico JavaCC.
-   `Token.java`: classe que representa os tokens da linguagem Ruby.
-   `TokenMgrError.java`: classe de exceção utilizada pelo parser léxico.
-   `Ruby.java`: classe principal que realiza a análise léxica do programa de entrada.

## Licença

Esse programa é licenciado sob a MIT License.