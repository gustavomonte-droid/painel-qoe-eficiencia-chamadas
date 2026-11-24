# Painel QoE - Eficiencia de Chamadas

Dashboard em Power BI para acompanhar a eficiencia de chamadas (QoE) de uma rede movel, por estado, regional e tecnologia (2G/3G, 4G VoLTE e 5G voNR).

> Os dados deste projeto sao **simulados**. Nao ha informacoes reais de nenhuma operadora.

## O que o painel mostra
- Eficiencia da semana atual e variacao contra a semana anterior, por tecnologia
- Evolucao da eficiencia ao longo do tempo
- Eficiencia vs. meta de QoE (92%)
- Os 8 piores estados em eficiencia
- Mapa do Brasil com semaforo por estado (vermelho abaixo de 93%, amarelo entre 93% e 93,5%, verde acima)
- Distribuicao de tentativas por tecnologia

## Arquivos
- Eficiencia de chamadas.pbix: relatorio Power BI (a Pagina 4 e o painel executivo)
- 	elecom_rede_movel.xlsx: base de dados simulada, 27 estados
- undo_painel_qoe.png: imagem de fundo do painel

## Ferramentas
Power BI Desktop, DAX, Excel, Git e GitHub.

Autor: Gustavo Almeida
