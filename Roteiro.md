# Roteiro: do power-on ao sistema operacional

### **Etapa 1: Power-on / POST**
- Fonte de energia estabiliza a tensão e envia sinal de reset para a placa-mãe
- CPU inicia execução a partir de um endereço fixo na memória (onde a BIOS/UEFI está mapeada)
- Firmware executa o POST: testa CPU, controlador de memória, RAM, barramentos (PCIe, SATA) e GPU
- Falha aqui = sistema trava antes de qualquer software rodar (beeps de erro, sem vídeo)

### **Etapa 2: BIOS/UEFI**
- Inicializa controladores essenciais: chipset, memória, portas de armazenamento
- Enumera dispositivos conectados nos barramentos (PCIe, USB, SATA/NVMe)
- Consulta a ordem de boot configurada
- Localiza um dispositivo com setor de boot válido (MBR) ou partição EFI válida (GPT)
- Transfere a execução para o bootloader e encerra sua responsabilidade
- Diferença UEFI x BIOS legado: UEFI roda em modo 32/64-bit desde o início (BIOS usa 16-bit real mode), suporta discos acima de 2TB e tem interface própria com suporte a rede

### **Etapa 3: Bootloader**
- Lê o kernel do SO no disco
- Carrega o kernel na RAM, junto com estruturas iniciais (ex: initramfs no Linux)
- Passa parâmetros de boot
- Cede a execução ao kernel

### **Etapa 4: Kernel assume o controle**
- Reconfigura o hardware que a BIOS deixou em modo básico
- Monta suas próprias tabelas de interrupção
- Assume gerenciamento de memória virtual (paginação, MMU)
- Assume escalonamento de processos na CPU
- A partir daqui, BIOS/UEFI não tem mais papel ativo

### **Etapa 5: Drivers e gerenciadores de recursos**
- Kernel carrega drivers específicos para cada dispositivo detectado (GPU, rede, disco, USB)
- Cada driver traduz chamadas genéricas do SO em comandos que aquele hardware entende
- Gerenciadores de memória, processos e arquivos entram em operação
- Mediam o acesso concorrente de múltiplos processos ao mesmo hardware

### **Etapa 6: Papel dos barramentos e E/S**
- CPU não acessa dispositivos diretamente; envia comandos pelo barramento correspondente (PCIe, USB, SATA/NVMe, memória)
- Controlador do dispositivo recebe o comando e executa
- Interrupções de hardware (IRQs) avisam a CPU quando um dispositivo precisa de atenção, sem espera ativa
- DMA (acesso direto à memória) permite que dispositivos movam dados sem ocupar o processador

### **Etapa 7: Ambiente do usuário**
- Shell ou desktop environment carrega
- Sistema operacional pronto para executar processos de usuário
