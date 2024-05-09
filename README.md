
<h1>Análise do Campeonato Brasileiro de Futebol</h1>

<h2>Objetivo</h2>

<p>Este projeto realiza uma análise exploratória de dados (EDA) sobre o Campeonato Brasileiro de Futebol, utilizando dados obtidos do Kaggle. O objetivo é entender as tendências de vitórias entre times mandantes e visitantes, e visualizar a distribuição de gols ao longo do tempo, diferenciando entre mandante e visitante.</p>

<h2>Dataset</h2>

<p>Os dados utilizados neste projeto foram obtidos do seguinte conjunto de dados no Kaggle: <a href="https://www.kaggle.com/datasets/adaoduque/campeonato-brasileiro-de-futebol">https://www.kaggle.com/datasets/adaoduque/campeonato-brasileiro-de-futebol</a></p>

<p>Dois arquivos CSV foram utilizados:</p>
<ul>
  <li><code>campeonato-brasileiro-full.csv</code>: Contém informações completas sobre as partidas, incluindo o vencedor, mandante, visitante, e outras estatísticas.</li>
  <li><code>campeonato-brasileiro-gols.csv</code>: Detalha os gols marcados em cada partida, com informações como clube, jogador, e minuto do gol.</li>
</ul>

<h2>Bibliotecas</h2>

<p>As seguintes bibliotecas Python foram utilizadas para análise e visualização:</p>
<ul>
  <li>pandas: Para manipulação e análise de dados.</li>
  <li>matplotlib: Para criação de gráficos.</li>
</ul>

<h2>Análise</h2>

<p>O código realiza duas análises principais:</p>

<h3>1. Comparação de Vitórias:</h3>
<ul>
  <li>Uma função é criada para classificar cada partida como vitória do mandante, visitante ou empate, com base na coluna "vencedor" do dataframe <code>campeonato-brasileiro-full.csv</code>.</li>
  <li>Em seguida, um gráfico de barras é gerado para visualizar a contagem de vitórias de mandantes versus visitantes.</li>
</ul>

<h3>2. Distribuição de Gols:</h3>
<ul>
  <li>O dataframe <code>campeonato-brasileiro-gols.csv</code> é carregado e a coluna "partida_id" é renomeada para "ID" para facilitar a junção com o outro dataframe.</li>
  <li>Uma função é definida para determinar se cada gol foi marcado pelo time mandante ou visitante, com base no ID da partida e nas informações do dataframe <code>campeonato-brasileiro-full.csv</code>.</li>
  <li>Os minutos dos gols são processados para lidar com casos onde há minutos adicionais indicados por um sinal "+".</li>
  <li>Filtra-se as últimas 15 partidas para analisar a distribuição de gols em jogos recentes.</li>
  <li>Um gráfico de dispersão é criado, mostrando a distribuição dos gols ao longo do tempo, com cores diferentes para gols de mandantes e visitantes.</li>
</ul>

<h2>Conclusões</h2>

<p>A análise fornece insights sobre o desempenho de mandantes e visitantes no Campeonato Brasileiro e permite visualizar padrões na distribuição de gols ao longo das partidas.</p>

<h2>Próximos Passos</h2>
<ul>
  <li>Explorar outras variáveis do conjunto de dados, como placar final, número de cartões, etc.</li>
  <li>Analisar tendências ao longo de diferentes temporadas ou campeonatos.</li>
  <li>Implementar técnicas de aprendizado de máquina para prever resultados de jogos ou desempenho de jogadores.</li>
</ul>
