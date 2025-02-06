<img src= "https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Imagens/Titulos/2.png?raw=true" width=100% > 

# Introdução
Neste projeto, foi construído um sistema de recomendação de filmes que utiliza dados do site 
MovieLens. Foram testados 3 algoritmos: FP-Growth, KNN e SVD, o último obteve o melhor 
desempenho. A liguagem utilizada foi **Python**.

O processo foi dividido em 5 etapas, conforme a figura a seguir: 

<img src= "https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/14cadd4403d7ee6c40dd757609c0fa5157170000/Imagens/Limpeza_e_Transformacao/Fluxograma.png" width=70% > 

O conjunto de dados tem 5 tabelas:
- **movies**: contêm o título e gênero do filme
- **ratings**: possui as avaliações de cada usuário, para cada filme. 
- **tags**: contêm as tags que cada usuário deu a um filme. Tags são palavras-chaves ou frases curtas que descrevem um filme.
- **genome_tags**: possui as colunas tag e tagId.
- **genome_scores**: tem uma coluna chamada relevance que mostra a relevância da tag em uma escala contínua (0 à 1).




# Link dos arquivos
O projeto foi dividido em 9 arquivos com duas versões: uma em HTML e outra em .iynb.
- **Amostragem:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/0.Amostragem_v2.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/0.Amostragem_v2.0.html) 
- **Limpeza:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/1.Limpeza_vers%C3%A3o_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/1.Limpeza_vers%C3%A3o_v4.html) 
- **Transformação parte 1 (tabela ratings):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.1_Transformacao_parte_1_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.1_Transformacao_parte_1_v4.0.html) 
- **Transformação parte 2 (tabelas movies e genome):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.0.html)
- **Transformação parte 3 (tabelas para modelagem):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.5.html) 
- **Análise Exploratória:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/4.Analise_Exploratoria_v5.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/4.Analise_Exploratoria_v5.5.html) <br>
- **Modelagem usando KNN:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_KNN_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_KNN_v4.0.html)
- **Modelagem usando FP-Growth:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_FP_Growth_v4.7.ipynb?short_path=86237e5) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_FP_Growth_v4.7.html) <br>
- **Modelagem usando SVD:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/25a629c173beebb46d044ff3d4a7e0dc157c0d17/Notebooks/6.Modelagem_SVD_v1.3.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/6.Modelagem_SVD_v1.3.html) <br>
<!--
- **Amostragem:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/0.Amostragem_v2.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/0.Amostragem_v2.0.html) 
<br><sub>O conjunto de dados é muito grande, por isso foi realizada amostragem de 3% dos usuários, o que deu 1.028.502 avaliações , 9.929 usuários e 26.770 filmes.</sub>
- **Limpeza:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/1.Limpeza_vers%C3%A3o_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/1.Limpeza_vers%C3%A3o_v4.html) 
<br><sub>Foi realizado a limpeza e descrição dos dados. Além da divisão entre dados de treino e teste.</sub>
- **Transformação parte 1 (tabela ratings):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.1_Transformacao_parte_1_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.1_Transformacao_parte_1_v4.0.html) 
<br><sub>Neste notebook foram realizada algumas transformações na tabela `ratings`, como a criação da coluna `ranting_medio_ponderado`.</sub>
- **Transformação parte 2 (tabelas movies e genome):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.0.html) <br><sub> Pequena pipeline para realizar transformações nas tabelas movies e genome.
- **Transformação parte 3 (tabelas para modelagem):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.5.html) 
<br><sub>Criação das tabelas para implementar os algoritmos FP-Growth e KNN.</sub>
- **Análise Exploratória:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/4.Analise_Exploratoria_v5.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/4.Analise_Exploratoria_v5.5.html) <br>
- **Modelagem usando KNN:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_KNN_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_KNN_v4.0.html)
- **Modelagem usando FP-Growth:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_FP_Growth_v4.7.ipynb?short_path=86237e5) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_FP_Growth_v4.7.html) <br>
- **Modelagem usando SVD:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/25a629c173beebb46d044ff3d4a7e0dc157c0d17/Notebooks/6.Modelagem_SVD_v1.3.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/6.Modelagem_SVD_v1.3.html) <br>
-->
# Resultado do Sistema de Recomendação
## Métrica 
A métrica utilizada será **Precisão (Precision)** que vai nos dizer quantos usuários assistiram pelo menos uma das 
recomendações. Foram consideradas 5 e 10 recomendações para o cálculo da 
métrica. A fórmula é a seguinte: 
<br><br>
$\text{Precisão} = \frac{\text{Assistiu}}{\text{(Assistiu + Não Assistiu)}} \times 100 \%$
<br><br>
Sendo, <br>
Assistiu: o algoritmo recomendou uma lista de filme e o usuário assistiu, pelo menos um filme.<br>
Não assistiu: o algoritmo recomendou uma lista de filme e o usuário não assistiu nenhum filme.

## Precisão (Precision) dos algorimos
O resultado da precisão (precision) foi resumido no gráfico a seguir. É possível notar que o algoritmo 
SVD obteve o melhor resultado.
<br>
<img src ="https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Imagens/Modelagem/Resultado_Precision.png?raw=true" width="50%">
#### FP-Growth
O algoritmo FP-Growth identifica padrões de comportamento com base no histórico de avaliações dos 
usuários. <br>
 Por exemplo, se vários usuários que avaliaram Harry Potter, também avaliaram O Senhor dos anéis, 
algoritmo vai entender isso como uma regra. E, na próxima vez que um usuário avaliar Harry Potter, 
o FP-Growth vai recomendar O Senhor dos anéis. <br>
O Precision do FP-Growth foi de apenas 19%, ou seja, o algoritmo acertou a recomendação para 19% 
dos usuários. Este foi o menor resultado.

#### KNN
O KNN é um algoritmo de classificação bem simples, ele dá a recomendação de filme com base na 
distância dos dados. Ao considerarmos 5 recomendações (n), o KNN acerta em 32% dos casos.
#### SVD (Decomposição de valor singular)
O terceiro algoritmo testado é o SVD (Decomposição de valor singular). Ele é um método de fatoração de matrizes. De maneira simplificada, a fatoração de matrizes é como se pegássemos o número 60 e fatorássemos em 3 x 4 x 5. 
   Depois que o SVD faz a decomposição (fatoração), ele reduz o tamanho das matrizes para diminuir a complexidade computacional.
  Uma analogia para isso, seria pensarmos em um pão de forma, tem pessoas que não gostam da casca e por isso, a retiram antes de preparar o sanduíche. Mesmo a gente retirando a casca, o resultado continua o mesmo.
   Ou seja, mesmo o SVD cortando as matrizes, o resultado final é o mesmo.  
  O precision do SVD foi de 54%, este foi o melhor resultado alcançado. Se considerássemos 10 recomendações, o precision do SVD chegaria a 60%.


## Referência de desempenho
Para termos uma noção se os resultados foram bons ou não, pesquisamos na literatura e encontramos 
uma precisão (precision) entre 25% e 87%, para este conjunto de dados: [(PATRA; GANGULY, 2019)](https://journals.sagepub.com/doi/abs/10.1177/2516600X19848956?journalCode=ospa),[(SIDDIQUE, A. et al)](https://journals.cfrit.com/index.php/ijisct/article/view/62) , [(AIREN; AGRAWAL, 2021)](https://link.springer.com/article/10.1007/s40009-021-01051-0), [(BAHI et al., 2023)](https://link.springer.com/chapter/10.1007/978-3-031-43838-7_4) e [(SUNILKUMAR, 2020)](https://elcvia.cvc.uab.cat/article/view/v19-n3-sunilkumar).

<mark><b>Portanto, concluímos que os resultados alcançados no projeto foram bons!</b></mark>

# Referências:
AIREN, S.; AGRAWAL, J. Movie Recommender System Using K-Nearest Neighbors 
Variants. **National Academy Science Letters**, 5 maio 2021.Disponível em: 
https://link.springer.com/article/10.1007/s40009-021-01051-0
<br><br>
BAHI, A et al. Personalized movie recommendation prediction using reinforcement learning. 
Em: **Communications in Computer and Information Science**. Cham: Springer Nature Switzerland, 
2023. p. 46–56. Disponível em: https://link.springer.com/chapter/10.1007/978-3-031-43838-7_4
PATRA, S.; GANGULY, B. Improvising singular value decomposition by KNN for use in movie 
recommender systems. **Journal of operations and strategic planning**, v. 2, n. 1, p. 22–34, 
2019.Disponível em: https://journals.sagepub.com/doi/full/10.1177/2516600X19848956
<br><br>
SIDDIQUE, A. et al. Movies rating prediction using supervised machine learning 
techniques. **International Journal of Information Systems and Computer Technologies**, v. 3, n. 1, 
p. 40–56, 2024. Disponível em: https://journals.cfrit.com/index.php/ijisct/article/view/62
<br><br>
SUNILKUMAR, C. N. A review of movie recommendation system: Limitations, Survey and 
Challenges. **ELCVIA Electronic Letters on Computer Vision and Image Analysis**, v. 19, n. 3, p. 
18, 17 set. 2020. Disponível em: https://elcvia.cvc.uab.cat/article/view/v19-n3-sunilkumar

