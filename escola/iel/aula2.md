---
title: Grandezas elétricas
header-includes:
  - \usepackage{asmath}
---

1. [Grandezas elétricas](#grandezas-elétricas)
   * [Unidades](#unidades)
   * [Corrente elétrica](#corrente-elétrica)
     * [Correntes contínuas ou varíaveis](#correntes-contínuas-ou-varíaveis)
   * [Efeito de Joule](#efeito-de-joule)
   * [Resistência](#resistência)
     * [Resistivade](#resistivade)
   * [Lei de Joule e Lei de Ohm](#lei-de-joule-e-lei-de-ohm)
   * [Força eletromotriz](#força-eletromotriz)
   * [Potência](#potência)
     * [Fornecer/Receber potência](#fornecer/receber-potência)
   * [Circuitos](#circuitos)
   * [Ligações](#ligações)
     * [Série](#série)
     * [Paralelo](#paralelo)

## Grandezas elétricas

Introdução às principais grandezas elétricas.

### Unidades
- Intensidade, A (Ampere);
- Potência, W (Wat);
- Resistência, $$\Omega $$ (ohm);

### Corrente elétrica

Unidade:
- Ampere, A.

Definiu-se a __intensidade de corrente__, $$I$$, como a __quantidade de carga 
elétrica ($$\Delta Q$$) que atravessa a superfície do condutor__, colocada 
normalmente à direção do movimento da carga, por unidade de tempo($$\Delta t$$).

$$
I = \frac{\Delta Q}{\Delta t}
$$

O sentido da corrente é do __terminal positivo para o terminal negativo__, sendo
contrário ao movimento real dos eletrões.

#### Correntes contínuas ou varíaveis

Naturalmente podemos ter correntes contínuas (ou constantes) ou correntes 
variáveis no tempo.
- Um tipo particular de correntes varíaveis no tempo são as sinusoidais, 
normalmente chamadas de correntes alternadas sinusoidais.

Se a corrente variar no tempo, temos de considerar a corrente em instantes 
específicos:

$$ 
I(t) = \frac{dQ}{dt}
$$

### Efeito de Joule

Uma corrente ao percorrer um condutor vai provocar o aquecimento do mesmo.
A este fenómeno é dado o nome de __efeito de Joule__.

A potência dissipada, $$P$$, sob a forma de calor num condutor dá-se por:

$$
P = RI^e
$$

Sendo $$R$$ a resistência de cada condutor.

### Resistência

A resistência de cada material representa a maior ou menor dificuldade de 
passagem de corrente nesse mesmo material.

Dado um condutor de comprimento $$l$$ e secção $$S$$ (secção é a área da 
superfície do condutor se cortado perpendicularmente ao seu comprimento):

$$
R = \rho \frac{l}{S}
$$

$$\rho$$, é a resistividade de dado material.

Tabela de resistências:


![Tabela de resistências](../../res/iel/resistencias.png)
#### Resistivade

A caraterística condutora de cada material pode ser dada por $$\rho$$, ou o
seu inverso $$\gamma$$.

A resistividade de cada material varia também com a temperatura:

$$
\rho (\theta) = \rho_{20ºC}[1+\alpha (\theta - 20ºC)]
$$

$$\alpha$$ sendo o coeficiente de temperatura do material.

Na maioria dos materiais a resistividade aumenta com a temperatura.

### Lei de Joule e Lei de Ohm

Lei de Joule:

$$P = RI^2$$

Lei de Ohm:

$$V = RI$$

### Força eletromotriz

Define-se pela energia produzida pela fonte no seu interior por unidade de 
carga:

$$E = \frac{W_p}{Q}$$

Tem o sentido coincidente da corrent, ou seja o inverso da Resistência.

### Potência

É a razão entre a energia fornecida/consumida no aparelho e o tempo gasto nessa
ação.

Usando a lei de Joule e a lei de Ohm, podemos derivar três fórmulas para 
potência:

$$
P=VI\\
P=\frac{V^2}{R}\\
P=RI^2
$$

#### Fornecer/Receber potência

Sabemos que um dispositivo está a fornecer potência quando, $$P=VI<0$$.

Sabemos que um dispositivo está a receber potência quando, $$P=VI>0$$.

### Circuitos

Elemento ativo - Fornece energia  
Elemento passivo - Gasta energia  

### Ligações

#### Série

Um circuito é em série se todos os componentes são percorrridos pela mesma corrente.

Os elementos em série constituem um __ramo__.

Um conjunto de ramos chama-se __malha__.

#### Paralelo

Dois ou mais elementos estão ligados em paralelo se todos estão sujeitos à mesma
tensão ou diferença de potencial.

Chama-se nó ao ponto em que se ligam 3 ou mais ramos.



