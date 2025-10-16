# 🟩 Etapa 0 — Preparação Imediata
**Projeto:** Galeria de NFTs  
**Disciplina:** Segurança em Aplicações  
**Aluno:** Fabricio Giannini (Marlon)  
**Data:** Outubro de 2025

---

## 🎯 Objetivo da Etapa
Iniciar o desenvolvimento da plataforma **Galeria de NFTs**, definindo o escopo mínimo (MVP), preparando o repositório, criando protótipos e estruturando a documentação necessária para a **apresentação parcial** (16/17 de outubro de 2025).

---

## 🧩 1. Escopo Mínimo (MVP)

A aplicação permitirá a criação e visualização de NFTs em um ambiente de galeria digital.

### Funcionalidades básicas para a apresentação parcial:
- Página inicial exibindo NFTs (galeria estática ou mockada);
- Página de **criação de NFT** (upload de imagem, nome e descrição);
- Exibição de **detalhes do NFT** (imagem, descrição e dono);
- Protótipo visual de **botão “Comprar”** (sem integração ainda);
- Estrutura de **cadastro/login** simulado para usuários.

### Funcionalidades planejadas para etapas futuras:
- Mint real via **smart contract (Solidity / ERC-721)**;
- Autenticação via **carteira digital (MetaMask / WalletConnect)**;
- Integração com **IPFS** para armazenamento de imagens e metadados;
- API REST com **Spring Boot** e banco de dados **PostgreSQL**.

---

## 🗂️ 2. Estrutura do Projeto (Repositório)

O projeto será organizado da seguinte forma:

/Galeria_NTF/
│
├── backend/ # Spring Boot (API REST)
│ ├── src/
│ └── pom.xml
│
├── frontend/ # React (interface web)
│ ├── src/
│ └── package.json
│
├── smart-contracts/ # Código Solidity (ERC-721)
│ ├── contracts/
│ ├── scripts/
│ └── hardhat.config.js
│
├── docs/ # Documentos do projeto
│ ├── briefing.pdf
│ ├── arquitetura.md
│ └── relatorio-etapa0.md
│
└── README.md


### Ferramentas:
- **Versionamento:** Git + GitHub
- **Protótipos:** Figma
- **IDE:** VSCode / IntelliJ
- **Gerenciamento:** Trello

---

## 🧠 3. Protótipo (Wireframes)

Protótipo criado no Figma (modo escuro), com as seguintes telas:

1. **Página Inicial (Galeria):** grade de NFTs com nome e imagem.
2. **Criar NFT:** formulário com upload de imagem, nome e descrição.
3. **Detalhes do NFT:** exibe informações completas do token e botão “Comprar”.

🖼️ **Link do protótipo (exemplo):** [figma.com/proto/galeria-nft](https://figma.com/proto/galeria-nft)  
*(inserir link real após criação)*

---

## 👥 4. Planejamento e Cronograma

| Data | Atividade | Entregável |
|------|------------|------------|
| 14/out | Criar repositório + estrutura inicial | Repositório no GitHub |
| 15/out | Criar protótipo (Figma) e documento de escopo | `docs/escopo.md` |
| 16/out | Revisar conteúdo e preparar slides da apresentação | Apresentação parcial pronta |

---

## 🔒 5. Requisitos de Segurança Inicial

Arquivo: `docs/requisitos-de-seguranca-inicial.md`

```markdown
# Requisitos de Segurança – Etapa 0
1. Nenhum dado sensível (como chaves privadas) deve ser armazenado no front-end.
2. Todo tráfego da aplicação deverá usar HTTPS.
3. O backend (Spring Boot) utilizará autenticação JWT em etapas futuras.
4. Implementar medidas de prevenção contra XSS e CSRF.
5. Registrar logs e hashes de transações para auditoria.
