# Comparing `tmp/b3fileparser-0.1.6.tar.gz` & `tmp/b3fileparser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3fileparser-0.1.6.tar", max compression
+gzip compressed data, was "b3fileparser-0.2.0.tar", max compression
```

## Comparing `b3fileparser-0.1.6.tar` & `b3fileparser-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/LICENSE
--rw-r--r--   0        0        0    12480 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/b3fileparser/__init__.py
--rw-r--r--   0        0        0     3984 2024-05-20 23:38:12.075313 b3fileparser-0.1.6/b3fileparser/b3_meta_data.py
--rw-r--r--   0        0        0     3101 2024-05-21 00:43:49.374664 b3fileparser-0.1.6/b3fileparser/b3parser.py
--rw-r--r--   0        0        0      422 2024-05-21 11:56:57.815597 b3fileparser-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    13035 1970-01-01 00:00:00.000000 b3fileparser-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-20 13:09:26.899061 b3fileparser-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12057 2024-05-25 21:17:54.094849 b3fileparser-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 13:09:26.899061 b3fileparser-0.2.0/b3fileparser/__init__.py
+-rw-r--r--   0        0        0     3982 2024-05-25 18:00:30.634980 b3fileparser-0.2.0/b3fileparser/b3_meta_data.py
+-rw-r--r--   0        0        0     1029 2024-05-25 21:04:41.830745 b3fileparser-0.2.0/b3fileparser/b3parser.py
+-rw-r--r--   0        0        0     2827 2024-05-25 17:23:05.674178 b3fileparser-0.2.0/b3fileparser/b3parser_base.py
+-rw-r--r--   0        0        0     2340 2024-05-25 17:48:53.632977 b3fileparser-0.2.0/b3fileparser/b3parser_pandas.py
+-rw-r--r--   0        0        0     1712 2024-05-25 20:34:47.385480 b3fileparser-0.2.0/b3fileparser/b3parser_polars.py
+-rw-r--r--   0        0        0      442 2024-05-25 21:24:17.657166 b3fileparser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12654 1970-01-01 00:00:00.000000 b3fileparser-0.2.0/PKG-INFO
```

### Comparing `b3fileparser-0.1.6/LICENSE` & `b3fileparser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.1.6/README.md` & `b3fileparser-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 # b3fileparser
 
 A função dessa biblioteca é fazer o parser do arquivo com cotações históricas da B3, disponíveis em https://www.b3.com.br/pt_br/market-data-e-indices/servicos-de-dados/market-data/historico/mercado-a-vista/cotacoes-historicas/
 
 ## Instalação
 
 Instalação pode ser feita via pip
+
 ```
 pip install b3fileparser
 ```
+
 ## Exemplo 1
+
 ```python
-from b3fileparser import b3parser
+from b3fileparser.b3parser import B3Parser
 
 
-dados_b3 = b3parser.read_b3_file('COTAHIST_A2023.TXT')
+parser = B3Parser.create_parser(engine='pandas')
+dados_b3 = parser.read_b3_file('COTAHIST_A2023.TXT')
 dados_b3
 ```
-`dados_b3` é um DataFrame pandas:
-
-|    |   TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI          | CODIGO_DE_NEGOCIACAO   | TIPO_DE_MERCADO   | NOME_DA_EMPRESA   | ESPECIFICACAO_DO_PAPEL   |   PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA   |   PRECO_DE_ABERTURA |   PRECO_MAXIMO |   PRECO_MINIMO |   PRECO_MEDIO |   PRECO_ULTIMO_NEGOCIO |   PRECO_MELHOR_OFERTA_DE_COMPRA |   PRECO_MELHOR_OFERTA_DE_VENDAS |   NUMERO_DE_NEGOCIOS |   QUANTIDADE_NEGOCIADA |   VOLUME_TOTAL_NEGOCIADO |   PRECO_DE_EXERCICIO |   INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO   |   FATOR_DE_COTACAO |   PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN   |   NUMERO_DE_DISTRIBUICAO |
-|---:|-------------------:|:--------------------|:--------------------|:-----------------------|:------------------|:------------------|:-------------------------|-----------------------------------:|:----------------------|--------------------:|---------------:|---------------:|--------------:|-----------------------:|--------------------------------:|--------------------------------:|---------------------:|-----------------------:|-------------------------:|---------------------:|----------------------------------:|:---------------------|-------------------:|-------------------------------:|:--------------|-------------------------:|
-|  1 |                  1 | 2023-01-02 00:00:00 | 34                  | MMMC34                 | VISTA             | 3M                | DRN                      |                                 -1 | R$                    |              165.56 |         165.56 |         159.06 |        160.97 |                 161.44 |                          161.44 |                          161.59 |                   31 |           120          |          20443.2         |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRMMMCBDR000  |                      143 |
-|  2 |                  1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | RRRP3                  | VISTA             | 3R PETROLEUM      | ON      NM               |                                 -1 | R$                    |               37.24 |          37.93 |          35.97 |         36.64 |                  36.41 |                           36.4  |                           36.41 |                13731 |             2.8788e+06 |              1.05483e+08 |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRRRRPACNOR5  |                      100 |
-|  3 |                  1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | RRRP3F                 | FRACIONARIO       | 3R PETROLEUM      | ON      NM               |                                 -1 | R$                    |               37.75 |          37.91 |          35.98 |         36.69 |                  36.94 |                           36.94 |                           37    |                 1309 |         24010          |         881003           |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRRRRPACNOR5  |                      100 |
-|  4 |                  1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | TTEN3                  | VISTA             | 3TENTOS           | ON      NM               |                                 -1 | R$                    |                9.65 |           9.65 |           9.07 |          9.23 |                   9.36 |                            9.35 |                            9.36 |                 3292 |        701700          |              6.48253e+06 |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRTTENACNOR0  |                      101 |
-|  5 |                  1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | TTEN3F                 | FRACIONARIO       | 3TENTOS           | ON      NM               |                                 -1 | R$                    |                9.34 |           9.44 |           9.08 |          9.26 |                   9.2  |                            9.2  |                            9.65 |                  238 |          4640          |          43069.7         |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRTTENACNOR0  |                      101 |
 
+> [!NOTE]
+> Pode-se obter os dados em formato DataFrame `Pandas` ou `Polars`
+> Configure engine para `engine='pandas'` ou `engine='polars'`
+
+`dados_b3` é um DataFrame:
+
+|     | TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI          | CODIGO_DE_NEGOCIACAO | TIPO_DE_MERCADO | NOME_DA_EMPRESA | ESPECIFICACAO_DO_PAPEL | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA | PRECO_DE_ABERTURA | PRECO_MAXIMO | PRECO_MINIMO | PRECO_MEDIO | PRECO_ULTIMO_NEGOCIO | PRECO_MELHOR_OFERTA_DE_COMPRA | PRECO_MELHOR_OFERTA_DE_VENDAS | NUMERO_DE_NEGOCIOS | QUANTIDADE_NEGOCIADA | VOLUME_TOTAL_NEGOCIADO | PRECO_DE_EXERCICIO | INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO | FATOR_DE_COTACAO | PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN  | NUMERO_DE_DISTRIBUICAO |
+| --: | ---------------: | :------------------ | :------------------ | :------------------- | :-------------- | :-------------- | :--------------------- | -------------------------------: | :------------------ | ----------------: | -----------: | -----------: | ----------: | -------------------: | ----------------------------: | ----------------------------: | -----------------: | -------------------: | ---------------------: | -----------------: | ------------------------------: | :----------------- | ---------------: | ---------------------------: | :----------- | ---------------------: |
+|   1 |                1 | 2023-01-02 00:00:00 | 34                  | MMMC34               | VISTA           | 3M              | DRN                    |                               -1 | R$                  |            165.56 |       165.56 |       159.06 |      160.97 |               161.44 |                        161.44 |                        161.59 |                 31 |                  120 |                20443.2 |                  0 |                               0 | NaT                |                1 |                            0 | BRMMMCBDR000 |                    143 |
+|   2 |                1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | RRRP3                | VISTA           | 3R PETROLEUM    | ON NM                  |                               -1 | R$                  |             37.24 |        37.93 |        35.97 |       36.64 |                36.41 |                          36.4 |                         36.41 |              13731 |           2.8788e+06 |            1.05483e+08 |                  0 |                               0 | NaT                |                1 |                            0 | BRRRRPACNOR5 |                    100 |
+|   3 |                1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | RRRP3F               | FRACIONARIO     | 3R PETROLEUM    | ON NM                  |                               -1 | R$                  |             37.75 |        37.91 |        35.98 |       36.69 |                36.94 |                         36.94 |                            37 |               1309 |                24010 |                 881003 |                  0 |                               0 | NaT                |                1 |                            0 | BRRRRPACNOR5 |                    100 |
+|   4 |                1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | TTEN3                | VISTA           | 3TENTOS         | ON NM                  |                               -1 | R$                  |              9.65 |         9.65 |         9.07 |        9.23 |                 9.36 |                          9.35 |                          9.36 |               3292 |               701700 |            6.48253e+06 |                  0 |                               0 | NaT                |                1 |                            0 | BRTTENACNOR0 |                    101 |
+|   5 |                1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | TTEN3F               | FRACIONARIO     | 3TENTOS         | ON NM                  |                               -1 | R$                  |              9.34 |         9.44 |         9.08 |        9.26 |                  9.2 |                           9.2 |                          9.65 |                238 |                 4640 |                43069.7 |                  0 |                               0 | NaT                |                1 |                            0 | BRTTENACNOR0 |                    101 |
 
 ## Exemplo 2 - Listando Opções de Venda da Petrobras
+
 ```python
-from b3fileparser import b3parser
+from b3fileparser.b3parser import B3Parser
 
 
-dados = b3parser.read_b3_file('COTAHIST_A2023.TXT')
+parser = B3Parser.create_parser()
+dados = parser.read_b3_file('COTAHIST_A2023.TXT')
 puts = dados[dados['TIPO_DE_MERCADO'] == 'OPCOES_DE_VENDA']
 putspetro = puts[puts['CODIGO_DE_NEGOCIACAO'].str.startswith('PETR')]
 putspetro.head()
 ```
-|       |   TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI      | CODIGO_DE_NEGOCIACAO   | TIPO_DE_MERCADO   | NOME_DA_EMPRESA   | ESPECIFICACAO_DO_PAPEL   |   PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA   |   PRECO_DE_ABERTURA |   PRECO_MAXIMO |   PRECO_MINIMO |   PRECO_MEDIO |   PRECO_ULTIMO_NEGOCIO |   PRECO_MELHOR_OFERTA_DE_COMPRA |   PRECO_MELHOR_OFERTA_DE_VENDAS |   NUMERO_DE_NEGOCIOS |   QUANTIDADE_NEGOCIADA |   VOLUME_TOTAL_NEGOCIADO |   PRECO_DE_EXERCICIO |   INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO   |   FATOR_DE_COTACAO |   PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN   |   NUMERO_DE_DISTRIBUICAO |
-|------:|-------------------:|:--------------------|:----------------|:-----------------------|:------------------|:------------------|:-------------------------|-----------------------------------:|:----------------------|--------------------:|---------------:|---------------:|--------------:|-----------------------:|--------------------------------:|--------------------------------:|---------------------:|-----------------------:|-------------------------:|---------------------:|----------------------------------:|:---------------------|-------------------:|-------------------------------:|:--------------|-------------------------:|
-| 24653 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM318               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.17 |           0.22 |           0.17 |          0.19 |                   0.18 |                               0 |                               0 |                   66 |                  68100 |                    13008 |                21.91 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      196 |
-| 24654 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM328               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.16 |           0.3  |           0.16 |          0.21 |                   0.29 |                               0 |                               0 |                   52 |                  47800 |                    10127 |                22.91 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      196 |
-| 24655 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRN282               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                1.11 |           1.11 |           1.07 |          1.1  |                   1.07 |                               0 |                               0 |                    9 |                  22000 |                    24340 |                24.98 |                                 0 | 2023-02-17 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 |
-| 24656 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM28                | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.69 |           1.03 |           0.69 |          0.97 |                   1    |                               0 |                               1 |                   26 |                  69600 |                    68155 |                25.66 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 |
-| 24657 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM294               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                1.09 |           1.23 |           1.04 |          1.11 |                   1.08 |                               0 |                               0 |                   12 |                   7700 |                     8616 |                26.16 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 | 
 
+|       | TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI      | CODIGO_DE_NEGOCIACAO | TIPO_DE_MERCADO | NOME_DA_EMPRESA | ESPECIFICACAO_DO_PAPEL | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA | PRECO_DE_ABERTURA | PRECO_MAXIMO | PRECO_MINIMO | PRECO_MEDIO | PRECO_ULTIMO_NEGOCIO | PRECO_MELHOR_OFERTA_DE_COMPRA | PRECO_MELHOR_OFERTA_DE_VENDAS | NUMERO_DE_NEGOCIOS | QUANTIDADE_NEGOCIADA | VOLUME_TOTAL_NEGOCIADO | PRECO_DE_EXERCICIO | INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO  | FATOR_DE_COTACAO | PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN  | NUMERO_DE_DISTRIBUICAO |
+| ----: | ---------------: | :------------------ | :-------------- | :------------------- | :-------------- | :-------------- | :--------------------- | -------------------------------: | :------------------ | ----------------: | -----------: | -----------: | ----------: | -------------------: | ----------------------------: | ----------------------------: | -----------------: | -------------------: | ---------------------: | -----------------: | ------------------------------: | :------------------ | ---------------: | ---------------------------: | :----------- | ---------------------: |
+| 24653 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM318             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.17 |         0.22 |         0.17 |        0.19 |                 0.18 |                             0 |                             0 |                 66 |                68100 |                  13008 |              21.91 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    196 |
+| 24654 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM328             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.16 |          0.3 |         0.16 |        0.21 |                 0.29 |                             0 |                             0 |                 52 |                47800 |                  10127 |              22.91 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    196 |
+| 24655 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRN282             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              1.11 |         1.11 |         1.07 |         1.1 |                 1.07 |                             0 |                             0 |                  9 |                22000 |                  24340 |              24.98 |                               0 | 2023-02-17 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
+| 24656 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM28              | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.69 |         1.03 |         0.69 |        0.97 |                    1 |                             0 |                             1 |                 26 |                69600 |                  68155 |              25.66 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
+| 24657 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM294             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              1.09 |         1.23 |         1.04 |        1.11 |                 1.08 |                             0 |                             0 |                 12 |                 7700 |                   8616 |              26.16 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
 
 ## Sobre os dados
+
 O parse do arquivo é realizado de acordo com o Layout fornecido pela b3: https://www.b3.com.br/data/files/33/67/B9/50/D84057102C784E47AC094EA8/SeriesHistoricas_Layout.pdf
 
 ### Colunas
-|    | COLUNA                           |   TAMANHO NO ARQUIVO TXT |
-|---:|:---------------------------------|-------------------------:|
-|  0 | TIPO_DE_REGISTRO                 |                        2 |
-|  1 | DATA_DO_PREGAO                   |                        8 |
-|  2 | CODIGO_BDI                       |                        2 |
-|  3 | CODIGO_DE_NEGOCIACAO             |                       12 |
-|  4 | TIPO_DE_MERCADO                  |                        3 |
-|  5 | NOME_DA_EMPRESA                  |                       12 |
-|  6 | ESPECIFICACAO_DO_PAPEL           |                       10 |
-|  7 | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO |                        3 |
-|  8 | MOEDA_DE_REFERENCIA              |                        4 |
-|  9 | PRECO_DE_ABERTURA                |                       13 |
-| 10 | PRECO_MAXIMO                     |                       13 |
-| 11 | PRECO_MINIMO                     |                       13 |
-| 12 | PRECO_MEDIO                      |                       13 |
-| 13 | PRECO_ULTIMO_NEGOCIO             |                       13 |
-| 14 | PRECO_MELHOR_OFERTA_DE_COMPRA    |                       13 |
-| 15 | PRECO_MELHOR_OFERTA_DE_VENDAS    |                       13 |
-| 16 | NUMERO_DE_NEGOCIOS               |                        5 |
-| 17 | QUANTIDADE_NEGOCIADA             |                       18 |
-| 18 | VOLUME_TOTAL_NEGOCIADO           |                       18 |
-| 19 | PRECO_DE_EXERCICIO               |                       13 |
-| 20 | INDICADOR_DE_CORRECAO_DE_PRECOS  |                        1 |
-| 21 | DATA_DE_VENCIMENTO               |                        8 |
-| 22 | FATOR_DE_COTACAO                 |                        7 |
-| 23 | PRECO_DE_EXERCICIO_EM_PONTOS     |                       13 |
-| 24 | CODIGO_ISIN                      |                       12 |
-| 25 | NUMERO_DE_DISTRIBUICAO           |                        3 |
+
+|     | COLUNA                           | TAMANHO NO ARQUIVO TXT |
+| --: | :------------------------------- | ---------------------: |
+|   0 | TIPO_DE_REGISTRO                 |                      2 |
+|   1 | DATA_DO_PREGAO                   |                      8 |
+|   2 | CODIGO_BDI                       |                      2 |
+|   3 | CODIGO_DE_NEGOCIACAO             |                     12 |
+|   4 | TIPO_DE_MERCADO                  |                      3 |
+|   5 | NOME_DA_EMPRESA                  |                     12 |
+|   6 | ESPECIFICACAO_DO_PAPEL           |                     10 |
+|   7 | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO |                      3 |
+|   8 | MOEDA_DE_REFERENCIA              |                      4 |
+|   9 | PRECO_DE_ABERTURA                |                     13 |
+|  10 | PRECO_MAXIMO                     |                     13 |
+|  11 | PRECO_MINIMO                     |                     13 |
+|  12 | PRECO_MEDIO                      |                     13 |
+|  13 | PRECO_ULTIMO_NEGOCIO             |                     13 |
+|  14 | PRECO_MELHOR_OFERTA_DE_COMPRA    |                     13 |
+|  15 | PRECO_MELHOR_OFERTA_DE_VENDAS    |                     13 |
+|  16 | NUMERO_DE_NEGOCIOS               |                      5 |
+|  17 | QUANTIDADE_NEGOCIADA             |                     18 |
+|  18 | VOLUME_TOTAL_NEGOCIADO           |                     18 |
+|  19 | PRECO_DE_EXERCICIO               |                     13 |
+|  20 | INDICADOR_DE_CORRECAO_DE_PRECOS  |                      1 |
+|  21 | DATA_DE_VENCIMENTO               |                      8 |
+|  22 | FATOR_DE_COTACAO                 |                      7 |
+|  23 | PRECO_DE_EXERCICIO_EM_PONTOS     |                     13 |
+|  24 | CODIGO_ISIN                      |                     12 |
+|  25 | NUMERO_DE_DISTRIBUICAO           |                      3 |
 
 ### Tipos de mercado
-|    | TIPO DE MERCADO                  |
-|---:|:---------------------------------|
-| 10 | VISTA                            |
-| 12 | EXERCICIO DE OPCOES DE COMPRA    |
-| 13 | EXERCÍCIO DE OPCOES DE VENDA     |
-| 17 | LEILAO                           |
-| 20 | FRACIONARIO                      |
-| 30 | TERMO                            |
-| 50 | FUTURO_COM_RETENCAO_DE_GANHO     |
-| 60 | FUTURO_COM_MOVIMENTACAO_CONTINUA |
-| 70 | OPCOES_DE_COMPRA                 |
-| 80 | OPCOES_DE_VENDA                  |
+
+|     | TIPO DE MERCADO                  |
+| --: | :------------------------------- |
+|  10 | VISTA                            |
+|  12 | EXERCICIO DE OPCOES DE COMPRA    |
+|  13 | EXERCÍCIO DE OPCOES DE VENDA     |
+|  17 | LEILAO                           |
+|  20 | FRACIONARIO                      |
+|  30 | TERMO                            |
+|  50 | FUTURO_COM_RETENCAO_DE_GANHO     |
+|  60 | FUTURO_COM_MOVIMENTACAO_CONTINUA |
+|  70 | OPCOES_DE_COMPRA                 |
+|  80 | OPCOES_DE_VENDA                  |
```

### Comparing `b3fileparser-0.1.6/b3fileparser/b3_meta_data.py` & `b3fileparser-0.2.0/b3fileparser/b3_meta_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 META_DATA = {    
-    "TIPREG":{'name':"TIPO_DE_REGISTRO", 'size':2, 'dtype':'category'},
+    "TIPREG":{'name':"TIPO_DE_REGISTRO", 'size':2, 'dtype':'object'},
     "DATAPR":{'name':"DATA_DO_PREGAO", 'size':8, 'dtype': 'object'},
     "CODBDI":{'name':"CODIGO_BDI", 'size':2, 'dtype':'category'},
     "CODNEG":{'name':"CODIGO_DE_NEGOCIACAO",'size':12,'dtype':'category'},
     "TPMERC":{'name':"TIPO_DE_MERCADO",'size':3, 'dtype':'category'},
     "NOMRES":{'name':"NOME_DA_EMPRESA",'size':12, 'dtype':'category'},
     "ESPECI":{'name':"ESPECIFICACAO_DO_PAPEL",'size':10, 'dtype':'category'},
     "PRAZOT":{'name':"PRAZO_EM_DIAS_DO_MERCADO_A_TERMO",'size':3, 'dtype':'object'},
```

### Comparing `b3fileparser-0.1.6/b3fileparser/b3parser.py` & `b3fileparser-0.2.0/b3fileparser/b3parser_pandas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,61 @@
+from .b3parser_base import B3ParserBase
 import pandas as pd
-from b3fileparser import b3_meta_data
-from zipfile import ZipFile
-from io import BytesIO
-import os
-
-def _post_processing(df, divide_by_100=True):
-    for col in df.columns:
-        if ('PRECO_' in col or 'VOLUME' in col) and divide_by_100:
-            df[col] = df[col] / 100
-        if 'DATA' in col:
-            df[col] = df[col].apply(lambda x: pd.NaT if x == "99991231" else x )
-            df[col] = pd.to_datetime(df[col])         
-        if col == "TIPO_DE_MERCADO":
-            df[col] = df[col].apply(lambda x: b3_meta_data.MARKETS.get(x, x))
-        if col == "INDICADOR_DE_CORRECAO_DE_PRECOS":
-            df[col] = df[col].apply(lambda x: b3_meta_data.INDOPC.get(x, x))
-        if col == "CODIGO_BDI":
-            df[col] = df[col].apply(lambda x: b3_meta_data.CODBDI.get(x, x))
-    return df
-
-def read_b3_file(file_path, file_type='path'):
-    """
-    Reads financial data from a Brazilian B3 file, supporting both plaintext and zipped formats.
-
-    Parameters:
-        file_path (str): Path or bytes of the file to be read.
-        file_type (str): 'path' if `file_path` is a filesystem path, 'bytes' if `file_path` is bytes data.
-
-    Returns:
-        pandas.DataFrame: Parsed data as a DataFrame, or None if an error occurs.
-
-    Raises:
-        ValueError: If the file format is not supported or `file_type` is invalid.
-
-    Examples:
-        # Read data from a TXT file
-        df = read_b3_file('/path/to/file.TXT')
-
-        # Read data from a ZIP file containing a TXT file
-        df = read_b3_file('/path/to/file.ZIP')
-
-        # Read data from bytes
-        df = read_b3_file(b'raw binary data from file', file_type='bytes')
-    """
-    # Validate the file type parameter
-    if file_type not in ['path', 'bytes']:
-        raise ValueError("Invalid file_type specified. Choose 'path' or 'bytes'.")
-
-    # Prepare columns and their sizes based on metadata
-    meta_data = pd.DataFrame(data=b3_meta_data.META_DATA.values())
-    dtypes = {row[1]:row[2] for row in meta_data[['name','dtype']].itertuples()}
+
+
+class B3ParserPandas(B3ParserBase):
+    def read_b3_file(self, file_path, file_type='path') -> pd.DataFrame:
+        """
+        Reads financial data from a Brazilian B3 file, supporting both plaintext and zipped formats.
+
+        Parameters:
+            file_path (str): Path or bytes of the file to be read.
+            file_type (str): 'path' if `file_path` is a filesystem path, 'bytes' if `file_path` is bytes data.
+
+        Returns:
+            pandas.DataFrame: Parsed data as a DataFrame, or None if an error occurs.
+
+        Raises:
+            ValueError: If the file format is not supported or `file_type` is invalid.
+
+        Examples:
+            # Read data from a TXT file
+            df = read_b3_file('/path/to/file.TXT')
+
+            # Read data from a ZIP file containing a TXT file
+            df = read_b3_file('/path/to/file.ZIP')
+
+            # Read data from bytes
+            df = read_b3_file(b'raw binary data from file', file_type='bytes')
+        """
+        meta_data = super()._load_meta_data()
+        file = super()._load_file(file_path, file_type)        
+
+        # Read and parse the file
+        b3_data = pd.read_fwf(
+            file,
+            header=None,
+            names=meta_data['names'],
+            widths=meta_data['sizes'],
+            dtype=meta_data['dtypes'],        
+            encoding='latin1',
+        )[1:-1]  # Skip potential header and footer rows
+
+        # Post-process the data
+        b3_data = self._post_processing(b3_data, meta_data)    
+        return b3_data
     
-    # Handle file input based on type
-    if file_type == 'path':
-        if not file_path.lower().endswith(('.txt', '.zip')):
-            raise ValueError('Invalid file format! Provide a .TXT or .ZIP file containing a .TXT')
-        
-        if file_path.lower().endswith('.zip'):
-            with ZipFile(file_path, 'r') as file_zip:
-                # Assuming the TXT file has the same base name as the ZIP file
-                txt_filename = os.path.basename(file_path).replace('.ZIP', '.TXT')
-                file = BytesIO(file_zip.read(txt_filename))
-        else:
-            file = file_path
-
-    elif file_type == 'bytes':
-        file = BytesIO(file_path)
-
-    # Read and parse the file
-    b3_data = pd.read_fwf(
-        file,
-        header=None,
-        names=meta_data['name'].to_list(),
-        widths=meta_data['size'].to_list(),
-        dtype=dtypes,        
-        encoding='latin1',
-    )[1:-1]  # Skip potential header and footer rows
-
-    # Post-process the data
-    b3_data = _post_processing(b3_data)    
-    return b3_data
+    def _post_processing(self, df, meta_data):
+        for col in df.columns:
+            if ('PRECO_' in col or 'VOLUME' in col):
+                df[col] = df[col] / 100
+            if 'DATA' in col:
+                df[col] = df[col].apply(lambda x: pd.NaT if x == "99991231" else x )
+                df[col] = pd.to_datetime(df[col])         
+            if col == "TIPO_DE_MERCADO":
+                df[col] = df[col].apply(lambda x: meta_data["MARKETS"].get(x, x))
+            if col == "INDICADOR_DE_CORRECAO_DE_PRECOS":
+                df[col] = df[col].apply(lambda x: meta_data["INDOPC"].get(x, x))
+            if col == "CODIGO_BDI":
+                df[col] = df[col].apply(lambda x: meta_data["CODBDI"].get(x, x))
+        return df
+
```

### Comparing `b3fileparser-0.1.6/PKG-INFO` & `b3fileparser-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,125 @@
 Metadata-Version: 2.1
 Name: b3fileparser
-Version: 0.1.6
+Version: 0.2.0
 Summary: A Python parser of Brazilian exchange B3 historical data files
 License: MIT
 Author: codigoquant
 Author-email: codigoquant@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: polars (>=0.20.29,<0.21.0)
 Description-Content-Type: text/markdown
 
 # b3fileparser
 
 A função dessa biblioteca é fazer o parser do arquivo com cotações históricas da B3, disponíveis em https://www.b3.com.br/pt_br/market-data-e-indices/servicos-de-dados/market-data/historico/mercado-a-vista/cotacoes-historicas/
 
 ## Instalação
 
 Instalação pode ser feita via pip
+
 ```
 pip install b3fileparser
 ```
+
 ## Exemplo 1
+
 ```python
-from b3fileparser import b3parser
+from b3fileparser.b3parser import B3Parser
 
 
-dados_b3 = b3parser.read_b3_file('COTAHIST_A2023.TXT')
+parser = B3Parser.create_parser(engine='pandas')
+dados_b3 = parser.read_b3_file('COTAHIST_A2023.TXT')
 dados_b3
 ```
-`dados_b3` é um DataFrame pandas:
-
-|    |   TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI          | CODIGO_DE_NEGOCIACAO   | TIPO_DE_MERCADO   | NOME_DA_EMPRESA   | ESPECIFICACAO_DO_PAPEL   |   PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA   |   PRECO_DE_ABERTURA |   PRECO_MAXIMO |   PRECO_MINIMO |   PRECO_MEDIO |   PRECO_ULTIMO_NEGOCIO |   PRECO_MELHOR_OFERTA_DE_COMPRA |   PRECO_MELHOR_OFERTA_DE_VENDAS |   NUMERO_DE_NEGOCIOS |   QUANTIDADE_NEGOCIADA |   VOLUME_TOTAL_NEGOCIADO |   PRECO_DE_EXERCICIO |   INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO   |   FATOR_DE_COTACAO |   PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN   |   NUMERO_DE_DISTRIBUICAO |
-|---:|-------------------:|:--------------------|:--------------------|:-----------------------|:------------------|:------------------|:-------------------------|-----------------------------------:|:----------------------|--------------------:|---------------:|---------------:|--------------:|-----------------------:|--------------------------------:|--------------------------------:|---------------------:|-----------------------:|-------------------------:|---------------------:|----------------------------------:|:---------------------|-------------------:|-------------------------------:|:--------------|-------------------------:|
-|  1 |                  1 | 2023-01-02 00:00:00 | 34                  | MMMC34                 | VISTA             | 3M                | DRN                      |                                 -1 | R$                    |              165.56 |         165.56 |         159.06 |        160.97 |                 161.44 |                          161.44 |                          161.59 |                   31 |           120          |          20443.2         |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRMMMCBDR000  |                      143 |
-|  2 |                  1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | RRRP3                  | VISTA             | 3R PETROLEUM      | ON      NM               |                                 -1 | R$                    |               37.24 |          37.93 |          35.97 |         36.64 |                  36.41 |                           36.4  |                           36.41 |                13731 |             2.8788e+06 |              1.05483e+08 |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRRRRPACNOR5  |                      100 |
-|  3 |                  1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | RRRP3F                 | FRACIONARIO       | 3R PETROLEUM      | ON      NM               |                                 -1 | R$                    |               37.75 |          37.91 |          35.98 |         36.69 |                  36.94 |                           36.94 |                           37    |                 1309 |         24010          |         881003           |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRRRRPACNOR5  |                      100 |
-|  4 |                  1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | TTEN3                  | VISTA             | 3TENTOS           | ON      NM               |                                 -1 | R$                    |                9.65 |           9.65 |           9.07 |          9.23 |                   9.36 |                            9.35 |                            9.36 |                 3292 |        701700          |              6.48253e+06 |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRTTENACNOR0  |                      101 |
-|  5 |                  1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | TTEN3F                 | FRACIONARIO       | 3TENTOS           | ON      NM               |                                 -1 | R$                    |                9.34 |           9.44 |           9.08 |          9.26 |                   9.2  |                            9.2  |                            9.65 |                  238 |          4640          |          43069.7         |                    0 |                                 0 | NaT                  |                  1 |                              0 | BRTTENACNOR0  |                      101 |
 
+> [!NOTE]
+> Pode-se obter os dados em formato DataFrame `Pandas` ou `Polars`
+> Configure engine para `engine='pandas'` ou `engine='polars'`
+
+`dados_b3` é um DataFrame:
+
+|     | TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI          | CODIGO_DE_NEGOCIACAO | TIPO_DE_MERCADO | NOME_DA_EMPRESA | ESPECIFICACAO_DO_PAPEL | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA | PRECO_DE_ABERTURA | PRECO_MAXIMO | PRECO_MINIMO | PRECO_MEDIO | PRECO_ULTIMO_NEGOCIO | PRECO_MELHOR_OFERTA_DE_COMPRA | PRECO_MELHOR_OFERTA_DE_VENDAS | NUMERO_DE_NEGOCIOS | QUANTIDADE_NEGOCIADA | VOLUME_TOTAL_NEGOCIADO | PRECO_DE_EXERCICIO | INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO | FATOR_DE_COTACAO | PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN  | NUMERO_DE_DISTRIBUICAO |
+| --: | ---------------: | :------------------ | :------------------ | :------------------- | :-------------- | :-------------- | :--------------------- | -------------------------------: | :------------------ | ----------------: | -----------: | -----------: | ----------: | -------------------: | ----------------------------: | ----------------------------: | -----------------: | -------------------: | ---------------------: | -----------------: | ------------------------------: | :----------------- | ---------------: | ---------------------------: | :----------- | ---------------------: |
+|   1 |                1 | 2023-01-02 00:00:00 | 34                  | MMMC34               | VISTA           | 3M              | DRN                    |                               -1 | R$                  |            165.56 |       165.56 |       159.06 |      160.97 |               161.44 |                        161.44 |                        161.59 |                 31 |                  120 |                20443.2 |                  0 |                               0 | NaT                |                1 |                            0 | BRMMMCBDR000 |                    143 |
+|   2 |                1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | RRRP3                | VISTA           | 3R PETROLEUM    | ON NM                  |                               -1 | R$                  |             37.24 |        37.93 |        35.97 |       36.64 |                36.41 |                          36.4 |                         36.41 |              13731 |           2.8788e+06 |            1.05483e+08 |                  0 |                               0 | NaT                |                1 |                            0 | BRRRRPACNOR5 |                    100 |
+|   3 |                1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | RRRP3F               | FRACIONARIO     | 3R PETROLEUM    | ON NM                  |                               -1 | R$                  |             37.75 |        37.91 |        35.98 |       36.69 |                36.94 |                         36.94 |                            37 |               1309 |                24010 |                 881003 |                  0 |                               0 | NaT                |                1 |                            0 | BRRRRPACNOR5 |                    100 |
+|   4 |                1 | 2023-01-02 00:00:00 | LOTE_PADRAO         | TTEN3                | VISTA           | 3TENTOS         | ON NM                  |                               -1 | R$                  |              9.65 |         9.65 |         9.07 |        9.23 |                 9.36 |                          9.35 |                          9.36 |               3292 |               701700 |            6.48253e+06 |                  0 |                               0 | NaT                |                1 |                            0 | BRTTENACNOR0 |                    101 |
+|   5 |                1 | 2023-01-02 00:00:00 | MERCADO FRACIONARIO | TTEN3F               | FRACIONARIO     | 3TENTOS         | ON NM                  |                               -1 | R$                  |              9.34 |         9.44 |         9.08 |        9.26 |                  9.2 |                           9.2 |                          9.65 |                238 |                 4640 |                43069.7 |                  0 |                               0 | NaT                |                1 |                            0 | BRTTENACNOR0 |                    101 |
 
 ## Exemplo 2 - Listando Opções de Venda da Petrobras
+
 ```python
-from b3fileparser import b3parser
+from b3fileparser.b3parser import B3Parser
 
 
-dados = b3parser.read_b3_file('COTAHIST_A2023.TXT')
+parser = B3Parser.create_parser()
+dados = parser.read_b3_file('COTAHIST_A2023.TXT')
 puts = dados[dados['TIPO_DE_MERCADO'] == 'OPCOES_DE_VENDA']
 putspetro = puts[puts['CODIGO_DE_NEGOCIACAO'].str.startswith('PETR')]
 putspetro.head()
 ```
-|       |   TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI      | CODIGO_DE_NEGOCIACAO   | TIPO_DE_MERCADO   | NOME_DA_EMPRESA   | ESPECIFICACAO_DO_PAPEL   |   PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA   |   PRECO_DE_ABERTURA |   PRECO_MAXIMO |   PRECO_MINIMO |   PRECO_MEDIO |   PRECO_ULTIMO_NEGOCIO |   PRECO_MELHOR_OFERTA_DE_COMPRA |   PRECO_MELHOR_OFERTA_DE_VENDAS |   NUMERO_DE_NEGOCIOS |   QUANTIDADE_NEGOCIADA |   VOLUME_TOTAL_NEGOCIADO |   PRECO_DE_EXERCICIO |   INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO   |   FATOR_DE_COTACAO |   PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN   |   NUMERO_DE_DISTRIBUICAO |
-|------:|-------------------:|:--------------------|:----------------|:-----------------------|:------------------|:------------------|:-------------------------|-----------------------------------:|:----------------------|--------------------:|---------------:|---------------:|--------------:|-----------------------:|--------------------------------:|--------------------------------:|---------------------:|-----------------------:|-------------------------:|---------------------:|----------------------------------:|:---------------------|-------------------:|-------------------------------:|:--------------|-------------------------:|
-| 24653 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM318               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.17 |           0.22 |           0.17 |          0.19 |                   0.18 |                               0 |                               0 |                   66 |                  68100 |                    13008 |                21.91 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      196 |
-| 24654 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM328               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.16 |           0.3  |           0.16 |          0.21 |                   0.29 |                               0 |                               0 |                   52 |                  47800 |                    10127 |                22.91 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      196 |
-| 24655 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRN282               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                1.11 |           1.11 |           1.07 |          1.1  |                   1.07 |                               0 |                               0 |                    9 |                  22000 |                    24340 |                24.98 |                                 0 | 2023-02-17 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 |
-| 24656 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM28                | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                0.69 |           1.03 |           0.69 |          0.97 |                   1    |                               0 |                               1 |                   26 |                  69600 |                    68155 |                25.66 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 |
-| 24657 |                  1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM294               | OPCOES_DE_VENDA   | PETRE             | ON      N2               |                                  0 | R$                    |                1.09 |           1.23 |           1.04 |          1.11 |                   1.08 |                               0 |                               0 |                   12 |                   7700 |                     8616 |                26.16 |                                 0 | 2023-01-20 00:00:00  |                  1 |                              0 | BRPETRACNOR9  |                      197 | 
 
+|       | TIPO_DE_REGISTRO | DATA_DO_PREGAO      | CODIGO_BDI      | CODIGO_DE_NEGOCIACAO | TIPO_DE_MERCADO | NOME_DA_EMPRESA | ESPECIFICACAO_DO_PAPEL | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO | MOEDA_DE_REFERENCIA | PRECO_DE_ABERTURA | PRECO_MAXIMO | PRECO_MINIMO | PRECO_MEDIO | PRECO_ULTIMO_NEGOCIO | PRECO_MELHOR_OFERTA_DE_COMPRA | PRECO_MELHOR_OFERTA_DE_VENDAS | NUMERO_DE_NEGOCIOS | QUANTIDADE_NEGOCIADA | VOLUME_TOTAL_NEGOCIADO | PRECO_DE_EXERCICIO | INDICADOR_DE_CORRECAO_DE_PRECOS | DATA_DE_VENCIMENTO  | FATOR_DE_COTACAO | PRECO_DE_EXERCICIO_EM_PONTOS | CODIGO_ISIN  | NUMERO_DE_DISTRIBUICAO |
+| ----: | ---------------: | :------------------ | :-------------- | :------------------- | :-------------- | :-------------- | :--------------------- | -------------------------------: | :------------------ | ----------------: | -----------: | -----------: | ----------: | -------------------: | ----------------------------: | ----------------------------: | -----------------: | -------------------: | ---------------------: | -----------------: | ------------------------------: | :------------------ | ---------------: | ---------------------------: | :----------- | ---------------------: |
+| 24653 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM318             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.17 |         0.22 |         0.17 |        0.19 |                 0.18 |                             0 |                             0 |                 66 |                68100 |                  13008 |              21.91 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    196 |
+| 24654 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM328             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.16 |          0.3 |         0.16 |        0.21 |                 0.29 |                             0 |                             0 |                 52 |                47800 |                  10127 |              22.91 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    196 |
+| 24655 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRN282             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              1.11 |         1.11 |         1.07 |         1.1 |                 1.07 |                             0 |                             0 |                  9 |                22000 |                  24340 |              24.98 |                               0 | 2023-02-17 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
+| 24656 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM28              | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              0.69 |         1.03 |         0.69 |        0.97 |                    1 |                             0 |                             1 |                 26 |                69600 |                  68155 |              25.66 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
+| 24657 |                1 | 2023-01-02 00:00:00 | OPCOES_DE_VENDA | PETRM294             | OPCOES_DE_VENDA | PETRE           | ON N2                  |                                0 | R$                  |              1.09 |         1.23 |         1.04 |        1.11 |                 1.08 |                             0 |                             0 |                 12 |                 7700 |                   8616 |              26.16 |                               0 | 2023-01-20 00:00:00 |                1 |                            0 | BRPETRACNOR9 |                    197 |
 
 ## Sobre os dados
+
 O parse do arquivo é realizado de acordo com o Layout fornecido pela b3: https://www.b3.com.br/data/files/33/67/B9/50/D84057102C784E47AC094EA8/SeriesHistoricas_Layout.pdf
 
 ### Colunas
-|    | COLUNA                           |   TAMANHO NO ARQUIVO TXT |
-|---:|:---------------------------------|-------------------------:|
-|  0 | TIPO_DE_REGISTRO                 |                        2 |
-|  1 | DATA_DO_PREGAO                   |                        8 |
-|  2 | CODIGO_BDI                       |                        2 |
-|  3 | CODIGO_DE_NEGOCIACAO             |                       12 |
-|  4 | TIPO_DE_MERCADO                  |                        3 |
-|  5 | NOME_DA_EMPRESA                  |                       12 |
-|  6 | ESPECIFICACAO_DO_PAPEL           |                       10 |
-|  7 | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO |                        3 |
-|  8 | MOEDA_DE_REFERENCIA              |                        4 |
-|  9 | PRECO_DE_ABERTURA                |                       13 |
-| 10 | PRECO_MAXIMO                     |                       13 |
-| 11 | PRECO_MINIMO                     |                       13 |
-| 12 | PRECO_MEDIO                      |                       13 |
-| 13 | PRECO_ULTIMO_NEGOCIO             |                       13 |
-| 14 | PRECO_MELHOR_OFERTA_DE_COMPRA    |                       13 |
-| 15 | PRECO_MELHOR_OFERTA_DE_VENDAS    |                       13 |
-| 16 | NUMERO_DE_NEGOCIOS               |                        5 |
-| 17 | QUANTIDADE_NEGOCIADA             |                       18 |
-| 18 | VOLUME_TOTAL_NEGOCIADO           |                       18 |
-| 19 | PRECO_DE_EXERCICIO               |                       13 |
-| 20 | INDICADOR_DE_CORRECAO_DE_PRECOS  |                        1 |
-| 21 | DATA_DE_VENCIMENTO               |                        8 |
-| 22 | FATOR_DE_COTACAO                 |                        7 |
-| 23 | PRECO_DE_EXERCICIO_EM_PONTOS     |                       13 |
-| 24 | CODIGO_ISIN                      |                       12 |
-| 25 | NUMERO_DE_DISTRIBUICAO           |                        3 |
+
+|     | COLUNA                           | TAMANHO NO ARQUIVO TXT |
+| --: | :------------------------------- | ---------------------: |
+|   0 | TIPO_DE_REGISTRO                 |                      2 |
+|   1 | DATA_DO_PREGAO                   |                      8 |
+|   2 | CODIGO_BDI                       |                      2 |
+|   3 | CODIGO_DE_NEGOCIACAO             |                     12 |
+|   4 | TIPO_DE_MERCADO                  |                      3 |
+|   5 | NOME_DA_EMPRESA                  |                     12 |
+|   6 | ESPECIFICACAO_DO_PAPEL           |                     10 |
+|   7 | PRAZO_EM_DIAS_DO_MERCADO_A_TERMO |                      3 |
+|   8 | MOEDA_DE_REFERENCIA              |                      4 |
+|   9 | PRECO_DE_ABERTURA                |                     13 |
+|  10 | PRECO_MAXIMO                     |                     13 |
+|  11 | PRECO_MINIMO                     |                     13 |
+|  12 | PRECO_MEDIO                      |                     13 |
+|  13 | PRECO_ULTIMO_NEGOCIO             |                     13 |
+|  14 | PRECO_MELHOR_OFERTA_DE_COMPRA    |                     13 |
+|  15 | PRECO_MELHOR_OFERTA_DE_VENDAS    |                     13 |
+|  16 | NUMERO_DE_NEGOCIOS               |                      5 |
+|  17 | QUANTIDADE_NEGOCIADA             |                     18 |
+|  18 | VOLUME_TOTAL_NEGOCIADO           |                     18 |
+|  19 | PRECO_DE_EXERCICIO               |                     13 |
+|  20 | INDICADOR_DE_CORRECAO_DE_PRECOS  |                      1 |
+|  21 | DATA_DE_VENCIMENTO               |                      8 |
+|  22 | FATOR_DE_COTACAO                 |                      7 |
+|  23 | PRECO_DE_EXERCICIO_EM_PONTOS     |                     13 |
+|  24 | CODIGO_ISIN                      |                     12 |
+|  25 | NUMERO_DE_DISTRIBUICAO           |                      3 |
 
 ### Tipos de mercado
-|    | TIPO DE MERCADO                  |
-|---:|:---------------------------------|
-| 10 | VISTA                            |
-| 12 | EXERCICIO DE OPCOES DE COMPRA    |
-| 13 | EXERCÍCIO DE OPCOES DE VENDA     |
-| 17 | LEILAO                           |
-| 20 | FRACIONARIO                      |
-| 30 | TERMO                            |
-| 50 | FUTURO_COM_RETENCAO_DE_GANHO     |
-| 60 | FUTURO_COM_MOVIMENTACAO_CONTINUA |
-| 70 | OPCOES_DE_COMPRA                 |
-| 80 | OPCOES_DE_VENDA                  |
+
+|     | TIPO DE MERCADO                  |
+| --: | :------------------------------- |
+|  10 | VISTA                            |
+|  12 | EXERCICIO DE OPCOES DE COMPRA    |
+|  13 | EXERCÍCIO DE OPCOES DE VENDA     |
+|  17 | LEILAO                           |
+|  20 | FRACIONARIO                      |
+|  30 | TERMO                            |
+|  50 | FUTURO_COM_RETENCAO_DE_GANHO     |
+|  60 | FUTURO_COM_MOVIMENTACAO_CONTINUA |
+|  70 | OPCOES_DE_COMPRA                 |
+|  80 | OPCOES_DE_VENDA                  |
```

