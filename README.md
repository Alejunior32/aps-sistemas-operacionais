# Sistemas Operacionais Atividade Prática - APS

### Objetivo

O objetivo do trabalho é escrever um programa para mostrar o funcionamento dos algoritmos de alocação de processos em memória, utilizando o modelo de alocação contigua em
partições dinâmicas, conforme foi visto em aula.

### Descrição

Este projeto envolve a construção de um simulador de alocação de processos em memória utilizando alocação contigua com partições dinâmicas.

Seu simulador deve receber como entrada:

1) Tamanho inicial dos blocos de memória, na ordem em que devem ser considerados, ou seja, do início para o final da memória

2) Sequência dos processos a serem alocados, na ordem que serão processados. Cada processo receberá um nome quando lido.

A entrada será feita por meio de um arquivo texto contendo os dados para execução. O arquivo deverá se chamar “entrada.txt” (não altere o nome do arquivo) e conter duas linhas obedecendo o seguinte formato:

Linha 1: Lista de blocos de memória livres, separados por “;”
Linha 2:Lista de processos (tamanho) separados por “;”

As linhas são uma lista de valores inteiros apenas, representando os tamanhos.

Exemplo de arquivo:

100;500;200;300;600
210;410;110;220

Ao ser lido o processo, o mesmo receberá um nome único para ser identificado (P1, P2, P3, etc.). Ao final da execução o simulador deve fornecer:

1) Lista com os blocos de memória ainda disponíveis para alocação,destacando o maior, o menor e a média de tamanho dos blocos livres. OBS: Um bloco de tamanho zero não deve ser considerado livre e por isso não pode entrar nesta contabilidade.
2) Lista de processos alocados (por nome: P1, P2, etc)
3) Lista de processos não alocados (por nome: P1, P2, etc.)
