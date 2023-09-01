# Equipe Yvensíveis

# Subgrupo A
* Pedro César Mesquita Ferreira - 183998
* Yvens Ian Prado Porto - 184031
* Lucca Miranda Nunes - 230554

## Modelo Conceitual ER Revisado

> Coloque aqui o diagrama entidade-relacionamento original ou revisado para transformação em modelo relacional. O diagrama deve atributos, cardinalidade e entidades fracas.
>
> Indique abaixo do diagrama (como no exemplo), se é o original ou o revisado.
>
> Não é necessário colocar o diagrama UML revisado.

<img src="images/ER_Diagram_MMORPG.png" width="400px" height="auto">

*Diagrama ER Revisado*

## Mapeamento para o Modelo Relacional

> Coloque aqui o modelo relacional que mapeia o modelo ER (original ou revisado). Nesse modelo deve constar o esquema das relações, com as chaves primárias e estrangeiras. A especificação de tipos de atributos é opcional.

> Exemplo de modelo lógico relacional
~~~
CARDAPIO(_Data_, Refeição, Porção)
    Componentes Porção chave estrangeira -> COMP_PORÇÃO (ID Porção)
CONSOME(_ID Aluno_, _Data_, ID Porção)
    ID Porção chave estrangeira -> Porção (ID Porção)
PORÇÃO (_ID Porção_, Vezes Rejeitado, Vezes consumido, Componentes Ingredientes)
COMP_PORÇÃO (ID Porção, ID Ingrediente)
    ID Porção chave estrangeira -> Porção (ID Porção)
    ID Ingrediente chave estrangeira -> Ingrediente (ID Ingrediente)
INGREDIENTE (ID Ingrediente, Proteína, Carboidrato, Lipídio)
COMP_INGREDIENTE (ID Ingrediente Principal, ID Ingrediente Secundário)
    ID Ingrediente Principal chave estrangeira -> Ingrediente (ID Ingrediente)
    ID Ingrediente Secundário chave estrangeira -> Ingrediente (ID Ingrediente)
~~~
