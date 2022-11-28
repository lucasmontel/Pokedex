# Anotações
# REM
##### O "rem" toma como base um tamanho já declarado, exemplo: body{font-size:15px} "p{font-size: .8rem}" esse rem pegará como base o primeiro tamanho declarado lá no body , já por sua vez o "em" , toma com base o rem que por sua vez sempre é o segundo a ser chamado.

# Promisse<response>
##### Ele quer dizer que uma hora ele irá chegar , mas não e de imediato

# then
##### Ele processa o que vem como resultado do servidor
# Catch
##### Diferente do then , o catch é caso algo de erro, e executa determinada coisa (caso verdadeiro)
# Promisse.all(parâmetro)

### .then((pokemons) => pokemons.map(pokeApi.getPokemonDetail))
### .then((detailRequests) => Promise.all(detailRequests)):

##### Na linha 14, fizemos uma requisição(chamando uma função que faz isso) para cada pokemon dentro da lista de pokemons(usando map), o que ele retornar, será atribuída  ao (detailRequest), depois falamos para ele esperar que a função que faz a requisição seja chamada para todos elementos do array, ou seja , cada "pokemon" , usando : "Promise.all(detailRequests)):"

### .then((pokemonsDetails) => pokemonsDetails):
##### Depois que fizemos a requisição para cada pokemon(A requisição ficará guardada com cada pokemon) falamos para ele que todos essa lista de requisição de pokemons é igual ao parâmetro.