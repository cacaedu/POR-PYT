
## Do Português para o Pythonês* <br><br> <sup ><sup>*neologismo do autor</sup></sup>
Aprender uma linguagem de programação, seja ela qual for, é quase sempre, intimidante e desafiador. Isso é natural e perfeitamente normal diante de algo novo para a nossa cultura e para o nosso cérebro.

Quando nos deparamos com algo que não conhecemos, a dúvida, a incerteza e o medo do desconhecido podem bloquear oportunidades de aprendizagem relevantes. É o caso de aprender uma nova linguagem, especialmente uma linguagem de programação que, além do núcleo comum de qualquer linguagem – símbolos, léxico, sintaxe e semântica –, tem um paradigma claro de lógica formal que deve ser aprendido.

Deixando o medo e as incertezas de lado, vamos tentar uma estratégia que pode ser interessante, de algum modo prazerosa e, até, divertida, para aprender uma linguagem de programação: vamos escrever os nossos "códigos" em linguagem natural (um idioma, no nosso caso o Português) e transformá-la em uma linguagem de programação com suas estruturas de dados, lógica etc. A linguagem de programação escolhida é Python. Essa linguagem é tida, por muitos, como a mais simples e de sintaxe mais limpa para o aprendizado de programação. Vamos começar?    

Python é uma linguagem orientada a objetos. Mas o que isso significa? Pense em um objeto. Por exemplo, um carro. Um carro é um objeto que pode exercer ações (funções) e que tem características próprias (propriedades), certo? Vamos listar algumas ações/funções e características/propriedades que um carro pode ter na tabela a seguir.

  |Ações|Propriedades|                       
  |:--------------|--------------|
  |Acelerar        |     Modelo  |
  |Brecar     |Cor       | 
  |Dar ré     |Marca      | 
  |Virar|  Ano de fabricação|

Então, de acordo com a tabela acima, podemos dizer que o objeto carro tem uma função chamada acelerar. Como dizemos isso em Pythonês? Assim: carro.acelerar(). Estranho? Escrevendo desse modo, estamos chamando a função acelerar() - as funções têm parênteses – do objeto carro através do ponto (.). Em Pythonês, pense no ponto como "acessar algo do objeto". Ou seja, estamos dizendo ao Pyhton "Ei, eu quero acessar/usar a função acelerar() do objeto carro". Quando fazemos isso, o código que escrevemos nos retorna o que essa função quer retornar ou nos mostrar como resultado. Como sabemos o que ela quer retornar? Bem, com o carro real, o retorno seria ele se mover mais rapidamente, não é isso? Vamos, então, simular o “se mover mais rapidamente” com um texto que precisa, além de ser retornado, mostrado de algum modo, ou seja, precisamos ver esse retorno na forma de texto. Fazemos isso com a função print() desse modo: print(carro.acelerar()). O que essa linha com uma função print() fará?

Print é uma função (print()) embutida ou incorporada ao Python que nos mostra (retorna) o que estiver dentro do parênteses (lembre-se que as funções têm parênteses. Esse é um modo de reconhecê-las e fazê-las funcionar). Então, print(carro.acelerar()) deve nos mostrar o retorno da função acelerar do objeto carro. Como vamos simular isso com um texto? Digamos que esse retorno seja “Estou acelerando agora”, indicando que a função está funcionando e deu o retorno esperado.

Desse modo, print(carro.acelerar()) mostrará o texto “Estou acelerando agora” sem as aspas. Veja o código (do Português ao Pythonês) abaixo.

Português: Acelere o carro e mostre que ele está acelerando
Pythonês: 
1. Acelere é uma ação, portanto deve ser representada por uma função. Funções devem iniciar com a palavra-chave def (de definition). Isso diz ao Python que o que vem a seguir é uma função, desde que tenha os parênteses no final. Então, criaremos a função acelerar primeiro e, na sequência, a chamaremos dentro da função print.
```
def acelerar():
	return "Estou acelerando agora"
	
print(acelerar())
```
Depois dos parênteses, devemos colocar dois pontos para mostrar ao Python que, depois deles, haverá um bloco (o bloco da função) que deve ser indentado (tabulado) com alguns espaços - normalmente quatro - para delimitar o bloco (tudo que estiver indentado fará parte do bloco)

A palavra-chave ```return``` é a responsável por retornar/mostrar o que a função tem de retornar quando ela for chamada. Para chamar uma função em Pythonês usa-se o nome da função seguido dos parênteses: acelerar().

Copie e cole este código [neste editor Python online](https://trinket.io/) e, em seguida, clique no botão play para ver o resultado a direita. Para fazer isso, delete o conteúdo de uma das duas abas disponibilizadas (Main.py e Shape.py) e, em seu lugar, cole o código da função e a sua chamada)Não é necessário fazer login para, apenas, testar códigos Python nesse site (Trinket).

Vamos nos aprofundar nisso. Um objeto tem funções e propriedades como vimos. Mas, onde elas estão? Onde elas foram escritas ou determinadas? Onde foi escrito esse retorno "Estou acelerando agora"? Em algo chamado classe. Aí vem a pergunta: o que é uma classe? A classe é a estrutura, o molde, o modelo que cria as funções e as propriedades que serão acessadas pelo objeto criado a partir dela. Confuso? Criamos objetos a partir de classes, assim como se criam carros a partir de fábricas. As fábricas têm os modelos, as regras a serem seguidas para fabricar os carros, assim como as classe têm as funções e as propriedades necessárias para criar objetos, como o nosso carro. Vamos criar a nossa “fábrica”, ou melhor, a nossa classe que cria carros em Python.

## Definição das características (propriedades) e funções de um carro

Primeiro, vamos escrever em Português para, depois, passarmos para o Pythonês:

Classe Carro --> o modelo com as instruções de “fabricação”.
1.  Inicie a produção com os parâmetros (não argumentos) cor, marca e modelo.

2. Defina uma função para simular o movimento do carro para frente (“andar”)

  
  

Passemos para o Pythonês com suas regras sintáticas:

class Carro:

def __init__(self, cor, marca, modelo):

self.minha_cor = cor

self.minha_marca = marca

self.meu_modelo = modelo

def andar(self):

return “Eu estou ‘andando’ para frente!”

  
  

Vamos, agora, comparar as duas instruções (Pythonês com explicações em Português):

  
  

class Carro: (isso define a classe Carro)

def __init__(self, cor, marca, modelo): (isso começa a “produção” do carro a partir da definição dos parâmetros escolhidos, onde self representa o carro a ser “fabricado” – veremos isso já já)

self.minha_cor = cor

self.minha_marca = marca

self.meu_modelo = modelo

def andar(self):

return “Eu estou ‘andando’ para frente!”



<!--stackedit_data:
eyJoaXN0b3J5IjpbODMxNzkyNTc2LDE1ODgwNTMzNTcsLTEzOT
g2MTQyMCwtODA5NTcxOTYzLDM3NTk3NjQ2OCwxNDE1MDM1NjU2
LDc4OTk2MTIyNiw1NjQ4OTY4MjgsNTY0ODk2ODI4LC0zMDAxNz
MzMzUsLTEzNjkzMDM3MDRdfQ==
-->