---
title: Setting Up an Integrated Development Environment for Python (Mac)
layout: lesson
date: 2012-07-17
authors:
- William J. Turkel
- Adam Crymble
reviewers:
- Jim Clifford
- Amanda Morton
editors:
- Miriam Posner
difficulty: 1
exclude_from_check:
  - review-ticket
activity: transforming
topics: [get-ready, python]
abstract: "Esta lição irá lhe auxiliar a configurar um ambiente de desenvolvimento integrado para o Python em um computador com o Sistema Operacional Mac."
redirect_from: /licoes/instalacao-mac
avatar_alt: Uma banda com três músicos
doi: 10.46430/phen0012
---

{% include toc.html %}





### Faça um backup do seu computador

É sempre importante garantir que você tenha backups regulares e recentes do seu computador. Este é um bom conselho que serve para a vida toda, e não se limita à pratica específica de programação. Usuários do Mac podem recorrer ao [Time Machine][] para isso.

### Instale o Python 3

Você ainda pode ter o Python 2 na sua máquina. Como essa versão do Python será descontinuada no fim de 2019, é importante que você instale o Python 3. Faça o download da versão mais estável da linguagem de programação Python (Version 3.8 de Novembro de 2019) e instale o software a partir do [Site do Python][].

### Crie um directório

Para que você se organize, o ideal é que você tenha um diretório (i.e., pasta) no seu computador onde você irá armazenar os seus programas em Python (por exemplo, `programming-historian`). Crie esse diretório em qualquer área do seu computador.

### Instale um editor de textos

Existem vários editores de texto que você pode utilizar para escrever, armazenar e executar comandos em Python. O Komodo Edit é o utilizado nesta lição, correspondendo a um editor gratuito e de código aberto. Se você prefere utilizar outro editor, existem [outros editores][]. Por exemplo, alguns dos nossos colaboradores preferem o programa [TextWrangler][]. Você pode escolher qual editor utilizar mas, para manter a consistência entre as lições, nós iremos utilizar o Komodo Edit. Você pode fazer o download do Komodo Edit diretamente do [Website do Komodo Edit][]. Faça a instalação a partir do ficheiro `.DMG`


#### Faça um comando “Run Python” no Komodo Edit

Deve agora configurar o editor para que seja possível executar programas em Python.

Se você não visualizar a barra de ferramentas (Toolbox) do lado direito, selecione a opção do menu `View -> Tabs -> Toolbox`. Na janela Toolbox, clique no ícone da engrenagem e selecione “`New Command…`“. Uma nova janela de diálogo irá abrir e você deve renomear o seu comando para “`Run Python`”. Fique a vontade para alterar também o ícone. Na caixa “`Command`”, digite:

``` python
%(python3) %f
```

e na aba de opções avançadas, sob o texto "Start in," digite:

``` python
%D
```

Cique no botão OK e o seu novo comando "Run Python" deve aparecer no painel de ferramentas.

## Passo 2 – “Olá Mundo” em Python
--------------------------------

É uma tradição para quem está começando a programar em uma nova linguagem que o primeiro programa a ser construído emita a frase "Olá Mundo". 

O Python é uma boa linguagem de programação para iniciantes porque ela é de alto-nível.
Isto quer dizer que é possível escrever pequenos programas que realizam muitas funcionalidades. 
Quanto menor o programa, mais provável que ele caiba em apenas um ecrã, e mais fácil será manter o controle dele em sua mente.

O Python é uma lingugagem 'interpretada'. Isto significa que existe um programa especial (conhecido como Interpretador) que sabe como seguir as instruções da linguagem. Uma forma de utilizar o interpretador é guardar todas as instruções a executar em um ficheiro para, em seguida, solicitar ao interpretador que ele interprete o conteúdo desse ficheiro.  

Um ficheiro que contém instruções de linguagem de programação é conhecido como um programa. O interpretador irá executar cada uma das instruções que você incluiu no seu programa e no final irá parar. Vamos experimentar como isto funciona.

No seu editor de texto, crie um novo ficheiro, entre o seguinte programa de duas linhas, e salve-o na pasta `programming-historian`:
 
`ola-mundo.py`

``` python
# ola-mundo.py
print('Olá Mundo')
```

O comando “*Run Python File*” permite que você execute o seu programa.
Se você escolheu um outro editor, este deve ter uma funcionalidade semelhante.
Se tudo correu bem, o ecrã deverá mostrar algo como apresentado de seguida (Clique na imagem para ver uma imagem maior):

![TextWrangler-hello-world](https://raw.githubusercontent.com/programminghistorian/jekyll/bc4c0f1398f54adb1add6bb156756212c28e8f78/images/TextWrangler-hello-world.png)
“Alô Mundo” em Python no Mac

## Interagindo com a linha de comandos do Python

Uma outra forma de interagir com o interpretador é utilizar o que é denominado por linha de comandos. Você pode digitar um comando na linha de comandos e pressionar a tecla Enter, sendo-lhe apresentada a resposta ao seu comando. Usar a linha de comandos é um ótimo método para testar os comandos, por forma a certificar que eles realmente fazem o que você está imaginando.

Abra o Finder, faça duplo-clique em `Applications -> Utilities -> Terminal` e, em seguida, digite “`python3`” 

Este comando irá abrir a linha de comandos do Python, indicando assim que você já pode executar comandos Python. De seguida, digite:

``` python
print('Olá Mundo')
```
e pressione Enter. O computador irá responder com:

``` python
Olá Mundo
```

Quando quisermos representar uma interação na linha de comandos, utilizaremos o símbolo `->` para indicar a resposta para o nosso comando, tal como no exemplo abaixo:

``` python
print('Alô Mundo')
-> Alô Mundo
```

No seu ecrã, você verá algo como:

![Ola Mundo no Mac](https://raw.githubusercontent.com/programminghistorian/jekyll/bc4c0f1398f54adb1add6bb156756212c28e8f78/images/hello-world-terminal.png)
Shell do Python no Terminal do Mac

Agora que você e o seu computador estão preparados, podemos seguir para tarefas mais interessantes. Se você está seguindo as lições do Python, a nossa sugestão é que tente a próxima aula ‘[Noções básicas de páginas web e HTML][]‘

  [Time Machine]: http://support.apple.com/kb/ht1427
  [Site do Python]: https://www.python.org/downloads/mac-osx/
  [Beautiful Soup]: http://www.crummy.com/software/BeautifulSoup/
  [outros editores]: https://wiki.python.org/moin/PythonEditors/
  [TextWrangler]: http://www.barebones.com/products/textwrangler/
  [Komodo Edit website]: http://www.activestate.com/komodo-edit
  [Understanding Web Pages and HTML]: /licoes/visualizando-arquivos-html
