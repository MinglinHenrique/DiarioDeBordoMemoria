# Projeto Diario de Bordo: Memória
<h2>Registradores</h2>

Os registradores são um tipo de memória de computador integrada diretamente ao processador ou CPU (Unidade Central de Processamento) que é usada para armazenar e manipular dados durante a execução de instruções. Um registrador pode armazenar uma instrução, um endereço de armazenamento ou qualquer tipo de dado (como uma sequência de bits ou caracteres individuais).
Os registradores também contêm circuitos de lógica de controle, que permitem coordenar o fluxo de dados e instruções dentro da CPU. Isso pode incluir operações como decodificação de sinais de controle, manipulação de dados (como carregamento, armazenamento ou operações aritméticas) e uso de multiplexadores para direcionar dados para um local específico dentro do registrador.


Tamanhos dos registradores da CPU

O número e o tamanho dos registradores em uma CPU são determinados pelo projeto do processador e podem ter um impacto significativo em seu desempenho e capacidades. A maioria dos processadores de computador modernos inclui:

•	Registradores de 8 bits: Esses registradores podem armazenar 8 bits de dados (1 byte). Eles são frequentemente usados para operações aritméticas básicas e manipulação de dados.

•	Registradores de 16 bits: Esses registradores podem armazenar 16 bits de dados (2 bytes). Eles são comumente encontrados em processadores mais antigos ou em arquiteturas específicas que exigem operações de 16 bits.

•	Registradores de 32 bits: Esses registradores podem armazenar 32 bits de dados (4 bytes). Eles são amplamente utilizados em muitos processadores e são capazes de lidar com tamanhos de dados maiores e cálculos mais complexos.

•	Registradores de 64 bits: Esses registradores podem armazenar 64 bits de dados (8 bytes). Eles são comuns em processadores modernos e oferecem maior poder computacional e capacidade de endereçamento de memória.

Os PCs modernos de hoje em dia geralmente possuem registradores de 32 bits ou 64 bits e são referidos como processadores de 32 bits e processadores de 64 bits, respectivamente. Isso indica o tamanho ou a largura dos registradores do processador e a quantidade de dados que o processador pode processar em uma única operação.


<h2>Cache</h2>
  
O cache, além de armazenar os dados temporários usados em um computador, tem como objetivo principal fornecer uma cópia mais rápida de dados frequentemente acessados, reduzindo assim o tempo de acesso aos mesmos. Ele possui três espaços de armazenamento:

O L1 é o mais rápido dos três por estar mais perto do processador, tendo a função de determinar a prioridade de acesso aos dados através do uso frequente deles pelo usuário. Ele também é o primeiro espaço em que o processador irá buscar informações.
O L2 age com um ponto secundário de armazenamento, guardando os dados mais recentes usados pelo usuário. Ele possui um espaço e velocidade menor do que o L1 pois está mais afastado do processador, mas como ambos estão ligados, o L1 pode pedir a transferências do L2 para si.
Ajudando no desempenho do L1 e L2, o L3 possui maior espaço e a menor velocidade dos três.
A memória secundária é aquela que está “fora” do processador ou sistema, e que permite o armazenamento de grandes quantidades de dados, mas com um acesso mais lento e sequencial; exemplos: HD, SSD, DVD, USB, etc.

O HD (Hard Disk Drive): é um dispositivo usado para o armazenamento de longo prazo em computadores pessoais, servidores e sistemas de armazenamento externo. Ele armazena dados de forma magnética em discos metálicos ou de vidro revestidos com material magnético (por isso também são chamados de “disco rígido“), além de oferecer capacidade significativa de armazenamento, mas pode ser mais suscetível a danos físicos devido às partes mecânicas móveis.

O SSD (Solid-state Drive): tendo o mesmo propósito do HD, o SSD não necessariamente é um substituto, mas com certeza uma alternativa menor, mais resistente, mais rápida e com melhor desempenho. Consistindo em chips de memória flash, ele não precisa realizar ações mecânicas para acessar os dados, o que resulta em tempos de acesso muito mais rápidos e taxas de transferência de dados mais elevadas que o HD

<h2>Memória RAM</h2>  
A RAM (Random Access Memory) é usada para armazenar os dados e programas que estão sendo executados pelo sistema no momento. Ela é dividida em células, cada uma com um endereço único, que podem ser acessadas em qualquer ordem pelo processador. Ela possui característica volátil, ou seja, perde os dados assim que é desconectado da energia.

<h2>Memória ROM</h2>
A ROM (Read-only Memory) é usada para armazenar os dados e programas que são essenciais para o funcionamento do computador, como a BIOS (Basic Input/Output System), que é o “programa” responsável por inicializar o computador e reconhecer os dispositivos conectados a ele. Diferente da RAM, nem todos os tipos dela podem ser alterados pelo usuário, apenas pelo fabricante, além de ter característica não voláteis, que mantem os dados mesmo quando o computador perde conexão com a energia.

<h2>Memória Primaria</h2>
O armazenamento primário é o componente encarregado de reter dados e instruções de programas que estão em uso ativo pelo processador de um computador.

O armazenamento primário também é conhecido como memória principal, retém quantidades relativamente pequenas de dados que o computador pode acessar enquanto opera. Devido à sua proximidade com a unidade central de processamento (CPU), é mais simples ler e gravar no armazenamento primário. Isso permite que os processadores forneçam acesso mais rápido aos dados e instruções que o armazenamento primário contém.

A diferença da memória externa, também conhecida como memória secundária, que envolve dispositivos de armazenamento que podem armazenar dados de forma contínua.
O armazenamento primário opera mantendo os dados e instruções que estão em uso atual pela CPU. Para executar programas, a CPU acessa o armazenamento primário para receber as instruções necessárias. O armazenamento primário é responsável por três tarefas operacionais essenciais ao processamento do computador.

<h3>Carregamento do sistema operacional (SO)</h3>  
Quando um computador é ligado, ele passa por um ciclo de inicialização no qual os componentes necessários do sistema operacional são adicionados à RAM a partir do disco rígido do computador. Depois que o SO estiver carregado, o sistema estará pronto para gerenciar as operações.

<h3>Execução de aplicativos</h3>
Antes que as aplicações possam ser executados, eles são primeiramente carregados do local existente no disco rígido para a RAM, que orquestra a execução do aplicativo e proporciona uma recuperação de dados mais rápida do que a que seria exibida originalmente.

<h3>Processamento de dados</h3>
Não são apenas os aplicativos que são carregados na RAM. O mesmo se aplica a todos os dados que precisam ser processados por uma aplicação. Essa distinção abrange dados de uma ampla gama de aplicativos, como os que lidam com matemática superior, imagens renderizadas e arquivos editados.

