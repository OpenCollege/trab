```
exit()
python2.7
from classes import *
from entrada import *
```

### Variáveis salvas:

- paises -> Arvore com todos países
- brasil -> Pais Brasil, com arvore jogadores
- russia -> Pais Russia, com arvore jogadores

### Jogadores:

Ordem dos parametros: numero,posicao,nome,nascimento,idade,jogos,gols,time
(Não precisa preencher todos)   


```python
 lucas = Jogador("10","Atacante","Lucas","21 de Outubro")
 ```

### 1 - Inserir Jogador

A partir de uma arvore, insere um jogador


```python
brasil.jogadores.insere(lucas)

central(brasil.jogadores.root)
```

### 2 - Arvore com Todos Jogadores

A partir da arvore de países, cria uma arvore com todos jogadores de todos países
```python
todos_jogadores = gera_arvore_com_todos(paises.root)
central(todos_jogadores.root)
```

### 3 - Pesquisar por Nome

A partir de uma arvore de jogadores, pesquisa um jogador por nome


```python
nodo_danilo = pesquisa_por_nome(arvore_com_todos.root,"Danilo")
nodo_danilo.info.informacoes()
```

### 4 - Modificar Jogador

Depois de encontrado um jogador, um atributo pode ser mudado


```python
nodo_danilo.info.idade = "50"
nodo_danilo.info.time = "Time da UCS"
nodo_danilo.info.detalhes()
```

### 5 - Exibir todos jogadores

A partir da lista de paises, exibe todos jogadores de todos paises em ordem alfabética + total de jogadores


```python
todos_jogadores_em_ordem(paises)
```

### 6 - Exibe Jogadores País

A partir de um pais informado, exibe em ordem todos jogadores do pais


```python
russia = pesquisa_por_nome(paises.root,"Russia")
jogadores_pais(russia.root)
```

### 7 - Goleiros (Filtro por posição)

Percorre uma arvore de jogadores filtrando aqueles que tem uma certa posição


```python
jogadores_por_posicao(arvore_com_todos.root,"Goleiro")
```

### 8 - Jogadores Por Letra

Percorre uma arvore de jogadores filtrando aqueles que começam com uma letra


```python
jogadores_por_letra(arvore_com_todos.root,"A")
```

### 9 - Percurso Por Nivel (extra)

Percorre uma arvore, imprimindo cada nível em uma nova linha e os que estão no mesmo nível na mesma linha


```python2
percurso_por_nivel(brasil.jogadores)
```

### 10 - Pesquisa Descritiva (extra)

Procura um nome descrevendo o que a pesquisa faz a cada etapa do caminho


```python
percurso_por_nivel(brasil.jogadores)
pesquisa_descritiva(brasil.jogadores.root,"Lucas")
```
