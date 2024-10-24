# Projeto Film Junky Union: Classificação de Resenhas de Filmes

## Descrição do Projeto
A **Film Junky Union**, uma nova comunidade para entusiastas de filmes clássicos, está desenvolvendo um sistema para filtrar e categorizar resenhas de filmes. O objetivo deste projeto é treinar um modelo para detectar automaticamente resenhas negativas. Utilizando um conjunto de dados de resenhas de filmes do IMDB com rotulagem de polaridade, o modelo deve classificar as resenhas como positivas ou negativas, atingindo um valor F1 de pelo menos 0,85.

## Ferramentas e Bibliotecas Utilizadas
- **Python**: Linguagem principal utilizada para a análise.
- **Pandas**: Biblioteca para manipulação e análise de dados.
- **NLTK**: Biblioteca para processamento de linguagem natural.
- **spaCy**: Biblioteca avançada para processamento de linguagem natural.
- **Scikit-learn**: Biblioteca para aprendizado de máquina e avaliação de modelos.
- **LightGBM**: Biblioteca para classificação e regressão de alto desempenho.

  ## Descrição dos Dados
Os dados são armazenados no arquivo `imdb_reviews.tsv`. 
- **review**: texto da resenha.
- **pos**: alvo, onde '0' indica negativo e '1' indica positivo.
- **ds_part**: 'train'/'test' para a parte de treinamento/teste do conjunto de dados.

## Passo a Passo do Projeto

1. **Carregamento dos Dados**:
   - Download do conjunto de dados a partir do arquivo `imdb_reviews.tsv`.

2. **Pré-processamento dos Dados**:
   - Análise inicial dos dados e aplicação de limpeza.

3. **Análise Exploratória de Dados (AED)**:
   - Condução de uma AED para entender a distribuição das classes e possíveis problemas de desequilíbrio.

4. **Preparação para Modelagem**:
   - Pré-processamento dos dados de texto para adequação à modelagem.

5. **Treinamento de Modelos**:
   - Treinamento de pelo menos três modelos diferentes, incluindo:
     - Modelo 1: NLTK, TF-IDF e Regressão Linear.
     - Modelo 2: spaCy, TF-IDF e Regressão Linear.
     - Modelo 3: spaCy, TF-IDF e LGBMClassifier.

6. **Teste dos Modelos**:
   - Avaliação dos modelos usando o conjunto de dados de teste e cálculo do F1-Score.

7. **Validação com Resenhas Manuais**:
   - Criação de algumas resenhas manuais e classificação delas usando todos os modelos.

8. **Análise de Resultados**:
   - Comparação dos resultados dos testes dos modelos e explicação das diferenças observadas.

9. **Apresentação das Descobertas**:
   - Compilação das descobertas e recomendações para futuras implementações.

## Conclusão
Neste projeto, buscou-se desenvolver modelos de classificação de sentimentos para resenhas de filmes, com o objetivo de atingir um valor F1 de pelo menos 0,85. Utilizamos três abordagens principais, descritas a seguir, com uma comparação detalhada de suas performances:

- **Modelo 1 - NLTK, TF-IDF e Regressão Linear**: F1-Score de 0,88. Acurácia de 94% nas resenhas manuais.
  
- **Modelo 2 - spaCy, TF-IDF e Regressão Linear**: F1-Score de 0,88. Acurácia de 94% nas resenhas manuais. Melhor desempenho geral.

- **Modelo 3 - spaCy, TF-IDF e LGBMClassifier**: F1-Score de 0,84. Acurácia de 83% nas resenhas manuais.

**Análise dos Resultados**: Modelos 1 e 2 alcançaram o objetivo de um F1-Score de pelo menos 0,85, com o Modelo 2 mostrando desempenho mais consistente. O Modelo 2 se destacou como o mais equilibrado e robusto para classificar novas resenhas.

## Aprendizados
Este projeto permitiu-me desenvolver as seguintes habilidades:
- **Processamento de Linguagem Natural (PLN)**: Aprendizado sobre técnicas de PLN e vetorização de texto.
- **Treinamento e Avaliação de Modelos**: Habilidade em treinar e avaliar modelos de classificação com diferentes abordagens.
- **Análise de Desequilíbrio de Classe**: Compreensão dos desafios e estratégias para lidar com o desequilíbrio de classe em conjuntos de dados.
- **Criação de Resenhas**: Experiência prática na aplicação de modelos para prever sentimentos em textos reais.

## Como Executar o Projeto

- Clone o repositório.
- Navegue até o diretório do projeto.
- Abra o projeto no seu IDE favorito.
- Instale as dependências.
- Execute o script principal.

## Contato

Luciano Pinto
[LinkedIn](https://www.linkedin.com/in/lucianolcp/)  
Email: dslucianopinto@gmail.com
