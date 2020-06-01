# Ghidra

## O que é?

O Ghidra é uma ferramenta open source para a engenharia reversa feita pela agência de segurança nacional dos EUA \(NSA\) e disponibilizada para o público em 2019.

A ferramenta pode ser baixada pelo [site oficial ](https://ghidra-sre.org/)ou pelo [github](https://github.com/NationalSecurityAgency/ghidra), onde parte do código se encontra.

Uma das grandes vantagens do IDA é a ferramenta de _decompile_, que permite que seja visualizado um código "descompilado" de um binário. Essa ferramenta suporta diversas arquiteturas nativamente e existem alguns plugins para adicionar suporte de outras.

Usualmente os binários que serão analisados vão ser das linguagens C/C++, mas também é possível analisar por exemplo binários escritos em Golang, análise que funciona melhor caso tenha plugins específicos para isso.

O Ghidra funciona tanto para Linux como para Windows \(p/ Mac também\), sem alterações significativas no seu funcionamento básico.

## Criando um novo Projeto

A tela inicial do ghidra é algo semelhante à tela a seguir:

![](../.gitbook/assets/image%20%281%29.png)

Para criar um novo projeto basta selecionar a opção de novo projeto e criar um não compartilhado \(dado que a versão compartilhada é feita para ser usada por múltiplos usuários simultaneamente em um servidor\), escolher um nome, caminho e criar.

Vai ser criada uma pasta, então você arrasta um binário ou o importa \(tecla de atalho i\). O formato tende a ser identificado automaticamente, então basta confirmar as seleções, onde uma nova tela vai abrir com diversas informações sobre os metadados do executável. Abra o codebrowser \(ou clique 2 vezes no executável\) e vá para a tela inicial.

Quando iniciar, clique em analisar para que seja possível obter informações do binário de forma automática. Recomendamos dar uma olhada em cada uma das opções e tentar entender o que elas significam, mas para um uso básico basta deixar tudo na opção padrão.

Uma das janelas mais importantes do programa encontra-se na esquerda, que é onde estarão listadas as funções. Procure pela main ou por funções interessantes, quando selecionar a função que quiser ela automaticamente vai aparecer na tela.

![Janela de s&#xED;mbolos, onde encontram-se as fun&#xE7;&#xF5;es](../.gitbook/assets/image%20%282%29.png)

![O disassembly na tela da esquerda e o c&#xF3;digo decompilado na tela da direita](../.gitbook/assets/image%20%283%29.png)

As hotkeys estarão na cheatsheet abaixo, mas já saiba que as mais importantes agora no início são L, que serve para renomear objetos selecionados e Ctrl+L, para ajeitar um tipo. \(Por exemplo representar várias variáveis seguidas como um vetor\)

Clicando duas vezes em uma função entra-se no código dela e Alt+Left volta para o local anterior.  
Caso queira desfazer alguma operação, o clássico Ctrl+Z é utilizado.

## Cheatsheet


