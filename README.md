# Análise da Taxa de Distorção Idade-Série no Brasil (2024)

Este repositório contém a análise da Taxa de Distorção Idade-Série (TDI) para Brasil, regiões e UFs, com base nos dados de 2024. A análise foi realizada usando Python e suas bibliotecas de ciência de dados.

## Visão Geral

A Taxa de Distorção Idade-Série é um indicador educacional que mostra a proporção de estudantes que estão com idade superior à esperada para a série/ano que estão cursando. Esta análise explora este indicador para diferentes:

- Níveis de ensino (Fundamental e Médio)
- Regiões geográficas do Brasil
- Anos/séries específicos

## Dados Analisados

Os dados utilizados são provenientes do arquivo `TDI_BRASIL_REGIOES_UFS_2024.xlsx`, que contém informações sobre:

- Taxa de Distorção por Unidade Geográfica (Brasil, Regiões, UFs)
- Localização (Total, Urbana, Rural)
- Dependência Administrativa (Total, Federal, Estadual, Municipal, Privada)
- Taxas por nível de ensino e por ano/série específico

## Principais Resultados

### Taxa de Distorção por Região

- **Brasil (média)**: 10,9% no Ensino Fundamental e 17,8% no Ensino Médio
- **Região Norte**: apresenta a maior taxa (17,6% no Fundamental e 26,8% no Médio)
- **Região Sudeste**: apresenta a menor taxa (7,5% no Fundamental e 13,9% no Médio)

### Progressão da Taxa de Distorção no Ensino Fundamental

- Observa-se um aumento progressivo da distorção ao longo dos anos escolares:
  - 1º Ano: 2,1%
  - 5º Ano: 11,1%
  - 9º Ano: 15,6%

### Taxas de Distorção no Ensino Médio

- Observa-se uma diminuição na taxa de distorção ao longo das séries do Ensino Médio:
  - 1ª Série: 21,3%
  - 2ª Série: 18,2%
  - 3ª Série: 13,4%
- Essa redução pode estar associada ao abandono escolar, que faz com que alunos com maior distorção não cheguem às séries finais

### Comparativo entre os níveis de ensino

- A taxa de distorção no Ensino Médio é consistentemente maior que no Ensino Fundamental em todas as regiões
- A diferença é de aproximadamente 6-9 pontos percentuais entre os dois níveis
- Observa-se um crescimento de 121,1% da distorção dos Anos Iniciais (7,1%) para os Anos Finais (15,7%) do Ensino Fundamental
- O crescimento é de 13,4% dos Anos Finais do Fundamental (15,7%) para o Ensino Médio (17,8%)
- O Ensino Médio apresenta a maior Taxa de Distorção Idade-Série (17,8%), indicando que o problema se intensifica à medida que os estudantes avançam no sistema educacional

## Metodologia

A análise foi realizada utilizando:

- Python como linguagem de programação
- Pandas para manipulação e análise de dados
- Matplotlib e Seaborn para visualizações gráficas
- Openpyxl para geração do arquivo Excel de resultados

O tratamento dos dados envolveu:

1. Carregamento e limpeza dos dados
2. Renomeação de colunas para facilitar a análise
3. Análises estatísticas descritivas
4. Criação de visualizações para identificar padrões e tendências
5. Organização dos resultados em um arquivo Excel estruturado

## Resultados Gerados

Os resultados da análise foram salvos na pasta `Resultados_TDI`, incluindo:

- Gráficos comparativos entre regiões
- Visualizações da progressão da distorção por ano/série
- Tabelas com dados estatísticos relevantes
- Arquivo Excel (`distorcao_idade_serie.xlsx`) contendo os dados organizados em 4 planilhas:
  - Dados Brasil: Visão geral dos dados do Brasil
  - Ensino Fundamental: Dados por ano do ensino fundamental
  - Ensino Médio: Dados por série do ensino médio
  - Comparativo: Comparação entre os diferentes níveis de ensino

## Análise e Implicações

### Análise do Comparativo entre Níveis de Ensino

- A Taxa de Distorção Idade-Série cresce 121,1% dos Anos Iniciais para os Anos Finais do Ensino Fundamental
- A Taxa de Distorção Idade-Série cresce 13,4% dos Anos Finais do Ensino Fundamental para o Ensino Médio
- O Ensino Médio apresenta a maior Taxa de Distorção Idade-Série (17,8%), indicando que o problema se intensifica à medida que os estudantes avançam no sistema educacional

### Implicações e Considerações

- O aumento progressivo da distorção idade-série sugere um efeito cumulativo de reprovações e abandonos ao longo da trajetória escolar
- As transições entre níveis de ensino (do fundamental para o médio) parecem ser momentos críticos onde a distorção se intensifica
- Políticas educacionais específicas podem ser necessárias para cada etapa, com atenção especial ao Ensino Médio, onde o problema é mais acentuado
- A redução da distorção nas séries finais do Ensino Médio pode estar relacionada à evasão escolar, sugerindo que os alunos em situação de maior distorção tendem a abandonar os estudos antes de concluir esta etapa

## Conclusões

A análise da Taxa de Distorção Idade-Série no Brasil revela:

- Disparidades regionais significativas, com Norte e Nordeste apresentando taxas mais elevadas
- Aumento progressivo da distorção ao longo da trajetória escolar, principalmente na transição dos Anos Iniciais para os Anos Finais do Ensino Fundamental
- Ensino Médio com taxas consideravelmente mais altas que o Ensino Fundamental
- Necessidade de políticas educacionais focadas nos anos finais do Ensino Fundamental e no Ensino Médio
- Efeito cumulativo de reprovações e abandonos ao longo da trajetória escolar
- Momentos críticos de transição entre níveis de ensino, onde a distorção se intensifica
- Possível relação entre a redução da distorção nas séries finais do Ensino Médio e a evasão escolar

Estes dados podem auxiliar na formulação de políticas públicas educacionais voltadas à redução da distorção idade-série e melhoria da qualidade do ensino no Brasil.

## Arquivos

- `AnaliseDadosTDI.ipynb`: Notebook Jupyter com toda a análise e visualizações
- `Resultados_TDI/`: Pasta contendo as imagens e arquivos gerados pela análise
  - `distorcao_idade_serie.xlsx`: Arquivo Excel com os dados tratados e organizados
  - `comparativo_niveis_ensino.png`: Gráfico comparativo entre os diferentes níveis de ensino
  - Diversos outros gráficos em formato PNG
- `Datasets/TDI_BRASIL_REGIOES_UFS_2024.xlsx`: Arquivo de dados original (não incluído no repositório)
