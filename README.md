# Edson Simões Boldrini - Blog

Seja bem vindo ao meu blog!
Aqui postarei vários textos que gosto e textos sobre as disciplinas e entregas de trabalhos da minha faculdade.<br>


# [Postagem 4 - Qualidade de Software - 17/04/10](https://github.com/edsonsb96/blog/blob/master/Postagem%202%20-%20Qualidade%20de%20Software.md)

Eae pessoal, tudo bem?<br>
Hoje falarei sobre um tema bastante polêmico, e que extremamente polarizado. Modelos ricos e modelos anêmicos.<br>
O que são modelos ricos e anêmicos? Quais as vantagens e desvantagens de cada um? Qual é mais adotado no mercado e porque?<br>
Esse post foi baseado no [podcast 11 modelo rico e modelo anêmico, da dotNet Arc Cast](http://podcast.dotnetarchitects.net/2010/03/podcast-11-modelo-anemico/), Fique a vontade para opinar com comentários.<br>

Modelo rico e modelo anêmico são duas perspectivas muito diferentes, ai está o porquê de serem tão polarizadas. <br>
Modelo anêmico trata de programas exclusivamente procedurais, ou seja, códigos com bastantes linhas, não há a presença de funções exclusivas, as vezes temos repetição de código e por fim muitas funçoes, dentro de um mesmo programa. Entre as desvantagens, encontramos dificuldade quando vamos fazer mudanças(manutenção) de algum programa; com suas funções colocadas de forma procedural, não conseguimos separar tão bem qual função(método) deve ser usada em qual variável(estrutura, objeto), e assim, quando vamos mudar algo no código, frequentemente temos que mudar uma grande parte das funções em cada simples mudança necessária. Como vantagem, temos o fato de que programação procedural, é bem mais fácil que programação orientada a objetos, esta, necessita de uma maturidade maior da a equipe para que o padrão de projeto não seja afetado(a programação orientada a objetos oferece um leque maior de soluções possíveis para um problma), maturidade essa não tão necessária no modelo anêmico/procedural, facilitando assim uma grande equipe trabalhar num projeto de grande escala.<br>
Modelos ricos tratam os problemas com mais abstração, ou seja, você não necessita criar um objeto sabendo o que ele vai se tornar, ele pode assumir vários atributos e vários métodos, você trabalha com modelos reais de construção tratando o problema como ele é na vida real(suas características, seus comportamentos e seus estados possíveis). Modelos ricos tendem a separar um programa em vários pedaços e camadas, e assim ele pode ser construido aos poucos enquanto cada parte tem uma pequena independência das demais, o que exige uma maturidade maior de seus progamadores, bem como uma visão mais ampla das relações em que cada parte tem entre si. Como vantagens, podemos citar características como, reutilização de código, polimorfismo, herança etc... todas essas, características exclusivas da programação orientada a objeto, abrindo assim, um grande leque de situações e soluções para um sistema ou problema.<br>
Sobre o mercado? Há uma grande preferência pelos modelos ricos, já foi citado anteriormente sobre seu leque de soluções e esse é o grande diferencial para as empresas que adotam esse sistema, além de poder trabalhar com objetos de verdade, analizando o problema de forma mais física observando seus atores e comportamentos. Já as empresas que ainda insistem em utilizar o modelo anêmico, em boa parte tem medo de colocar seus funcionários para trabalharem utilizando as diretrizes de um modelo mais complexo, e assim, preferem continuar com seu modelo mais simples, com entendimento mais fácil, porém com manutenção bem mais complicada. <br>
Termino minha postagem dizendo que os modelos ricos são o presente e o futuro das soluções computacionais, se vc quer ter sucesso em alguma empresa ou quer que a sua empresa tenha mais sucesso, preze pelo modelo rico, pressione seus funcionários a terem um entendimento maior e não se acomodarem com a programação procedural. Costumes mais simples, sempre criam empregados mais acomodados e preguiçosos, o que gera, consequentemente, um rendimento menor.<br>

Edson Simões Boldrini<br>

# [Postagem 2 - Qualidade de Software - 17/03/13](https://github.com/edsonsb96/blog/blob/master/Postagem%202%20-%20Qualidade%20de%20Software.md)

![alt text](https://github.com/edsonsb96/blog/blob/master/ferrari.jpg "Pode um Fusca, ser melhor que uma Ferrari?")

Eae pessoal, tudo bem?<br>
Hoje falarei sobre um tema que tem sido frequentemente discutido na esfera de desenvolvimento em TI. Qualidade de software.<br>
Afinal, o que é Qualidade de software? O que é mais importante na hora de desenvolver? O que são os indicadores e atributos de qualidade?<br>
Essa discussão foi baseada no [podcast 10 qualidade do software, dotNet Arc Cast](http://podcast.dotnetarchitects.net/2010/02/podcast-10-qualidade-de-software/), Fique a vontade para opinar com comentários.<br>

Qualidade de software, muitas vezes é um assunto muito subjetivo. Uns pensam que qualidade se resume ao fato de algo ser bom, mas o que de fato é ser bom?<br>
Gosto da comparação que é feita entre um Fusca e uma Ferrari citada no podcast. Na primeira impressão, se alguém te perguntasse o que tem mais qualidade, entre os dois, obviamente você responderia que a Ferrari é superior ao Fusca, mas então pra exemplicar o que é qualidade, um caso hipotético onde essa pergunta pode ter uma resposta seria o seguinte: Essa Ferrari, foi projetada pra ter 300 km/h de velocidade máxima, já o Fusca, projetado pra chegar a uma velocidade máxima de 80 km/h. Na prática, o Fusca chegou a 100 km/h e a Ferrari chegou a 250 km/h. Você conseguiria responder que a Ferrari ainda tem a qualidade superior que o Fusca?<br>
Não! E isso não é subjetivo, pois para medir se algo tem qualidade ou não tem, é preciso analisar antes do teste, o que ele se propôs a fazer. Usando o exemplo, o Fusca tinha como velocidade máxima 80 km/h, mas conseguiu ir além das expectativas, já a Ferrari, tinha como 300 km/h como velocidade, mas não conseguiu atender bem as especificações. Resumindo, a Ferrari, decepcionou e não mostrou a efetividade e qualidade presentes na construção do Fusca, que superou as suas próprias marcas.<br>
Assim, também acontece nos códigos, se aquele programa que está sendo desenvolvido não atende bem, ou atende por um tempo insuficiente a demanda proposta, ele tem sua qualidade colocada em xeque.<br>
O que é mais importante na hora de desenvolver? O que são os indicadores e atributos de qualidade?<br>
Aqui sim temos um ramo bem subjetivo, afinal, nenhum cliente é igual ao outro, então o que é mais importante bem como os atributos de qualidade podem variar de sistema pra sistema. Por exemplo, um cliente pode querer um sistema que tenha como prioridade a entrega mais rápida possível, e assim apressar o desenvolvedor(não dar um tempo suficente para que ele desenvolva um sistema melhor) na hora da produção do sistema; possivelmente, esse sitema terá alguns bugs que teriam sido resolvidos caso o desenvolvedor tivesse um tempo maior para poder trabalhar o projeto. Resumindo, os atributos de qualidade e seus indicadores, dependerão única e exclusivamente do que seus respectivos clientes estão tratando como prioridade, por isso, é de suma importância, tratar bem detalhadamente com o cliente certos atributos antes de assumir o projeto, atributos como: Quanto tempo o sistema demorará pra ser feito, quais dados deverão ser fornecidos pelo cliente, quanto custará o serviço final... são fundamentais antes da produção do sistema.<br>
Após essas discussões, podemos ver que qualidade de software não é algo tão simples, exige um grande comprometimento do prestador de serviços para que ele descubra as diretrizes e prioridades do cliente, para assim, poder garantir que o sistema terá uma qualidade anexada.<br>

Edson Simões Boldrini<br>
