# Titanic: Análise de Sobrevivência

<p align="center">
    <img src="https://media1.giphy.com/media/Nvupk0dHsjBXq/giphy.webp?cid=ecf05e47dm7m3kephr6m55toehbcms0zzcambd69gszvx1mc&ep=v1_gifs_related&rid=giphy.webp&ct=g" alt="GIF Titanic" width="400">
</p>

##Análise e Predição da Sobrevivência no Titanic
O objetivo deste projeto é realizar uma análise exploratória detalhada dos dados do Titanic e construir modelos preditivos para entender os fatores que influenciaram as chances de sobrevivência dos passageiros. O projeto é com base em dados históricos de passageiros, como idade, classe social, sexo, e porto de embarque, o projeto visa identificar padrões e insights sobre as variáveis que mais impactaram as probabilidades de sobrevivência. Além disso, serão desenvolvidos modelos preditivos que podem auxiliar na compreensão dos comportamentos passados e fornecer uma base para a análise de decisões em contextos de emergência e resgate.

## Justificativa

O naufrágio do Titanic, um dos maiores desastres marítimos da história, continua a ser um marco de reflexão sobre os fatores que influenciam a sobrevivência em situações extremas. Analisar os dados históricos dos passageiros do Titanic pode fornecer valiosos insights sobre a relação entre características como classe social, idade, sexo e a probabilidade de sobrevivência. Este projeto visa explorar essas variáveis para entender os padrões e os determinantes que afetaram as chances de sobrevivência, fornecendo informações que podem ser aplicadas no desenvolvimento de modelos preditivos para cenários de crise e resgate.

## Base de dados

A análise utiliza o dataset 'Titanic: Machine Learning from Disaster', disponível no <a href="https://www.kaggle.com/c/titanic/data" target="_blank">Kaggle</a>
. A base contém informações sobre passageiros do Titanic, como idade, sexo, classe de cabine, número de familiares a bordo, entre outras variáveis. Com esses dados, é possível realizar uma análise aprofundada sobre o impacto de fatores socioeconômicos e pessoais nas chances de sobrevivência durante o desastre.

## Metodologia

A metodologia utilizada será a CRISP-DM, composto por:

1. Entendimento de negócio
2. Entendimento de dados
3. Preparação dos dados
4. Modelagem

## Etapas do projeto

### Dicionário de dados
Etapa de realização da coleta inicial de dados, com criação de um arquivo na pasta data/raw.
Criação do dicionário de dados, estrutura que servirá para explicar o dado, contendo as seguintes informações para cada uma das variáveis do conjunto de dados:
* variavel: nome da coluna no pandas
* descricao: descrição da coluna
* tipo: quantitativa ou qualitativa
* subtipo: nominal, ordinal, discreta, contínua

### Análise exploratória de dados
Criação de um notebook de análise exploratória notebooks/01-exploratory_data_analysis.ipynb, com as seguintes seções de texto:
* Descrição dos dados: informações sobre a quantidade de instâncias, variáveis e seus tipos, quantidade de valores faltantes. Utilize o dicionário de dados nessa seção.
* Perguntas de partida e hipóteses: que tipo de informações podem ser obtidas a partir dos dados e quais hipóteses podem ser levantadas?
* Insights: respostas às perguntas feitas na seção anterior e quais informações interessantes podem ser levantadas através dos dados?

### Análise comparativa de modelos
Criação de um notebook de análise comparativa notebooks/02-comparative_analysis.ipynb, contendo as seguintes seções de texto: Metodologia, Configuração do experimento, Resultados e discussão.
* Desenvolver todo pré-processamento de dados, realizando tratamento de dados faltantes, codificação de variáveis e normalização de dados.
* Utilizar um método de validação cruzada (holdout, k-fold, Monte Carlo).
* Apresentar no mínimo quatro modelos: um baseline, para servir de comparação a pelo menos outros três (ou mais) experimentos com modelos de famílias diferentes. Deverão ser utilizadas pelo menos duas métricas para efetuar a comparação entre os modelos;
* Para que os resultados sejam avaliados, eles devem ser sintetizados através da utilização de tabelas e/ou gráficos explicativos;

## Funcionalidades

Esse template foi inicialmente baseado no [template de ciência de dados do cookiecutter](https://drivendata.github.io/cookiecutter-data-science/), mas ao longo do tempo várias modificações foram sendo realizadas. Atualmente o template tem as seguintes características:
 - Utilização do arquivo `pyproject.toml` como centralizador de dependências;
 - Configuração para criação de aplicação `streamlit`;
 - Utilização de [jupyter notebooks](https://jupyter.org/) para arquivos de análise;
 - Documentação com o [mkdocs](https://www.mkdocs.org/) ([material design](https://squidfunk.github.io/mkdocs-material/) theme)

## Instruções para iniciar o projeto

### Requisitos

Para utilizar este template, você precisará de um ambiente com os seguintes softwares:
 - git
 - Python 3.8
 - Poetry `1.1.13` ou superior

É aconselhável o uso do `pyenv` para o gerenciamento de versões do Python.

### Iniciando um novo projeto

Para iniciar um novo projeto você precisa ter instalado na sua máquina as aplicações citadas na seção anterior, depois disso basta:

1. clicar no botão **Use this template** (ou "Usar este modelo").
2. Digitar um nome para seu repositório e uma descrição opcional.
3. Escolher a visibilidade do projeto (Publica ou privada).
4. Clicar em **Create repository from template** (Criar repositório a partir do modelo).

Pronto, acaba de criar um repositório a partir deste modelo. Para mais informações sobre o uso de templates, acesse a [documentação oficial](https://docs.github.com/pt/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).


### Contribuindo com um repositório já criado

Depois de criar o repositório, para começar a modificá-lo e/ou contribuir com repositórios já criados,  você precisa cloná-lo. Para isso, siga os seguintes passos:

1. Acima da lista de arquivos, clique no botão **Code** (em verde).
2. Copie a URL para o repositório.
    - Tente clonar utilizando uma chave **SSH**. Para isso, clique na aba **SSH** e em seguida clique no ícone de cópia.
3. Abra o terminal.
4. Altere o diretório de trabalho atual para o local que deseja ter o diretório clonado.
5. Digite `git clone` e cole a URL que você copiou anteriormente:

```
git clone git@github.com:NOME-DE-USUARIO/REPOSITORIO.git
```
6. Pressione **Enter** para criar seu clone local.

Proto, com isso você acaba de clonar um repositório. Para mais informações sobre a clonagem de arquivos, acesse a [documentação oficial](https://docs.github.com/pt/repositories/creating-and-managing-repositories/cloning-a-repository).

Com o repositório clonado, você precisa navegar até a pasta local, usando o comando :

```
cd REPOSITORIO
```

Estando na pasta do repositório, basta instalar as dependências do projeto utilizando o comando:

```
poetry install
```

Ele irá instalar todas as dependências contidas no arquivo `pyproject.toml`. Depois disso basta ativar o ambiente virtual criado pelo Poetry utilizando o comando:

```
poetry shell
```

Para mais informações sobre os comandos do Poetry, visite a [documentação oficial](https://python-poetry.org/docs/).

Para contribuir com um projeto, tente utilizar uma metodologia adequada. Utilize [este artigo](https://omadson.github.io/site/blog/2022/software-development-workflow/) para obter mais informações.


### Organização de diretórios


```
.
├── data/              # Diretório contendo todos os arquivos de dados
│   ├── external/      # Arquivos de dados de fontes externas
│   ├── interim/       # Arquivos de dados intermediários
│   ├── processed/     # Arquivos de dados processados
│   └── raw/           # Arquivos de dados originais, imutáveis
├── docs/              # Documentação gerada através da biblioteca mkdocs
├── models/            # Modelos treinados e serializados, predições ou resumos de modelos
├── notebooks/         # Diretório contendo todos os notebooks utilizados nos passos
├── references/        # Dicionários de dados, manuais e todo o material exploratório
├── src/               # Código fonte utilizado nesse projeto
│   ├── data/          # Classes e funções utilizadas para download e processamento de dados
│   ├── deployment/    # Classes e funções utilizadas para implantação do modelo
│   └── model/         # Classes e funções utilizadas para modelagem
├── app.py             # Arquivo com o código da aplicação do streamlit
├── Procfile           # Arquivo de configuração do heroku
├── pyproject.toml     # Arquivo de dependências para reprodução do projeto
├── poetry.lock        # Arquivo com sub-dependências do projeto principal
├── README.md          # Informações gerais do projeto
└── tasks.py           # Arquivo com funções para criação de tarefas utilizadas pelo invoke

```
