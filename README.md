### Neste repositório conterá minhas anotações sobre Programação Orientada a Objetos.

---

Na programação existem alguns paradigmas que são adotados, visando otimizar o processo de desenvolvimento de softwares. Em geral, aprende-se a programar utilizando o paradigma estruturado, ou seja, o código sequencial, escrito com pouco ou nenhum reaproveitamento de determinados sub-algoritmos (salvo pelas funções).

Embora existam alguns paradigmas amplamente utilizados dentro da computação, indubitavelmente aquele que tem mais aderência do mercado é a Programação Orientada a Objetos, conhecida também como POO.

A maior parte das linguagens de programação tem uma estrutura voltada à Orientação a Objetos e o Python é uma delas. Veremos no decorrer deste módulo algumas vantagens de se utilizar a programação orientada a objetos no desenvolvimento de softwares, bem como, conheceremos algumas características e peculiaridades do Python quanto a este paradigma.

---

### POO E SUAS VANTAGENS

O GRANDE CORAÇÃO DA PROGRAMAÇÃO ORIENTADA A OBJETOS: CLASSES, MÉTODOS E ATRIBUTOS

No módulo de funções deste material, você deve ter percebido algumas vantagens de se reaproveitar determinados trechos de código na escrita de algoritmos mais complexos. Alguns motivos podem ser elencados sem muita dificuldade.

A POO vem ao encontro deste mesmo objetivo e possibilitará ao desenvolvedor duas grandes vantagens. A primeira delas, claro, é o reaproveitamento de código. A segunda é a segurança da aplicação (VOCÊ CONSEGUE ENCAPSULAR/VETAR ACESSO A DETERMINADAS ÁREAS DO SEU CÓDIGO / VETAR ALTERAÇÃO DE CONTEÚDOS)

Este critério de segurança da aplicação é um tanto relativo em Python, pois a base de segurança - o encapsulamento, conforme veremos adiante - é tratado de modo diferente se comparado a linguagens mais engessadas como o Java, porém, isso não é um demérito da linguagem, pelo contrário, isso é uma forma de dar maior autonomia ao programador e confiar em seu bom senso de desenvolvedor.

TEMOS UMA ESTRUTURA ONDE PRECISAMOS CADASTRAR UMA DETERMINADA PESSOA EM UM SISTEMA DE ESCOLA:

E DA MESMA FORMA ESSE ALUNO TEM ESSES DADOS: NOME, E-MAIL, CPF, TAMBÉM TEM ALGUMAS AÇÕES QUE ELE PODE EXECUTAR, COMO FAZER MATRÍCULA (SE MATRICULAR).

CASO VOCÊ TENHA 1.000 ALUNOS, VOCÊ TERÁ QUE REPLICAR AS VARIÁVEIS PARA ESSES 1.000 ALUNOS (SE VOCÊ TEM 1.000 ALUNOS, VOCÊ TERÁ 1.000 VARIÁVEIS DE NOMES / 1.000 VARIÁVEIOS DE E-MAILS / 1.000 VARIÁVEIS DE CPF / 1.000 AÇOES DE MATRICULAR).

E O SISTEMA COMEÇA A FICAR COMPLEXO,PRINCIPALMENTE SE VOCÊ PRECISAR FAZER UMA ALTERAÇÃO DEPOIS, PORQUE VOCê NÃO FARÁ ESSA ALTERAÇÃO EM APENAS 1 ALUNO, MAS VOCÊ TERÁ QUE REPLICAR PARA TODOS OS 1.000 ALUNOS)

A POO VEM JUSTAMENTE PARA RESOLVER ESSE TIPO DE PROBLEMAS, VOCÊ CRIA UM MOLDE (UMA ESTRUTURA PADRÃO) QUE TERÁ 1 NOME, 1 E-MAIL, 1 CPF E 1 MATRÍCULA.

E PARA CADA ALUNO QUE VOCÊ FOR ADICIONAR DENTYRO DO DITEMA, VOCÊ IRÁ CRIAR O ALUNO 1 E FALA QUE ELE PERTENCE A ESSE MOLDE, CRIA O ALUNO, 2 , 30 OU 1.000 ALUNOS VOCÊ TERÁ APENAS 1 MOLDE PADRÃO QUE VOCÊ IRÁ REPLICAR PARA TODOS AQUELES ALUNOS E VOCÊ ESTARÁ ECONOMIZANDO MAIS DE 1.000 VARIÁVEIS.

RESUMINDO, VOCÊ ESTARÁ USANDO POR PADRÃO 1 MOLDE QUE SERÁ REPLICADO PARA TODOS OS ELEMENTOS QUE UTILIZAREM AQUELA MESMA ESTRUTURA PADRÃO.

---

### CLASSES, MÉTODOS E ATRIBUTOS

As classes fornecem um meio de agrupar dados e funcionalidades. A criação de uma nova classe cria um novo tipo de objeto, permitindo que novas instâncias desse tipo sejam feitas. Cada instância de classe pode ter atributos anexados a ela para manter seu estado. As instâncias de classe também podem ter métodos (definidos por sua classe) para modificar seu estado. (Python.org).

Em outras palavras, as classes são formas de se agrupar informações que são do mesmo tipo dentro de um escopo 

Animal

Atributos
Nome

Métodos
Comer

Temos uma classe chamada Animal. Esta classe pode ser considerada uma classe abstrata, uma vez que é genérica o suficiente para se adequar a qualquer tipo de animal, veja:

Todo animal tem um nome
Todo animal tem um tipo (ave, mamífero) - Atributos
Todo animal pode comer - Método

Desta forma, quando criamos um molde genérico que pode ser adaptado a qualquer objeto que o utilize, temos uma classe abstrata que passará, futuramente, dados às classes específicas.

Uma característica inerente às classes é o fato de começarem sempre com letra maiúscula. Isso não interfere propriamente no funcionamento da classe (na maioria das linguagens), mas para que seja seguida uma convenção, ou seja, um “acordo de consenso da comunidade de desenvolvedores”, adota-se o mesmo padrão. Desta forma, sempre que escrever o nome de uma classe, seja ela abstrata ou não, utilize a inicial maiúscula.

### PARA UM ARQUIVO ENXERGAR O OUTRO, PRECISO FAZER A IMPORTAÇÃO DO ARQUIVO. (PARA ISSO, USAREMOS O COMANDO DE IMPORT)

from Pessoa import Pessoa

AGORA QUE OS ARQUIOS ESTÃO CONECTADOS ENTRE SI, CONSEGUIMOS PUXAR INFORMAÇÕES QUE ESTÃO LÁ NO ARQUIVO PESSOA, DENTRO DO ARQUIVO TESTE.

E PARA CONSEGUIR 

1:20



---

POR CONVENÇÃO, SEMPRE QUE CRIAMOS UMA CLASSE, ELA IRÁ INICIAR COM A LETRA MAIÚSCULA E QUANDO TIVER MAIS DE 1 PALAVRA, COLOCAMOS A INICIAL DE CADA PALAVRA EM MAIÚSCULO.

NA PRÁTICA, ISSO NÃO FARÁ DIFERENÇA A NÍVEL FUNCIONAL, MAS SIM A NÍVEL DE CONVENÇÃO.

CONVENÇÃO É UM ACORDO QUE EXISTE MUNDIAL PARA QUE TODA CLASSE SEJA FEITA DESSA FORMA.

E É QUANDO UMA COMUNIDADE DE DESENVOLVEDORES CHEGARAM A UM CONCENSO DE QUE FAZER UMA CLASSE TEM QUE SER DESSE JEITO.

---

CRIAREMOS UMA CLASSE CHAMADA PESSOA, E DENTRO DA ESTRUTURA DESSA CLASSE PODEMOS TER QUALQUER INFORMAÇÃO, ONDE TEREMOS MÉTODOS E ATRIBUTOS.

ATRIBUTOS = VARIÁVEIS

CADA PESSOA PODE TER UM NOME, CPF, E-MAIL, ... SENDO ELES CARACTERÍSTICAS/SUBSTANTIVOS OU ADJETIVOS RELATIVOS AQUELA PESSOA. COR DE CABELO/IDADE/SEXO, ...

SÃO ESSES ATRIBUTOS QUE SÃO VARIAÉVEIS QUE COLOCAREMOS.

class Pessoa:
    nome = ""
    idade = 0

MÉTODOS SÃO AS AÇÕES QUE UMA CLASSE PODE EXECUTAR ATRAVÉS DO SEU OBJETO.

UMA PESSOA PODE SE MATRICULAR. ESSAS AÇÕES QUE GERALMENTE SÃO VERBOS, QUE CHAMAMOS DE MÉTODO E TODO MÉETODO É UMA FUNÇÃO.

E TODA FUNÇÃO COMEÇA COM A PALAVRA def.

POR PADRÃO, QUANDO VOCê TEM UM MÉTODO, OU VOCÊ SIMPLESMENTE O CHAMA EXECUTANDO ALGUMA COISA MAS SEM RECEBER NENHUM VALOR (print("texto")) - estou imprimindo um valor que não depende de um valor que virá de fora.

OU VOCÊ USA VALORES PADRÕES DAQUELA CLASSE.







