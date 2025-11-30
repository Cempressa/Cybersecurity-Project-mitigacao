# Cybersecurity-Project-mitigacao
Desafio DIO: Implementação de ataques de força bruta com Medusa e análise de mitigação em serviços FTP, Web e SMB.
# 🛡️ Cybersecurity-Project-mitigacao

## 📜 1. Introdução
[cite_start]Breve descrição sobre o objetivo do projeto (simular ataques de força bruta com Medusa e propor mitigação)[cite: 5, 16].

## ⚙️ 2. Configuração do Ambiente
[cite_start]Detalhe as configurações das VMs (Kali Linux e Metasploitable 2) no VirtualBox e a rede interna (Host-Only) utilizada[cite: 6].

## 🔍 3. Cenários de Ataque e Análise (FTP, Web, SMB)
Para cada cenário que você executar (FTP, DVWA, SMB):
* **3.1. Serviço Alvo:** [Ex: Força Bruta em FTP]
* **3.2. [cite_start]Comandos Utilizados:** Mostrar os comandos exatos do Medusa e do Nmap (opcional)[cite: 8].
* **3.3. [cite_start]Wordlist:** Descreva a wordlist simples utilizada (ou link para o arquivo na pasta `wordlists/`)[cite: 8].
* **3.4. [cite_start]Validação de Acesso:** Evidencie o acesso bem-sucedido[cite: 8].

## ✅ 4. Recomendações e Mitigação
A parte mais importante! [cite_start]Proponha medidas de prevenção/mitigação para cada serviço atacado (FTP, Web, SMB)[cite: 8, 16].

## 🛠️ 5. Recursos e Ferramentas
[cite_start]Liste as ferramentas utilizadas (Kali Linux, Medusa, Metasploitable 2, DVWA)[cite: 5].

## ⚙️ 2. Configuração do Ambiente

A auditoria de segurança foi realizada em um ambiente controlado, utilizando máquinas virtuais configuradas no **VirtualBox**.

### 2.1. Topologia da Rede
[cite_start]Para garantir o isolamento dos testes, foi utilizada uma rede interna que simula um ambiente corporativo fechado, conforme recomendado no desafio[cite: 6].

* **Software de Virtualização:** VirtualBox (ou VMWare, etc.)
* **Tipo de Rede:** **Rede Interna (Host-Only)**, que permite a comunicação apenas entre o Kali Linux e o Metasploitable 2.

### 2.2. Máquinas Virtuais (VMs)

| VM | Sistema Operacional | Função no Teste | Configuração de Rede | Endereço IP (Exemplo) |
| :--- | :--- | :--- | :--- | :--- |
| **VM 1: Atacante** | **Kali Linux** | [cite_start]Contém a ferramenta Medusa para execução dos ataques de força bruta[cite: 5]. | Adaptador Host-Only | 192.168.56.101 (Exemplo) |
| **VM 2: Alvo** | **Metasploitable 2** | [cite_start]Contém o serviço FTP vulnerável a ataques[cite: 5]. | Adaptador Host-Only | 192.168.56.102 (Exemplo) |

> **⚠️ NOTA IMPORTANTE:** Os endereços IP acima são exemplos. É crucial que você **substitua** pelos endereços IP reais das suas máquinas virtuais, que você pode descobrir com o comando `ip a` ou `ifconfig` no Kali Linux e no Metasploitable 2.
