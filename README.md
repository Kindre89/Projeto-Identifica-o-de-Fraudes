# Dicionário de dados

Fonte dos dados: [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

| Nome da coluna | Descrição             | Tipo de dado |
|----------------|-----------------------|--------------|
| `Time`         | Intervalo em segundos entre cada transação e a primeira | float     |
| `Vx`           | Resultado de PCA das variáveis originais | float   |
| `Amount`       | Valor de cada transação | float         |
| `Class`        | Classificação da transação entre genuína, 0, e fraudulenta, 1 | int        |

Na descrição da base de dados no Kaggle, são fornecidas algumas explicações acerca das variáveis:

- por questões de confidencialidade, não são disponibilizadas as identificações de boa
parte das variáveis originais;
- as representadas como V1, V2,... V28 são resultado de
uma transformação de análise de componentes principais - PCA, uma técnica utilizada para
condensar a informação contida em várias variáveis originais em um conjunto menor de
variáveis estatísticas (componentes) com uma perda mínima de informação. No trabalho
veremos algumas consequências dessa transformação em nossa análise;

## Organização do projeto

```
├── .env               <- Arquivo de variáveis de ambiente (não versionar)
├── .gitignore         <- Arquivos e diretórios a serem ignorados pelo Git
├── ambiente.yml       <- O arquivo de requisitos para reproduzir o ambiente de análise
├── LICENSE            <- Licença de código aberto se uma for escolhida
├── README.md          <- README principal para desenvolvedores que usam este projeto.
|
├── dados              <- Arquivos de dados para o projeto.
|
├── modelos            <- Modelos treinados e serializados, previsões de modelos ou resumos de modelos
|
├── notebooks          <- Cadernos Jupyter. A convenção de nomenclatura é um número (para ordenação),
│                         as iniciais do criador e uma descrição curta separada por `-`, por exemplo
│                         `01-fb-exploracao-inicial-de-dados`.
│
|   └──src             <- Código-fonte para uso neste projeto.
|      │
|      ├── __init__.py  <- Torna um módulo Python
|      ├── config.py    <- Configurações básicas do projeto
|      └── graficos.py  <- Scripts para criar visualizações exploratórias e orientadas a resultados
|
├── referencias        <- Dicionários de dados, manuais e todos os outros materiais explicativos.
|
├── relatorios         <- Análises geradas em HTML, PDF, LaTeX, etc.
│   └── imagens        <- Gráficos e figuras gerados para serem usados em relatórios
```

