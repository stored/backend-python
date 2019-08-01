# Desafio técnico Python

Alguns requisitos:

- Use Git;
- Procure fazer "micro commits" que são muitos commits com menos código isso nos ajuda a compreender a sua lógica;
- Nos pergunte sobre qualquer dúvida que venha a surgir durante o desenvolvimento;
- Não procure soluções na internet;
- Crie um repositório público e nos passe o link para acompanharmos o desenvolvimento.


Sugerimos utilizar:
- Use Python >= 3.6;
- Use Django;
- Use Django Rest Framework;
- Docker


A Stored-Frete, grande empresa de logística está desenvolvendo um novo sistema e sua ajuda é muito importante neste	momento.
Sua	tarefa será	desenvolver um novo	sistema	de entregas	visando	sempre o menor custo.

Esse sistema consiste numa API Rest, com uma autenticação JWT.
Você está livre para escolher o formato de grafia do seu endpoint, mas pedimos que ele seja versionado.
Obviamente você deve usar os verbos da metodologia RESTful.

O sistema consiste nas instancias: Usuário, Malha logística, Rota e Cidade
Onde cada usuário possui suas malhas, e cada malha possui suas respectivas rotas entre as cidades.
Importante que cada usuário só veja na api as suas respectivas malhas

Sugestão para usuário:

	/api/v1/login - Sem autenticação JWT
	/api/v1/register - Sem autenticação JWT


Para o cadastro das malhas e cidades, você está totalmente livre para definir a sua estrutura.
Só lembrando que para os dados das malhas, devem seguir a autenticação JWT.
Mais basicamente, consiste em definir um ponto de origem, um ponto de destino e a distância entre eles. 

Exemplo da "Malha SP"
---------------------
- A	B	10
- B	D	15
- A	C	20
- C	D	30
- B	E	50
- D	E 30

No sistema, é importante que se tenha um endpoint para listar as rotas e as cidades de uma determinada malha.
Com as suas malhas já definidas, vem o verdadeiro objetivo do sistema que é calcular o menor valor de uma entrega, como também o melhor caminho entre as rotas.

Um exemplo de requisição, seguindo o exemplo de "Malha SP"
----------------------------------------------------------
	mapa SP
	origem A
	destino	D
	autonomia 10
	valor do litro 2,5

A resposta seria
----------------
	resposta seria a rota ABD com 6,25 de custo

Voce está livre	para definir a melhor arquitetura e	tecnologias	para solucionar	este desafio,
mas	não	se esqueça de contar sua motivação no arquivo README que deve acompanhar sua solução, junto	com	os detalhes de	como executar seu programa.
Documentação e testes serão	avaliados também =).

Lembre-se de que iremos	executar seu código	com	malhas beeemm mais complexas, por isso é importante	pensar em requisitos não funcionais	também!

Também gostariamos de acompanhar o desenvolvimento	da	sua	aplicação através do	código	fonte
Por	isso, solicitamos a criação	de	um	repositório	que	seja compartilhado	com	a gente.

Nós	solicitamos	que	você trabalhe no desenvolvimento desse sistema	sozinho	e não	divulgue a solução	desse problema	pela internet.

Bom desafio!

![Luck](https://media.tenor.com/images/e026ce9d75219c8d82277ddf0558ee2b/tenor.gif)
