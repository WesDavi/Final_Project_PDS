# Análise da influência dos movimentos oculares em sinais de EEG

Além dos ruídos de natureza técnica, biopotenciais indesejados, oriundos da atividade elétrica em outras partes do corpo humano, podem interferir significativamente na leitura do potencial elétrico que descreve a atividade neuronal no eletroencefalograma (EEG) (NIDAL; MALIK, 2014).

Esses ruídos, geralmente chamados de artefatos, são originados de fontes diversas como:
- Piscadas ou movimento do globo ocular
- Atividade muscular da cabeça: pescoço e mandíbula
- Atividade cardíaca

## Motivações

- O processo de filtragem minimiza a interferência artefatos que prejudicam a qualidade dos sinais de EEG para fins de estudos científicos.
- Além disso, existem fenômenos fisiológicos que ocorrem em faixas de frequências específicas, que podem ser selecionadas através de processos de filtragem.
- Não obstante, a interferência dos artefatos presentes nos sinais de EEG tem impactos negativos consideráveis em sistemas de Interface Cérebro Máquina (ICM) baseados nesses biosinais, as quais buscam interpretar as atividades cerebrais para fins de comunicação ou interação com o ambiente externo.

## Objetivo

Desenvolver um filtro capaz de minimizar a interferência de biopotenciais indesejados, mais especificamente o movimento do globo ocular, nos sinais de EEG.

## Tecnologias Usadas

Para o desenvolvimento do projeto foi necessário a utilização das seguintes tecnologias open source:

- Python3
- Colab Notebook
- Numpy
- Scipy
- Matplotlib

## Instalação

Este projeto pode ser executado de maneira direta, basta baixar o arquivo project.ipynb e carregalo em seu Colab Notebook.
Caso deseje executar em máquina local realize a clonagem do repositório e as modificações necessárias.

 - Clonagem do repositório:
shell
$ git clone https://github.com/danilosl/Learning-PDS.git


## Resultados

<p align="center">
  <img src="https://github.com/danilosl/Learning-PDS/raw/main/img/sinais_brutos.svg"/>
  <img src="https://github.com/danilosl/Learning-PDS/raw/main/img/sinais_filtrados.svg"/>
</p>

Este projeto, buscou percorrer os principais tópicos relacionados a projeção de filtros digitais, juntamente com um estudo de caso da influência do biopotencial indesejado dos movimentos oculares em sinais de EEG, afim de contribuir com a melhor compressão da problemática e propor um filtro capaz de minimizar essa influência.

O filtro projetado apresentou resultados promissores, entretanto, na banda de passagem do filtro, ainda se encontram influências dos movimentos oculares. Como trabalhos futuros é sugerido a agregação de outras técnicas de remoção de artefatos dos sinais de EEG, como o método Local SSA (Local Singular Spectrum Analysis) que remove os artefatos oculares sem perder amostras do sinal.

## Referências

>[1] DE NORONHA AMABILE, Renato Augusto. Remoção de artefatos e análise de parâmetros espectrais em sinais de EEG: efeitos do fármaco flunitrazepam. 2008.
>
>[2] DUTRA, O. O. Um Amplificador Neural de baixo ruído e baixa potência utilizando uma topologia Folded Cascode OTA com malha de realimentação PID e ganho ajustável para EEG SoC Arrays. 2012. 85 f. Dissertação (Mestrado) - Curso de Engenharia Elétrica, Universidade Federal de Itajubá, Itajubá, 2012.
>
>[3] LATHI, Bhagwandas Pannalal. Sinais e sistemas lineares-2. Bookman, 2006.
>
>[4] NIDAL, Kamel; MALIK, Aamir Saeed (Ed.). EEG/ERP analysis: methods and applications. Crc Press, 2014.
>
>[5] OPPENHEIM, Alan V.; SCHAFER, Ronald W. Processamento em tempo discreto de sinais. Tradução Daniel Vieira. 3ª ed.-São Paulo: Pearson Education do Brasil, 2012.
>
>[6] Romero, S., Mañanas, M. A., & Barbanoj, M. J. (2008). A comparative study of automatic techniques for ocular artifact reduction in spontaneous EEG signals based on clinical target variables: a simulation case. Computers in biology and medicine, 38(3), 348-360.
>
>[7] Urigüen, J. A., & Garcia-Zapirain, B. (2015). EEG artifact removal—state-of-the-art and guidelines. Journal of neural engineering, 12(3), 031001.

## Links Úteis
>BCI Competition IV:
>https://www.bbci.de/competition/iv/#dataset2a
>
>Repositório da ferramenta pyfda no GitHub:
>https://github.com/chipmuenk/pyfda
