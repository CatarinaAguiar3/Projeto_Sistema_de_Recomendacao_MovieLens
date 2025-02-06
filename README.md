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
1. **Amostragem:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/0.Amostragem_v2.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/0.Amostragem_v2.0.html) 
<br><sub>O conjunto de dados é muito grande, por isso foi realizada amostragem de 3% dos usuários, o que deu 1.028.502 avaliações , 9.929 usuários e 26.770 filmes.</sub>
2. **Limpeza:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/1.Limpeza_vers%C3%A3o_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/1.Limpeza_vers%C3%A3o_v4.html) 
<br><sub>Foi realizado a limpeza e descrição dos dados. Além da divisão entre dados de treino e teste.</sub>
3. **Transformação parte 1 (tabela ratings):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.1_Transformacao_parte_1_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.1_Transformacao_parte_1_v4.0.html) 
<br><sub>Neste notebook foram realizada algumas transformações na tabela `ratings`, como a criação da coluna `ranting_medio_ponderado`.</sub>
4. **Transformação parte 2 (tabelas movies e genome):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.2_Transforma%C3%A7%C3%A3o_parte_2_v3.0.html) <br><sub> Pequena pipeline para realizar transformações nas tabelas movies e genome.
5. **Transformação parte 3 (tabelas para modelagem):** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/2.3_Transforma%C3%A7%C3%A3o_parte_3_v3.5.html) 
<br><sub>Criação das tabelas para implementar os algoritmos FP-Growth e KNN.</sub>
6. **Análise Exploratória:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/4.Analise_Exploratoria_v5.6.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/4.Analise_Exploratoria_v5.5.html) <br>
7. **Modelagem usando KNN:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_KNN_v4.1.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_KNN_v4.0.html)
8. **Modelagem usando FP-Growth:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/main/Notebooks/5.Modelagem_FP_Growth_v4.7.ipynb?short_path=86237e5) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/5.Modelagem_FP_Growth_v4.7.html) <br>
9. **Modelagem usando SVD:** [notebook](https://github.com/CatarinaAguiar3/Projeto_Sistema_de_Recomendacao_MovieLens/blob/25a629c173beebb46d044ff3d4a7e0dc157c0d17/Notebooks/6.Modelagem_SVD_v1.3.ipynb) e [página html](https://catarinaaguiar3.github.io/Projeto_Sistema_de_Recomendacao_MovieLens/HTML/6.Modelagem_SVD_v1.3.html) <br>
