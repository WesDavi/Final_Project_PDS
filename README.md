# Programa feito em Python com objetivo de remover ruídos presentes en arquyivos de áudio

Ao se gravar um audio pode ser que no mesmo tenha ruídos, esses ruídos geralmente podem ser capturados no momento da gravação do áudio, alguns dispositivos 
de gravação possuem de fábrica filtros que minimizam os ruídos, tendo em vista que ainda assim, alguns ruídos ainda possam ser capturados.
Tendo em vista amenizar ruídos que possam ser capturados na gravação de um áudio, o presente trabalho visa a criação de um sistema capaz de amenizar ruídos
sem perder a mensagem principal do arquivo que sera filtrado.

## Motivações

- O processo de filtragem minimiza a interferência de ruídos que prejudicam a qualidade dos sinais analisados.
- Além disso, uso e emprego de conhecimentos de Processamento Digital de Sinais, fazendo uso de um filtro passa-baixa.
- Não obstante, a interferência de ruídos externos no momento da gravação de um áudio pode fazer com que a mensagem principal não seja entendida pelo ouvinte.

## Objetivo

Desenvolver um filtro capaz de minimizar a interferência de ruídos e barulhos indesejados, na gravação de um áudio.

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
$ git clone https://github.com/WesDavi/Final_Project_PDS


## Resultados

Este projeto, buscou reduzir de forma suscinta e sem grandes perdas da mensagem principal a redução ou eliminação de ruídos e/ou barulhos que possam prejudicar a mensagem principal que esta tentando ser passada. Foi utilizado um filtro passa-baixa, fazendo com que o mesmo passasse apenas sinais a baixo da banda de corte, essa analise de onde o filtro deve agir deve ser feita pelo usuário ao observar no dominio da frequência onde está presente o ruído e apartir disso visar eliminar o ruído (não existe possibilidade de eliminar o mesmo 100% porém deve-se tentar minimizar o ruído ao máximo).

O filtro projetado apresentou resultados promissores, tendo em vista que no arquivo de áudio utilizado o ruído foi eliminado quase que 100% mostrando, dessa forma que o filtro passa-baixa cumrpiu com o objetivo principal do trabalho em questão.

## Referências

>[1] DE NORONHA AMABILE, Renato Augusto. Remoção de artefatos e análise de parâmetros espectrais em sinais de EEG: efeitos do fármaco flunitrazepam. 2008.
>
>[3] LATHI, Bhagwandas Pannalal. Sinais e sistemas lineares-2. Bookman, 2006.
>
>[4] NIDAL, Kamel; MALIK, Aamir Saeed (Ed.). EEG/ERP analysis: methods and applications. Crc Press, 2014.
>
>[5] OPPENHEIM, Alan V.; SCHAFER, Ronald W. Processamento em tempo discreto de sinais. Tradução Daniel Vieira. 3ª ed.-São Paulo: Pearson Education do Brasil, 2012.
