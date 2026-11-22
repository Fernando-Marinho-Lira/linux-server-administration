# Projeto 01 — Infraestrutura de Redes com Linux, MikroTik, Pi-hole, Squid e Samba

**Portfólio técnico | Administração de infraestrutura, redes e segurança**

## Visão geral
Projeto de infraestrutura de redes documentado em ambiente Linux, integrando serviços de **DNS e filtragem (Pi-hole)**, **proxy de navegação (Squid)**, **compartilhamento de arquivos (Samba)** e **roteamento e segurança de rede (MikroTik)**.

O objetivo foi centralizar serviços essenciais, aplicar regras de acesso, melhorar a visibilidade do tráfego e aproveitar hardware de baixo custo.

> **Natureza do projeto:** laboratório e documentação técnica. As capturas, comandos e configurações detalhadas estão no portfólio em PDF. Exemplos e recomendações no documento não devem ser confundidos com todas as funcionalidades efetivamente implantadas.

## Tecnologias abordadas

| Tecnologia | Aplicação no projeto |
|---|---|
| **antiX Linux** | Servidor para os serviços de rede |
| **MikroTik RouterOS** | Roteamento, segmentação, firewall e NAT |
| **Pi-hole** | Resolução e filtragem DNS, bloqueio de domínios |
| **Squid Proxy** | Controle de navegação, cache, filtros e registros de acesso |
| **Samba** | Compartilhamento de arquivos, usuários e permissões |
| **TCP/IP e DHCP** | Endereçamento, conectividade e distribuição de parâmetros de rede |
| **Logs e monitoramento** | Diagnóstico e acompanhamento de serviços e tráfego |

## Arquitetura da solução

- **Internet → MikroTik:** gateway, roteamento, políticas de firewall e NAT.
- **Rede administrativa (192.168.100.0/24):** computadores e uso do proxy Squid.
- **Rede de clientes Wi-Fi (172.16.1.0/24):** clientes com filtragem DNS pelo Pi-hole.
- **Servidor Linux (IP privado documentado: 192.168.100.174):** serviços Pi-hole, Squid e Samba.

Os diagramas do portfólio descrevem as rotas de DNS, navegação web e compartilhamento de arquivos. Os IPs mostrados são endereços privados do ambiente documentado.

## Principais componentes

### 1. Squid Proxy
- Controle e filtragem de acesso à web.
- Políticas de acesso e cache.
- Análise de registros em `/var/log/squid/access.log`.
- Diagnóstico de desempenho e comportamento de consultas DNS.

### 2. MikroTik, firewall e NAT
- Roteamento entre redes locais e acesso à internet.
- Regras de filtragem, controle de acesso e redirecionamento DNS.
- Análise de regras de firewall, NAT e conexões no RouterOS.
- Separação de tráfego por função e cuidado com loops de resolução DNS.

### 3. DNS com Pi-hole
- Filtragem de anúncios e domínios indesejados.
- Uso do Pi-hole para resolução DNS dos clientes definidos na arquitetura.
- Integração com DHCP e políticas de DNS no MikroTik.
- Verificação de consultas, bloqueios e logs.

### 4. Samba
- Compartilhamento de arquivos pela rede.
- Configuração de usuários, grupos e permissões.
- Validação do arquivo `smb.conf` com `testparm -s`.
- Testes de acesso a partir de clientes Windows e Linux.

### 5. Monitoramento e troubleshooting
- Acompanhamento dos painéis Pi-hole e Squid e dos registros de acesso.
- Análise de logs do Samba e de regras do MikroTik.
- Testes de conectividade, DNS, portas e serviços com `ping`, `traceroute`, `nslookup`, `curl`, `ss` e `systemctl`.
- Procedimentos de diagnóstico de falhas de navegação, resolução de nomes e compartilhamentos.
- Referências a ferramentas como Zabbix, Grafana e Netdata como possibilidades de evolução, sem afirmar sua implantação.

## Resultados e aprendizado
A documentação apresenta integração dos serviços, controles de acesso, compartilhamento de arquivos, filtragem DNS e procedimentos de diagnóstico. O projeto evidencia experiência com **Linux, redes TCP/IP, MikroTik, firewall, NAT, DNS, proxy, Samba e troubleshooting**.

## Documentação completa

📄 [Visualizar o portfólio de infraestrutura de redes (PDF)](./Portfolio_Infraestrutura_Redes_Fernando_Marinho_CORRIGIDO.pdf)

O PDF inclui arquitetura, topologia, configurações, exemplos de comandos, monitoramento, segurança e conclusão.

**Nota editorial:** a versão atual do PDF reúne duas páginas de monitoramento e deve passar por uma revisão final de conteúdo e numeração.

## Autor

**Fernando Marinho Lira**  
Infraestrutura de TI | Linux | Redes | MikroTik | Microsoft Azure | AZ-900

[Perfil no LinkedIn](https://www.linkedin.com/in/fernando-marinho-lira/)

---
*Projeto apresentado para fins de portfólio e demonstração de competências técnicas. Não publique senhas, credenciais, IPs públicos, dados pessoais de terceiros ou configurações sigilosas.*