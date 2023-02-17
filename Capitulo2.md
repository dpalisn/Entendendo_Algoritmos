
# Capítulo 2

### 2.1 Suponha que você esteja criando um aplicativo para acompanhar as suas finanças. Todos os dias você anotará tudo o que gastou e onde gastou. No final do mês, você deverá revisar os seus gastos e resumir o quanto gastou. Logo, você terá um monte de inserções e poucas leituras. Você deverá usar um array ou uma lista para implementar este aplicativo?

*Baseando na ideia de otimizar a escrita em detrimento da leitura devemos escolher uma lista ao invés de um array, já que a inserção de anos em uma lista é dado por O(1) enquanto em um array é dado por O(n)*

### 2.2 Suponha que você esteja criando um aplicativo para anotar os pedidos dos clientes em um restaurante. Seu aplicativo precisa de uma lista de pedidos. Os garçons adicionam os pedidos a essa lista e os chefes retiram os pedidos da lista. Funciona como uma fila. Os garçons colocam os pedidos no final da fila e os chefes retiram os pedidos do começo dela para cozinhá-los. Você usaria um array ou uma lista encadeada para implementar essa lista? 

*Eu usaria uma lista, visto que os padrão de utilização se foca na inserção no início e retirada no final, sendo ambas operações O(1). Além do mais o acesso randômico facilitado, que seria a vantagem do array, não se aplica ao modelo de utilização da implementação.*

### 2.3 Vamos analisar um experimento. Imagine que o Facebook guarda uma lista de usuários. Quando alguém tenta acessar o Facebook, uma busca é feita pelo nome de usuário. Se o nome da pessoa está na lista, ela pode continuar o acesso. As pessoas acessam o Facebook com muita frequência, então existem muitas buscas nessa lista. Presuma que o Facebook usa a pesquisa binária para procurar um nome na lista. A pesquisa binária requer acesso aleatório – você precisa ser capaz de acessar o meio da lista de nomes instantaneamente. Sabendo disso, você implementaria essa lista como um array ou uma lista encadeada?

*Eu implementaria um array, já que a operação de acesso aos dados de forma aleatória seria dado por O(1), enquanto em uma lista a operação ter O(n)*

### 2.4 As pessoas se inscrevem no Facebook com muita frequência também. Suponha que você decida usar um array para armazenar a lista de usuários. Quais as desvantagens de um array em relação às inserções? Em particular, imagine que você está usando a pesquisa binária para buscar os logins. O que acontece quando você adiciona novos usuários em um array?

*A desvantagem do uso de array para as inserções é que adicionar um novo elemento tem velocidade de operação de O(n).*
*Ao inserir um elemento novo ao array a operação de busca binária iria aumentar o número de operações seguindo a curva Olog(n)*

### 2.5 Na verdade, o Facebook não usa nem arrays nem listas encadeadas para armazenar informações. Vamos considerar uma estrutura de dados híbrida: um array de listas encadeadas. Você tem um array com 26 slots. Cada slot aponta para uma lista encadeada. Por exemplo, o primeiro slot do array aponta para uma lista encadeada que contém os usuários que começam com a letra A. O segundo slot aponta para a lista encadeada que contém os usuários que começam com a letra B, e assim por diante.

### Suponha que o Adit B se inscreva no Facebook e você queira adicioná-lo à lista. Você vai ao slot 1 do array, a seguir para a lista encadeada do slot 1, e adiciona Adit B no final. Agora, suponha que você queira procurar o Zakhir H. Você vai ao slot 26, que aponta para a lista encadeada de todos os nomes começados em Z. Então, procura pela lista até encontrar o Zakhir H. Compare esta estrutura híbrida com arrays e listas encadeadas. É mais lento ou mais rápido fazer inserções e eliminações nesse caso? Você não precisa responder dando o tempo de execução Big(O), apenas diga se a nova estrutura de dados é mais rápida ou mais lenta do que os arrays e as listas encadeadas.

*A resposta depende do caso. Para buscas ela é mais lenta que um array e mais rápida que a lista ligada. Já na operação de inserção ela é mais rápida que um array e equivalente a lista lista ligada*
