# 🔒 ZkVerify Node - Zero-Knowledge Proof Verifier Node

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Status](https://img.shields.io/badge/status-active-blue.svg)

> Um node local confiável para validar provas zero-knowledge (ZK) com foco em segurança, transparência e escalabilidade. Este repositório serve como portfólio para minha carreira como desenvolvedor Web3, evidenciando habilidades práticas em infraestrutura, automação e segurança blockchain.

---

## ✨ Visão Geral

O `ZkVerify` é um node que roda localmente e permite verificar provas criptográficas ZK com facilidade. Ele é ideal para:

- Desenvolvedores que trabalham com aplicações **zk-SNARKs** e **zk-Rollups**;
- Testes e simulações de verificação ZK off-chain;
- Participação em redes blockchain com provas ZK.

---

## 🚀 Recursos

- ✅ Suporte a `zk-SNARK` e `zk-STARK`;
- 🔐 Verificação segura de provas com `zkVerify SDK`;
- ⚙️ Scripts de inicialização e automação com **bash** e **Docker**;
- 📈 Logging e monitoramento com saída formatada por `jq`;
- 🧱 Pronto para testes locais e integração em sistemas maiores.

---

## 📦 Tecnologias Utilizadas

| Categoria          | Ferramenta                      |
|--------------------|---------------------------------|
| Linguagens         | Bash, JSON, YAML                |
| Infraestrutura     | Docker, Docker Compose v2       |
| Dependências CLI   | `jq`, `curl`, `docker`, `bash`  |
| Scripts            | Linux Shell Scripts             |
| OS Recomendado     | Linux / WSL / Git Bash no Windows |

---

## 🛠️ Pré-Requisitos

Certifique-se de ter os seguintes itens instalados:

- [Docker](https://www.docker.com/)
- [Docker Compose v2](https://docs.docker.com/compose/)
- [`jq`](https://jqlang.github.io/jq/download/)
- Git Bash (ou WSL no Windows)

## 📥 Instalando o `jq` no Windows

> Use o `winget` ou instale manualmente:

```bash
winget install --id jqlang.jq
```

Se o terminal bash não reconhecer o jq, baixe manualmente de:
🔗 https://github.com/stedolan/jq/releases

E adicione ao seu PATH.

## ⚙️ Como Subir o Node

```bash
git clone https://github.com/seu-usuario/ZkVerify.git
cd ZkVerify
./scripts/init.sh
```

📌 O script verifica dependências e inicializa os contêineres.

## 📁 Estrutura do Projeto

```bash
ZkVerify/
├── docker-compose.yml       # Orquestração dos serviços
├── .env                     # Variáveis de ambiente
├── scripts/
│   ├── init.sh              # Script principal de inicialização
│   └── utils.sh             # Funções auxiliares
└── README.md                # Documentação
```

## 🧪 Testes

```bash
./scripts/test_proof.sh
```

Resultado esperado:

```bash
✅ Prova válida
```

## 📊 Métricas e Logs

Os logs são formatados com jq para facilitar a leitura. Exemplo:

```bash
docker logs zkverify_node | jq
```

## 🧠 Conceitos Envolvidos
ZKP (Zero-Knowledge Proof): provas que permitem validar informações sem revelá-las.

zk-SNARKs/STARKs: tipos específicos de provas usadas em blockchains modernas.

Docker: permite isolar ambientes de execução para maior reprodutibilidade.

jq: ferramenta poderosa para parseamento e manipulação de JSON.

##🤝 Contribuições

Contribuições são bem-vindas! Siga os passos:

1. Faça um fork

2. Crie sua branch com a feature (git checkout -b feature/minha-feature)

3. Commit suas alterações (git commit -m 'feat: adiciona minha feature')

4. Push na sua branch (git push origin feature/minha-feature)

5. Crie um Pull Request

## 🧾 Licença
Distribuído sob a licença [MIT](LICENSE). Veja o arquivo para mais detalhes.

## ⭐️ Se achou útil...
Considere dar uma estrela ⭐️ no repositório para ajudar mais desenvolvedores Web3 a encontrarem este projeto!

“A prova de conhecimento zero não revela nada — mas comprova tudo.”
— Criptografia moderna

