# Diario de Bordo Memória

## Memória Flash

### **Oque é:**
é um tipo de memória não volátil que mantém o armazenamento mesmo sem uma fonte de energia.
permite regravações e exclusões de blocos de dados em nível de byte.
são amplamente utilizados e armazenam dados para finalidades muito específicas.
atualmente assume algumas das funções anteriormente reservadas aos discos rígidos. Por exemplo, ao ligar um computador, ele executa a BIOS.

### **Como Funciona:**
A memória flash armazena dados em células de memória flash baseadas em transistores de porta flutuantes. As células de memória dos chips de memória flash são compostas por transistores, que atuam como interruptores de roteamento da corrente elétrica que passa por aquela célula de memória flash.

Os chips de memória flash são organizados em grades, semelhantes a blocos urbanos. As células de memória são distribuídas em linhas, conhecidas como bit linesesses chips possuem interseções, e em cada interseção há um transistor. Cada transistor possui duas portas (gates).

Uma delas é a porta de controle, que fica na camada superior do transistor. A outra porta é chamada de porta flutuante, assim chamada porque ela efetivamente flutua entre a porta de controle e a camada superior do chip transistor MOSFET.

Além disso, há uma camada fina de separação entre a porta de controle e a porta flutuante, conhecida como camada de óxido.
A quantidade específica de memória flash determina se o uso dessa memória se enquadra em uma classificação de baixa, média ou alta densidade. Gravações com densidade mais alta refletem maiores quantidades de memória flash.

[fonte](https://www.ibm.com/br-pt/think/topics/flash-memory)

## Buffers de instrução

###  **Oque São:**
É uma região da memória física de um computador utilizada para armazenar dados temporariamente, tendo como finalidade manter as informações salvas antes de serem efetivamente usadas.

### ***Como Funciona:**
Armazena dados temporariamente na memória RAM para melhorar o sempenho do computador e agilizar a reprodução.
É ativada pelo sistema quando há uma diferença entre a taxa de recebimento e processamento de dados ou, alguns caso, quando elas são variáveis.

Por exemplo, ao reproduzir um arquivo de áudio/vídeo pela internet, os primeiros 20% são carregados na memória buffer. Enquanto essa porcentagem está sendo reproduzida, o computador baixa o restante do arquivo e o armazena novamente no buffer. Assim, se houver um congestionamento na rede, as chances de ocorrer travamentos são menores, já que a reprodução não depende diretamente da internet.

Pode aprimorar o desempenho do computador no disco rígido e placa de vídeo, em acesso eficiente aos dados ou sendo carregados antes de serem exibidos.
