# instala-o-linux
Processo de instalação do Linux na máquina virtual.

# Documentação: Instalação do Linux em Máquina Virtual

## Introdução

Este documento descreve o processo de instalação do Linux em uma máquina virtual (VM).

## Requisitos

- Máquina Virtual com VirtualBox, VMware ou outro software de virtualização.
- Imagem ISO do Linux (neste caso, Debian).

## Passos para Instalação

### 1. Preparação da Máquina Virtual

1. **Crie uma Nova Máquina Virtual:**
   - Abra seu software de virtualização (VirtualBox, VMware, etc.).
   - Clique em "Nova" ou "Create New Virtual Machine".
   - Selecione um nome para a VM, como "Linux-Debian".
   - Escolha o tipo e versão do sistema operacional (Debian 64-bit).

2. **Configure a Memória e o Armazenamento:**
   - Atribua a quantidade de memória RAM (recomendado: 2 GB ou mais).
   - Crie um disco rígido virtual. Selecione o tipo VDI (VirtualBox Disk Image) ou equivalente e aloque espaço (recomendado: 20 GB ou mais).

### 2. Instalação do Sistema Operacional

1. **Anexe a Imagem ISO:**
   - Vá para as configurações da VM e selecione a opção de armazenamento.
   - Anexe a imagem ISO do Debian ao drive óptico da VM.

2. **Inicie a Máquina Virtual:**
   - Inicie a VM e selecione a opção de inicializar a partir do CD/DVD.

3. **Inicie o Instalador do Debian:**
   - Selecione o idioma e o layout do teclado.
   - Escolha o método de instalação.

4. **Configure a Rede e o Nome do Host:**
   - Configure a rede para obter um IP automaticamente (DHCP) ou manualmente, conforme necessário.
   - Defina o nome do host da máquina virtual.

5. **Particione o Disco:**
   - Escolha o método de particionamento (recomendado: usar o disco inteiro).
   - Siga as instruções para configurar as partições (raiz, swap, etc.).

6. **Instale o Sistema Base e Configure o Gerenciador de Pacotes:**
   - Selecione os pacotes adicionais desejados (recomendado: ambiente gráfico, ferramentas de desenvolvimento).
   - Complete a instalação e reinicie a máquina virtual.

### 3. Pós-instalação

1. **Atualize o Sistema:**
   ```bash
   sudo apt-get update
   sudo apt-get upgrade
