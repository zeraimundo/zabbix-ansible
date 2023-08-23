# Instalação do Zabbix com Ansible e Vagrant

Este repositório contém scripts e instruções para provisionar uma máquina virtual usando o Vagrant e configurar o Zabbix Server com o Ansible. Isso facilita a criação de um ambiente de monitoramento com o Zabbix de forma rápida e automatizada.

## Pré-requisitos

Antes de começar, certifique-se de ter o seguinte instalado no seu sistema:

Git

Virtualbox

Vagrant

## Uso

1. Clone este repositório:

   ```bash
   git clone https://github.com/zeraimundo/zabbix-ansible.git
   ```
2. Navegue até o diretório do projeto:

   ```bash
   cd zabbix-ansible
   ```
   
3. Inicialize a máquina virtual usando o Vagrant:
   ```bash
   vagrant up
   ```

4. Agora, você deve ter um ambiente de monitoramento do Zabbix em execução. Acesse o Zabbix Web UI em um navegador da web:

        URL: http://ip_da_máquina_provisionada:8080/zabbix
        
        Login: Admin
        
        Senha: zabbix

