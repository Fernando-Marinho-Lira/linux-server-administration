# 🐧 Administração de Servidores Linux e Infraestrutura de Redes

**Portfólio técnico de Fernando Marinho Lira | Linux • Redes • MikroTik • Serviços de Infraestrutura**

[![GitHub](https://img.shields.io/badge/GitHub-Perfil_profissional-181717?style=flat-square&logo=github)](https://github.com/Fernando-Marinho-Lira)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Contato_profissional-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/fernando-marinho-lira/)
![Documentação](https://img.shields.io/badge/Status-Documenta%C3%A7%C3%A3o_em_evolu%C3%A7%C3%A3o-blue?style=flat-square)

## 📌 Sobre este repositório

Este espaço reúne **documentação técnica de laboratórios e projetos de infraestrutura**, com foco em administração de sistemas Linux, redes, serviços corporativos, segurança e troubleshooting.

Os materiais apresentam arquiteturas, tecnologias abordadas, procedimentos e referências técnicas. **Configurações demonstrativas e possibilidades de evolução não devem ser interpretadas automaticamente como recursos já implantados ou testes executados.**

## 🗂️ Índice de laboratórios existentes

| Laboratório | Escopo documentado | Acessar |
|---|---|---|
| **01 — Infraestrutura de redes com Linux, MikroTik, Pi-hole, Squid e Samba** | antiX Linux, roteamento, firewall/NAT, DNS e filtragem, proxy, compartilhamento de arquivos e diagnóstico | [📂 Abrir laboratório 01](./projeto-01-linux-samba-pihole/) |

**Situação do catálogo:** 1 laboratório documentado neste repositório. Novos laboratórios poderão ser incluídos conforme forem realizados e documentados.

## 🔎 Laboratório 01 — Visão rápida

O [Laboratório 01](./projeto-01-linux-samba-pihole/README.md) descreve uma infraestrutura de rede integrada, incluindo:

- **Linux (antiX):** servidor dedicado a serviços de rede.
- **MikroTik RouterOS:** gateway, roteamento, firewall e NAT.
- **Pi-hole:** resolução e filtragem DNS.
- **Squid Proxy:** políticas de navegação e registros de acesso.
- **Samba:** compartilhamento de arquivos e permissões.
- **Troubleshooting:** consulta a logs e procedimentos de verificação de conectividade e serviços.

A documentação específica registra a arquitetura com rede administrativa `192.168.100.0/24` e rede de clientes Wi-Fi `172.16.1.0/24`. Consulte o README do laboratório para entender o escopo e as ressalvas do ambiente descrito.

### 📚 Documentos disponíveis

| Arquivo | Finalidade |
|---|---|
| [README do laboratório](./projeto-01-linux-samba-pihole/README.md) | Visão geral, arquitetura, tecnologias e documentação técnica |
| [Portfólio de infraestrutura de redes — PDF](./projeto-01-linux-samba-pihole/Portfolio_Infraestrutura_Redes_Fernando_Marinho_CORRIGIDO.pdf) | Documento principal com descrição do projeto, diagramas e referências técnicas |
| [Projeto de infraestrutura Linux — PDF](./projeto-01-linux-samba-pihole/Projeto_Infraestrutura_Linux_Portfolio.pdf) | Arquivo complementar já existente no repositório |

> **Revisão pendente:** o README do laboratório indica que o PDF principal ainda contém repetição de páginas de monitoramento e precisa de revisão editorial. Ele permanece disponível sem alterações nesta etapa.

## 🎯 Objetivos de documentação

- Organizar experiências e laboratórios técnicos com estrutura navegável.
- Demonstrar decisões de arquitetura e o papel de cada serviço.
- Registrar procedimentos de configuração, segurança e manutenção.
- Distinguir claramente **o que foi documentado**, **o que foi validado** e **o que é proposta de evolução**.
- Acrescentar evidências e resultados reais à medida que forem verificados.

## 🧱 Estrutura atual

```text
linux-server-administration/
├── README.md
└── projeto-01-linux-samba-pihole/
    ├── README.md
    ├── Portfolio_Infraestrutura_Redes_Fernando_Marinho_CORRIGIDO.pdf
    └── Projeto_Infraestrutura_Linux_Portfolio.pdf
```

## 🛣️ Estrutura recomendada para futuras publicações

Para **novos laboratórios**, manter o padrão `projeto-XX-nome-descritivo/`, preferencialmente com:

1. `README.md` contendo objetivo, cenário, arquitetura e escopo.
2. Configurações, scripts ou comandos **somente quando revisados e seguros para publicação**.
3. Evidências reais (capturas, saídas de comandos e testes), com dados sensíveis ocultos.
4. Resultados observados, limitações e lições aprendidas.
5. Links para documentos complementares.

**Nenhuma dessas pastas ou evidências adicionais foi criada nesta atualização.** Essa é apenas uma orientação de organização para trabalhos futuros.

## 👤 Autor

**Fernando Marinho Lira**  
Analista de Infraestrutura de TI | Linux | Redes | MikroTik | Microsoft Azure  
**Certificação:** Microsoft Azure Fundamentals (AZ-900)

[GitHub](https://github.com/Fernando-Marinho-Lira) · [LinkedIn](https://www.linkedin.com/in/fernando-marinho-lira/)

---

*Documentação para fins de estudo e portfólio profissional. Antes de publicar configurações reais, remova credenciais, dados de clientes, informações pessoais e detalhes confidenciais de rede.*
