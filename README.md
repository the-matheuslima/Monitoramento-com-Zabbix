# Monitoramento-com-Zabbix
## 📌 Visão Geral

Este projeto consiste na implementação de um laboratório de monitoramento de infraestrutura utilizando o Zabbix, com o objetivo de simular um ambiente real de TI.
O Zabbix Server foi configurado em um Ubuntu Server, responsável por monitorar múltiplos hosts Linux e Windows em um ambiente virtualizado com VirtualBox.

O laboratório foi desenvolvido com foco em monitoramento proativo, análise de desempenho, disponibilidade de serviços e boas práticas de infraestrutura.

## 🎯 Objetivos do Projeto

- Implementar um servidor de monitoramento centralizado

- Monitorar hosts Linux e Windows via Zabbix Agent

- Configurar triggers, itens e dashboards

- Simular um ambiente corporativo virtualizado

- Consolidar conhecimentos em infraestrutura, redes e Linux

## 🧱 Arquitetura do Ambiente

### Topologia

- Zabbix Server

- Ubuntu Server

- Hosts Monitorados

  Ubuntu Server (Zabbix Agent)

  Windows Server (Zabbix Agent)

- Hypervisor

  Oracle VirtualBox

## Diagrama (opcional)

Inserir imagem do diagrama da rede aqui

## ⚙️ Tecnologias Utilizadas

- Zabbix Server

- Zabbix Agent

- Ubuntu Server

- Windows Server

- VirtualBox

- SSH

- MySQL / MariaDB (caso aplicável)

## 🔧 Configurações do Ambiente
- Sistema Operacional

  Ubuntu Server (ubuntu-24.04.3)

- Rede

  Tipo de rede: Host-only / NAT + Host-only
  Comunicação via SSH e TCP (porta 10050/10051)

  ## Preparação do Ambiente
- Criação das máquinas virtuais no VirtualBox

    <img width="1920" height="1080" alt="virtualbox_vms" src="https://github.com/user-attachments/assets/9dba5327-2358-4769-8e2a-85091288dbe1" />
  
- Configuração de rede e endereçamento IP
- Atualização dos sistemas operacionais
- Configuração de hostname em todas as VMs

## Instalação do Zabbix Server
- Adição do repositório oficial do Zabbix

    <img width="1908" height="917" alt="image" src="https://github.com/user-attachments/assets/686143ba-f94e-4be6-a7e2-2190d9604566" />

  
- Instalação do Zabbix Server e frontend
- Configuração do banco de dados
- Ajustes no arquivo zabbix_server.conf
- Inicialização e validação dos serviços
  
    <img width="1277" height="798" alt="image" src="https://github.com/user-attachments/assets/0b323142-68e9-428f-8505-a21f105785b3" />

- Frontend inicializado

  <img width="1917" height="899" alt="zabbix_config_login" src="https://github.com/user-attachments/assets/45202899-361f-4fb6-9a09-9702e1c5d49a" />

  <img width="1917" height="848" alt="dashboard_inicial" src="https://github.com/user-attachments/assets/05fdedb3-6b2c-40e7-a5b7-d99bc3f6071e" />

  
## Instalação do Zabbix Agent no Linux
- Instalação do pacote zabbix-agent
  
 <img width="1913" height="961" alt="zabbix_agent_page" src="https://github.com/user-attachments/assets/f2523925-e53c-4ff9-84cb-2d1cdfea294a" />

- Configuração do arquivo zabbix_agentd.conf

  <img width="1281" height="812" alt="ubuntu_agent-config" src="https://github.com/user-attachments/assets/33f4bfa7-ee49-47e0-8d12-89c2d3a65f23" />


- Definição do Server e ServerActive
- Inicialização do serviço

    <img width="1280" height="799" alt="ubuntu_agent_status" src="https://github.com/user-attachments/assets/1f3054d2-d86b-4b84-ac76-e079b2fcbe31" />

  
- Teste de comunicação com o Zabbix Server

## Instalação do Zabbix Agent no Windows
- Download e instalação do Zabbix Agent
- Configuração do arquivo de configuração
- Criação e inicialização do serviço
- Liberação das portas no firewall
- Validação do host no frontend do Zabbix

## Monitoramentos Implementados

<img width="1916" height="852" alt="latest_data_ubuntu_host" src="https://github.com/user-attachments/assets/1d2d3de5-afd8-43ab-bb30-f01107773835" />

- Uso de CPU
- Uso de memória RAM
- Espaço em disco
- Disponibilidade do host
- Status do Zabbix Agent

## Aprendizados
- Instalação e configuração completa do Zabbix
- Monitoramento de ambientes heterogêneos
- Importância do monitoramento proativo
- Troubleshooting de rede e agentes
- Organização de documentação técnica

## 📌 Próximos passos do projeto:

- Criação de dashboards personalizados (estilo NOC)
- Configuração de triggers e alertas
- Evolução da documentação para portfólio
- Monitoramento via SNMP
- Integração com e-mail ou Telegram

## Autor
- Nome: Matheus Lima
- GitHub: https://github.com/the-matheuslima
- LinkedIn: https://www.linkedin.com/in/the-matheuslima/

## Licença
- Projeto de caráter educacional
- Uso livre para fins de estudo e aprendizado
