# Diario de Bordo Memória

## Disco Rígido

### **Oque São:**
É um dispositivo de armazenamento de dados eletromecânico que armazena e recupera dados digitais usando armazenamento magnético e um ou mais pratos rígidos de rotação rápida revestidos com material magnético.
Os pratos são emparelhados com cabeças magnéticas, geralmente dispostas em um braço atuador móvel, que lê e grava dados nas superfícies dos pratos. Os dados são acessados de maneira aleatória, o que significa que blocos individuais de dados podem ser armazenados e recuperados em qualquer ordem. Os HDDs são um tipo de armazenamento não volátil, retendo os dados armazenados mesmo quando desligados.

### **Como Funciona:**

Um HDD moderno grava dados magnetizando um filme fino de material ferromagnético. em ambos os lados de um disco. Mudanças sequenciais na diretação da magnetização representavam bits de dados binátios. Os dados são lidos do disco detectando as transições na magnetização. Os dados do usuário são codificados usando um esquema de codificação, como codificação limitada por comprimento de execução, que determina como os dados são representados pelas transições magnéticas.

Um projeto de HDD típico consiste em um fuso que contém discos circulares planos, chamados de pratos, que armazenam os dados gravados. Os pratos são feitos de um material não magnético, geralmente liga de alumínio, vidro ou cerâmica. Eles são revestidos com uma camada rasa de material magnético tipicamente de 10 a 20 nm de profundidade, com uma camada externa de carbono para proteção. Para referência, um pedaço de papel de cópia padrão tem 0,07-0,18 mm (70.000-180.000 nm) de espessura.

As informações são gravadas e lidas em um prato à medida que ele gira em torno de dispositivos chamados cabeças de leitura e gravação que são posicionadas para operar muito perto da superfície magnética, com sua altura de vôo geralmente na faixa de dezenas de nanômetros. A cabeça de leitura e gravação é usada para detectar e modificar a magnetização do material que passa imediatamente sob ela.

[fonte](https://pt.wikipedia.org/wiki/Unidade_de_disco_r%C3%ADgido)

## Cache da CPU

###  **Oque São:**
é um cache de hardware usado pela CPU para reduzir o custo médio (tempo ou energia) de acesso a dados da memória principal.

Um cache é uma memória menor e mais rápida, localizada mais perto de um núcleo de processador , que armazena cópias dos dados de locais de memória principal frequentemente usados , evitando a necessidade de sempre consultar a memória principal, cujo acesso pode ser dezenas ou centenas de vezes mais lento.

A maioria das CPUs possui uma hierarquia de múltiplos níveis de cache (L1, L2, frequentemente L3 e raramente até mesmo L4), com caches específicos para instruções (cache I) e caches específicos para dados (cache D) separados no nível 1.

Os diferentes níveis são implementados em diferentes áreas do chip; o L1 está localizado o mais próximo possível de um núcleo da CPU e, portanto, oferece a maior velocidade devido aos curtos caminhos de sinal, mas requer um projeto cuidadoso. Os caches L2 são fisicamente separados da CPU e operam mais lentamente, mas impõem menos exigências ao projetista do chip e podem ser muito maiores sem impactar o projeto da CPU. Os caches L3 são geralmente compartilhados entre múltiplos núcleos da CPU.

[fonte](https://en.wikipedia.org/wiki/CPU_cache)

### **Como Funciona:**

Os dados são transferidos entre a memória e o cache em blocos de tamanho fixo, chamados linhas de cache ou blocos de cache . Quando uma linha de cache é copiada da memória para o cache, uma entrada de cache é criada. A entrada de cache incluirá os dados copiados, bem como a localização de memória solicitada (chamada de tag).

Quando o processador precisa ler ou escrever em um endereço de memória, ele primeiro verifica se existe uma entrada correspondente no cache. O cache verifica o conteúdo do endereço de memória solicitado em quaisquer linhas de cache que possam conter esse endereço. Se o processador encontrar o endereço de memória no cache, ocorreu um acerto de cache . No entanto, se o processador não encontrar o endereço de memória no cache, ocorreu uma falha de cache . No caso de um acerto de cache, o processador lê ou escreve imediatamente os dados na linha de cache. Para uma falha de cache, o cache aloca uma nova entrada e copia os dados da memória principal; em seguida, a solicitação é atendida com o conteúdo do cache.

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

### **Como Funciona:**
Armazena dados temporariamente na memória RAM para melhorar o sempenho do computador e agilizar a reprodução.
É ativada pelo sistema quando há uma diferença entre a taxa de recebimento e processamento de dados ou, alguns caso, quando elas são variáveis.

Por exemplo, ao reproduzir um arquivo de áudio/vídeo pela internet, os primeiros 20% são carregados na memória buffer. Enquanto essa porcentagem está sendo reproduzida, o computador baixa o restante do arquivo e o armazena novamente no buffer. Assim, se houver um congestionamento na rede, as chances de ocorrer travamentos são menores, já que a reprodução não depende diretamente da internet.

Pode aprimorar o desempenho do computador no disco rígido e placa de vídeo, em acesso eficiente aos dados ou sendo carregados antes de serem exibidos.

[fonte](https://tecnoblog.net/responde/o-que-e-buffer/)
