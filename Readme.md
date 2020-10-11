# Visão Geral
Neste Projeto, vamos construir um sistema de recomendação baseado em filtragem colaborativa usando MovieLens Datasets. Além disso, sera usado um modelo KNN para agrupar filmes parecidos baseado na avaliaçao dos usuarios e fazer recomendações com base na pontuaçao de similaridade de filmes avaliados anteriormente. 

# Sistemas de Recomendação

Um sistema de recomendaçao é basicamente um sistema de filtragem de informaçao que visa prever a avaliaçao ou preferencia que um usuario poderia dar a um "item". Isto é utilizado em varios pontos da internet, por exemplo: Amazon, Netflix, Spotify, or medias sociais como facebook, e youtube. Com uso de SR, essa companias sao capazes de fornecer melhor ou mais produtos/serviços/conteudos que sao personalizados para o usuario com base no seu historico de consumo

Sistemas de Recomendaçao tipicamente produzem uma lista de recomendaçoes atraves da filtragem colaborativa ou atraves da filtragem baseada em conteudo. 

Este projeto vai focar na filtragem colaborativa e e usar sistemas de filtragem colaborativa com base em itens para recomendar filmes.

# Filtragem colaborativa baseada em item

Sistemas baseados em filtragem colaborativa usam açoes de usuarios para recomendar outros items. Em geral, podem ser baseados no usuario ou item.User based collaborating filtering uses the patterns of users similar to me to recommend a product (users like me also looked at these other items). A filtragem colaborativa baseada em item usa os padrões de usuários que navegaram no mesmo item que eu para me recomendar um produto (os usuários que olharam meu item também olharam esses outros itens). A abordagem baseada em item é geralmente preferida do que a abordagem baseada no usuário. A abordagem baseada no usuário costuma ser mais difícil de escalonar devido à natureza dinâmica dos usuários, enquanto os itens geralmente não mudam muito, então a abordagem baseada em itens pode ser calculada offline.  

# Base de dados

Para este exemplo escolhi a [base de dados minificada MovieLens] que descreve a avaliação de 5 estrelas e a atividade de marcação de texto livre do MovieLens, um serviço de recomendação de filmes. Ele contém 1.00836 classificações e 3.683 aplicativos de marcação em 9.742 filmes. Esses dados foram criados por 610 usuários entre 29 de março de 1996 e 24 de setembro de 2018. Este conjunto de dados foi gerado em 26 de setembro de 2018.

Os usuários foram selecionados aleatoriamente para inclusão. Todos os usuários selecionados avaliaram pelo menos 1 filme. Nenhuma informação demográfica é incluída. Cada usuário é representado por um id e nenhuma outra informação é fornecida. Os dados estão contidos nos arquivos genome-scores.csv, genome-tags.csv, links.csv, movies.csv, ratings.csv e tags.csv.

# Conteudo do Projeto

1. Carregar dados
2. Analise Exploratoria dos dados
3. Treinar modelo KNN para filtragem colaborativa dos daos. 
4. Usar o modelo treinado para fazer recomendaçoes de filme 
5. Aprofundamento nos gargalos da abordagem de filtragem colaborativa baseada em item.
    - Problema de congelamento inicial
    - Problema de dispersão dos dados
    - viés popular (como recomendar produtos desde o final da distribuição de produtos)
    - Gargalo na scalabilidade
6. Estudos para o futuro



   [base de dados minificada MovieLens]: <https://www.kaggle.com/pedroaugusto97/movielenssmall/download>