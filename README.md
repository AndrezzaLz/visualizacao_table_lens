# Visualização de Dados Educacionais com Table Lens

Este repositório contém um trabalho prático focado na construção de visualizações de dados avançadas utilizando a técnica de Table Lens. O objetivo do projeto é demonstrar como representar múltiplas dimensões de dados (nominais, ordinais e quantitativos) simultaneamente de forma clara e comparativa.

A análise utiliza o conjunto de dados states_all.csv, que traz indicadores de receita, despesa e desempenho escolar (notas de matemática e leitura) dos estados norte-americanos.

## Tecnologias Utilizadas
- Python
- Pandas e NumPy para manipulação e categorização de dados
- Matplotlib para a construção da visualização customizada

## O que foi feito

O desenvolvimento foi estruturado nas seguintes etapas:

1. Seleção e Pré-processamento:
- Extração dos dados específicos do ano de 2015.
- Seleção das variáveis de foco: estado, receita total, despesa total e nota média em matemática (4ª série).
- Engenharia de atributos: criação da variável categórica ordinal NIVEL_MATH (Baixo, Médio, Alto) a partir da distribuição das notas.

2. Ordenação Estratégica:
- Os dados foram ordenados com base na Receita Total (TOTAL_REVENUE) de forma crescente, criando uma base sólida para a identificação de correlações visuais entre a verba do estado e o nível educacional.

3. Construção do Gráfico (Table Lens):
- Criação de uma matriz visual com múltiplos eixos (subplots) combinados.
- Representação nominal: nomes dos estados renderizados em texto alinhado.
- Representação ordinal: níveis de matemática mapeados por blocos de intensidade de cor.
- Representação quantitativa: receitas e despesas exibidas através do comprimento de barras horizontais.
- Omissão de eixos numéricos e bordas convencionais para simular uma tabela analítica imersiva e limpa.

## Como executar
1. Clone o repositório.
2. Certifique-se de ter o Python instalado com as bibliotecas pandas, numpy e matplotlib.
3. Atualize o caminho do arquivo states_all.csv no código para apontar para o diretório local correto.
4. Execute o notebook para rodar as células de pré-processamento e gerar a imagem final do Table Lens.
