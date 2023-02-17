  
# Capítulo 1
### 1.1 Suponha que você tenha uma lista com 128 nomes e esteja fazendo uma pesquisa binária. 
Qual seria o número máximo de etapas que você levaria para encontrar o nome desejado?
*Sabendo que se trata de um algoritmo de pesquisa binária, deveremos calcular o número máximo a partir da do logaritmo de n na base 2, sendo n o número de elementos. Sendo Log2(128) = 7 temos que o número máximo de operações será 7.*

### 1.2 Suponha que você duplique o tamanho da lista. Qual seria o número máximo de etapas agora?
*Duplicando o número de itens na lista teremos 256 itens ao todo. Novamente aplicando Log2(256) = 8, chegamos ao resultado de 8 operações para o pior caso.*

## Forneça o tempo de execução para cada um dos casos a seguir em termos da notação Big O.
  ### 1.3 Você tem um nome e deseja encontrar o número de telefone para esse nome em uma agenda telefônica.
*Considerando o algoritmo de busca binária sendo o mais adequado para buscar em uma lista telefônica ordenada, o tempo de execução para esse algoritmo será dado por O log(n).*

### 1.4 Você tem um número de telefone e deseja encontrar o dono dele em uma agenda telefônica. 
*Uma vez que a busca deverá percorrer toda a agenda pois os a ordenação da lista é por nomes e não pelos números dos contatos, o algoritmo deverá ser uma busca linear. Por ser uma busca linear ela terá como tempo de execução O(n).*

### 1.5 Você quer ler o número de cada pessoa da agenda telefônica.
*Para ler o numero de cada pessoa também será preciso percorrer a lista como um todo, então o tempo de execução será novamente linear dado por O(n).*

### 1.6 Você quer ler os números apenas dos nomes que começam com A.
*A resposta para essa questão é O(n). Pois mesmo que seja somente uma fatia do todo que seria composto o alfabeto a curva de crescimento manterá a mesma, tornando O(n) a forma correta descrever a rapidez do algoritmo.*
