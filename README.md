# ACMQ-HK
O programa HK obtém aproximações para filtros analógi- cos contínuos de vários tipos, usando o método clássico de aproximação usando a função de transdução H(s) e a função característica K(s).

http://www.coe.ufrj.br/~acmq/programs/

O programa HK obtém aproximações para filtros analógi-
cos contínuos de vários tipos, usando o método clássico de
aproximação usando a função de transdução H(s) e a função
característica K(s).
Na notação adotada, a função característica é definida
por
 K(s)=F(s)/P(s), e a função de
 transdução
 por
H(s)=E(s)/P(s). onde F(s), E(s) e P(s) são polinômios com
coeficientes reais. K(s) e H(s) são associadas pela equa-
ção de FeldtKeller: H(s)H(-s)=1+K(s)K(-s), ou E(s)E(-
s)=F(s)F(-s)+P(s)P(-s). Desta forma, |H(jw)| é a atenuação
do filtro, e a função de transferência desejada vale
T(s)=k/H(s), onde k depende da forma de realização. Os
pólos da função de transferência T(s) são as raízes de
E(s), e seus zeros, os zeros de transmissão, são as raízes
de P(s). As raízes de F(s) são os zeros de atenuação.
Apenas aproximações tipo passa-baixas podem ser direta-
mente construídas pelo programa, mas é possível transfor-
má-las depois para outras formas. Em todos os cálculos, o
programa assume aproximações normalizadas, com corte ou
frequência central em 1 rad/s.
Dada K(s), o programa calcula H(s), ou dada H(s), o
programa calcula K(s). Os polinômios necessários, F(s) e
P(s) ou E(s) e P(s), podem ser fornecidos ao programa
usando-se a opção de ler polinômio, ou calculados pelo
prαprio programa, nos casos de alguns tipos particulares
de aproximação. K(s) é calculada diretamente para quatro
tipos de aproximação em que K(jw) é puramente real, e é
obtida a partir de um polinômio característico Q(w). H(s)
é calculada diretamente para a aproximação de Bessel.
Aproximações polinomiais, onde K(jw)=εQ(w), incluem as
aproximações de Butterworth e Chebyschev. O parâmetro ε
define a atenuação na banda passante. A aproximação é
obtida a partir do polinômio característico Q(w), e o
programa gera os polinômios adequados para aproximações de
Butterworth (Q(w)=wn), Chebyschev (Q(w)=Cn(w)) e Chebys-
chev modificada (Q(w)=CMn(w)), que é Cn(w) com menores
raízes movidas para a origem por uma transformação de
Moebius) polinômios, que levam a aproximações intermediá-
rias entre estes extremos, podem ser gerados pelo programa
APOL, e lidos pelo programa.
Aproximações
 polinomiais
 inversas,
 onde
K(jw)=εα2
wn/Qr(w) e Qr(w)=wnQ(1/w) é o polinômio Q(w) com
os coeficientes em ordem reversa, incluem as aproximações
de Chebyschev inversas (Q(w)=Cn(w)). O parâmetro α define
a relação entra a atenuação nas bandas passante e de re-
jeição. Todos os polinômios geráveis pelo programa APOL
podem também ser usados para estas aproximações.
Aproximações
 racionais
 simétricas
 onde
K(jw)=εαQ(w)/Qr(w) incluem as aproximações
 elípticas.
Polinômios Q(w) adequados, mesmo para o caso das aproxima-
ções elípticas, devem ser gerados numericamente pelos
programas APRS ou APRA.
Aproximações racionais simétricas modificadas, onde
K(jw)= ε(2αQ(w)-Qr(w))/Qr(w) incluem aproximações
 com
"ripple" uniforme na banda passante e zeros de transmissão
duplos, de ordem par (um caso algo particular). Polinômios
Q(w) adequados devem ser gerados pelo programa APRS.
Outras aproximações podem ser geradas, fornecendo-se ao
programa H(s) ou K(s), e calculando a outra função.
A opção de elevar um polinômio ao quadrado serve para a
obtenção de aproximações cujas funções K(s) ou H(s) sejam
o quadrado de alguma outra, por exemplo.

