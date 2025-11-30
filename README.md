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

## ⚠️ Aviso e Boas Práticas em Segurança

Este projeto foi desenvolvido estritamente para **fins educacionais e de auditoria de segurança**, conforme proposto no Desafio DIO. A aplicação dos conhecimentos aqui documentados deve seguir rigorosamente a **ética profissional**.

**Regras Essenciais:**

* **1. Conhecimento e Responsabilidade:** **Nunca** execute comandos sem o devido conhecimento de seus efeitos e implicações legais. A compreensão é a primeira linha de defesa.
* **2. Ambiente Controlado:** **Somente** realize testes em ambientes controlados e de sua propriedade (como as VMs Metasploitable 2 ou DVWA). Atacar sistemas sem permissão é ilegal.
* **3. Profissionalismo:** Utilize ferramentas adequadas para o trabalho, sem improvisação. O uso correto e ético das ferramentas é um sinal de profissionalismo.
* **4. Organização do Laboratório:** Mantenha seu laboratório virtual e seus arquivos de projeto organizados. A clareza no ambiente de testes leva à clareza na análise de resultados.
* **5. Conhecimento é Ferramenta:** Lembre-se que o **conhecimento** também é uma ferramenta poderosa. Mantenha sua mente focada e "limpa", dedicando-se ao estudo contínuo e à aplicação ética dos conceitos de segurança.

* ## Desenvolvido por: Cempressa
