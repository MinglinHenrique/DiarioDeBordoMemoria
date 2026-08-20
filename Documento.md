# Diario de Bordo Memória

## Disco Rígido

### **Oque São:**
É um dispositivo de armazenamento de dados eletromecânico que armazena e recupera dados digitais usando armazenamento magnético e um ou mais pratos rígidos de rotação rápida revestidos com material magnético.
Os pratos são emparelhados com cabeças magnéticas, geralmente dispostas em um braço atuador móvel, que lê e grava dados nas superfícies dos pratos. Os dados são acessados de maneira aleatória, o que significa que blocos individuais de dados podem ser armazenados e recuperados em qualquer ordem. Os HDDs são um tipo de armazenamento não volátil, retendo os dados armazenados mesmo quando desligados.

### **Como Funciona:**

Um HDD moderno grava dados magnetizando um filme fino de material ferromagnético em ambos os lados de um disco. Mudanças sequenciais na direção da magnetização representam bits de dados binários. Os dados são lidos do disco detectando as transições na magnetização. Os dados do usuário são codificados usando um esquema de codificação, como codificação limitada por comprimento de execução, que determina como os dados são representados pelas transições magnéticas.

Um projeto de HDD típico consiste em um fuso que contém discos circulares planos, chamados de pratos, que armazenam os dados gravados. Os pratos são feitos de um material não magnético, geralmente liga de alumínio, vidro ou cerâmica. Eles são revestidos com uma camada rasa de material magnético tipicamente de 10 a 20 nm de profundidade, com uma camada externa de carbono para proteção. Para referência, um pedaço de papel de cópia padrão tem 0,07-0,18 mm (70.000-180.000 nm) de espessura.

As informações são gravadas e lidas em um prato à medida que ele gira em torno de dispositivos chamados cabeças de leitura e gravação que são posicionadas para operar muito perto da superfície magnética, com sua altura de vôo geralmente na faixa de dezenas de nanômetros. A cabeça de leitura e gravação é usada para detectar e modificar a magnetização do material que passa imediatamente sob ela.

## Cache da CPU

### **Oque São:**
É um cache de hardware usado pela CPU para reduzir o custo médio (tempo ou energia) de acesso a dados da memória principal.

Um cache é uma memória menor e mais rápida, localizada mais perto de um núcleo de processador, que armazena cópias dos dados de locais de memória principal frequentemente usados, evitando a necessidade de sempre consultar a memória principal, cujo acesso pode ser dezenas ou centenas de vezes mais lento.

A maioria das CPUs possui uma hierarquia de múltiplos níveis de cache (L1, L2, frequentemente L3 e raramente até mesmo L4), com caches específicos para instruções (cache I) e caches específicos para dados (cache D) separados no nível 1.

Os diferentes níveis são implementados em diferentes áreas do chip; o L1 está localizado o mais próximo possível de um núcleo da CPU e, portanto, oferece a maior velocidade devido aos curtos caminhos de sinal, mas requer um projeto cuidadoso. Os caches L2 estão localizados no mesmo chip, porém mais distantes do núcleo, operando mais lentamente que o L1, mas impondo menos exigências ao projetista e podendo ser muito maiores sem impactar tanto o projeto do núcleo. Os caches L3 são geralmente compartilhados entre múltiplos núcleos da CPU.

### **Como Funciona:**

Os dados são transferidos entre a memória e o cache em blocos de tamanho fixo, chamados linhas de cache ou blocos de cache. Quando uma linha de cache é copiada da memória para o cache, uma entrada de cache é criada. A entrada de cache incluirá os dados copiados, bem como a localização de memória solicitada (chamada de tag).

Quando o processador precisa ler ou escrever em um endereço de memória, ele primeiro verifica se existe uma entrada correspondente no cache. O cache verifica o conteúdo do endereço de memória solicitado em quaisquer linhas de cache que possam conter esse endereço. Se o processador encontrar o endereço de memória no cache, ocorreu um acerto de cache. No entanto, se o processador não encontrar o endereço de memória no cache, ocorreu uma falha de cache. No caso de um acerto de cache, o processador lê ou escreve imediatamente os dados na linha de cache. Para uma falha de cache, o cache aloca uma nova entrada e copia os dados da memória principal; em seguida, a solicitação é atendida com o conteúdo do cache.

## Registradores de memória da CPU

### **Oque são?**
O registrador de uma UCP (unidade central de processamento) é a memória dentro da própria CPU que armazena bits.
Os registradores estão no topo da hierarquia de memória, sendo assim, é um tipo de memória mais rápida e financeiramente mais custosa. Apesar do alto custo por bit armazenado, sua velocidade de acesso é essencial para o funcionamento dos computadores modernos e, portanto, são incluídos, ainda que em menor capacidade, mesmo em processadores de baixo custo.
Os registradores são circuitos digitais capazes de armazenar e deslocar informações binárias, e são tipicamente usados como um dispositivo de armazenamento temporário.

Nos dias de hoje os computadores necessitam de muito mais espaço para armazenar as informações em todos os tipos de memória, a partir desse momento, as informações que são armazenadas por conjuntos de dígitos binários nos sistemas digitais internos do computador também tem que ser maior, ocupando um espaço de 32 ou 64 bits, sendo que em períodos mais antigos essa memória dos conjuntos de dígitos binários possuía 8 ou 16 bits.

Os sistemas digitais necessitam de comunicação com a parte de hardware do computador, para que seja armazenado nos conjuntos de dígitos binários.
Dentro dos sistemas digitais temos os circuitos digitais capazes de realizar o armazenamento de informações sendo eles os registradores.

### **Como Funciona:**
São utilizados na execução de programas de computadores, disponibilizando um local para armazenar dados. Na maioria dos computadores modernos, quando da execução das instruções de um programa, os dados são deslocados da memória principal para os registradores.
As instruções que utilizam estes dados são executadas pelo processador e, finalmente, os dados são movidos de volta para a memória principal.

## Memória Flash

### **Oque é:**
É um tipo de memória não volátil que mantém o armazenamento mesmo sem uma fonte de energia.
Permite escrita e leitura em nível de byte, mas a exclusão (apagamento) de dados só pode ser feita em blocos inteiros — essa é justamente a característica que distingue a memória flash de outras EEPROMs.
São amplamente utilizados e armazenam dados para finalidades muito específicas.
Atualmente assume algumas das funções anteriormente reservadas às EEPROMs e memórias ROM. Por exemplo, ao ligar um computador, a BIOS/UEFI hoje é armazenada e executada a partir de um chip de memória flash na placa-mãe.

### **Como Funciona:**
A memória flash armazena dados em células de memória flash baseadas em transistores de porta flutuante. As células de memória dos chips de memória flash são compostas por transistores, que atuam como interruptores de roteamento da corrente elétrica que passa por aquela célula de memória flash.

Os chips de memória flash são organizados em grades, semelhantes a blocos urbanos. As células de memória são distribuídas em linhas, conhecidas como bit lines. Nas interseções desses chips há um transistor. Cada transistor possui duas portas (gates).

Uma delas é a porta de controle, que fica na camada superior do transistor. A outra porta é chamada de porta flutuante: ela fica entre a porta de controle e o canal do transistor, isolada por camadas de óxido acima e abaixo — por isso ela "flutua" eletricamente, retendo carga mesmo sem energia.

Além disso, há uma camada fina de separação entre a porta de controle e a porta flutuante, conhecida como camada de óxido.
A quantidade específica de memória flash determina se o uso dessa memória se enquadra em uma classificação de baixa, média ou alta densidade. Gravações com densidade mais alta refletem maiores quantidades de memória flash.

## Buffer de instruções da CPU

### **Oque É:**
É uma pequena região de memória de altíssima velocidade dentro (ou muito próxima) do núcleo da CPU, usada para armazenar temporariamente as instruções já buscadas na memória, antes de serem decodificadas e executadas. Diferente de um buffer genérico de I/O (como o de streaming de vídeo), esse buffer opera dentro do pipeline de instruções do processador.

### **Como Funciona:**
Enquanto a CPU executa uma instrução, o estágio de busca (fetch) já adianta a leitura das próximas instruções da memória/cache e as deposita nesse buffer. Isso evita que o núcleo fique ocioso esperando cada instrução chegar da memória a cada ciclo, mantendo o pipeline de execução abastecido continuamente.

Esse mecanismo é essencial para técnicas como *pipelining* e *pré-busca de instruções* (instruction prefetching): ao manter um estoque de instruções já buscadas, o processador reduz bolhas no pipeline causadas pela latência de acesso à memória principal, aumentando o throughput de execução.
