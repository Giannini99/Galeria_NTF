# 🟪 Documento de Escopo do Projeto
**Projeto:** Galeria de NFTs  
**Disciplina:** Segurança em Aplicações  
**Aluno:** Fabricio Giannini (Marlon)  
**Data:** Outubro de 2025

---

## 🎯 1. Visão Geral do Projeto
A **Galeria de NFTs** é uma plataforma web voltada para a **criação, compra e venda de NFTs (Tokens Não Fungíveis)**, permitindo que artistas, colecionadores e entusiastas do mundo digital possam expor e negociar suas obras de maneira segura, transparente e descentralizada.

O sistema buscará integrar tecnologias de **blockchain**, **armazenamento descentralizado (IPFS)** e **autenticação por carteira digital (MetaMask)**, garantindo a originalidade e propriedade de cada item digital.

---

## 🧭 2. Objetivos

### Objetivo Geral
Desenvolver uma aplicação web segura e funcional para gerenciamento e comercialização de NFTs, com integração blockchain e mecanismos de proteção de dados.

### Objetivos Específicos
- Permitir o **mint (criação)** de NFTs únicos seguindo o padrão ERC-721.
- Exibir NFTs em uma **galeria interativa** com detalhes visuais e metadados.
- Implementar **compra e venda** com integração de carteiras digitais.
- Armazenar **imagens e metadados** em IPFS para garantir imutabilidade.
- Garantir **segurança das transações** e proteção de dados dos usuários.
- Criar **logs e auditorias** para rastreabilidade de ações.

---

## 💻 3. Tecnologias Envolvidas

| Camada | Tecnologia | Finalidade |
|--------|-------------|-------------|
| **Frontend** | React.js + Tailwind CSS | Interface responsiva e interativa |
| **Backend** | Spring Boot (Java) | API REST para gerenciamento de usuários e NFTs |
| **Banco de Dados** | PostgreSQL | Armazenamento off-chain de dados complementares |
| **Blockchain** | Solidity (Ethereum Testnet / Hardhat) | Smart Contracts ERC-721 |
| **Armazenamento** | IPFS | Armazenamento descentralizado de imagens e metadados |
| **Autenticação** | MetaMask / WalletConnect | Assinatura de transações e login |
| **Versionamento** | Git + GitHub | Controle de código e documentação |
| **Documentação** | Markdown + Swagger | Organização técnica e de API |

---

## 🧩 4. Escopo Funcional

### Funcionalidades Principais
1. **Cadastro e autenticação de usuário** (simulada inicialmente, via login simples).
2. **Criação de NFT (mint)**: upload de imagem, nome, descrição e metadados.
3. **Galeria de NFTs:** listagem dos tokens disponíveis.
4. **Visualização de NFT:** detalhes, dono, valor e botão “Comprar”.
5. **Compra e transferência de NFTs** entre usuários (em etapas futuras).
6. **Histórico de transações** (vendas, criações, compras).
7. **Logs e auditorias** das ações do sistema.

### Funcionalidades Futuras / Fora do Escopo Atual
- Integração com múltiplas blockchains (Polygon, Solana, etc.).
- Sistema de leilão ou ofertas automáticas.
- Integração com gateway de pagamento tradicional (Pix/cartão).
- Aplicativo mobile nativo.

---

## 🔒 5. Requisitos de Segurança

| Tipo | Descrição |
|------|------------|
| **Autenticação Segura** | Uso de JWT e assinatura de transações via MetaMask. |
| **Proteção de Dados** | Nenhum dado sensível será armazenado em texto puro. |
| **Integridade** | IPFS e hashes garantirão a originalidade dos NFTs. |
| **Confidencialidade** | Todo tráfego ocorrerá sob HTTPS. |
| **Auditoria** | Logs e registros imutáveis das ações críticas. |
| **Prevenção de Ataques** | Mitigação de XSS, CSRF, e SQL Injection. |

---

## 🗓️ 6. Cronograma Resumido

| Etapa | Período | Entregáveis |
|--------|----------|--------------|
| **Etapa 0** | até 16/10 | Estrutura inicial, protótipo, documentos e slides |
| **Etapa 1** | 17/10 – 31/10 | Arquitetura e contrato inteligente básico |
| **Etapa 2** | 01/11 – 15/11 | Backend (API REST) e integração com IPFS |
| **Etapa 3** | 16/11 – 06/12 | Frontend completo e integração blockchain |
| **Etapa 4** | 07/12 – 11/12 | Testes de segurança, deploy e apresentação final |

---

## 📦 7. Entregáveis Principais
- **Protótipo (Figma)** com telas de galeria, criação e detalhes.
- **Repositório GitHub** com estrutura completa do projeto.
- **Smart Contract (Solidity)** testado localmente.
- **API REST (Spring Boot)** documentada com Swagger.
- **Frontend (React)** integrado ao backend e contrato.
- **Relatório de Segurança e Testes**.
- **Apresentação Final (slides e demo funcional)**.

---

## 🚧 8. Riscos Identificados

| Risco | Impacto | Mitigação |
|--------|----------|------------|
| Erros em contratos inteligentes | Alto | Testes automatizados e auditoria de código |
| Falhas de autenticação | Alto | JWT + assinatura via carteira |
| Exposição de chaves privadas | Crítico | Armazenar somente no cliente (nunca no servidor) |
| Falhas de integração IPFS | Médio | Cache local e fallback de armazenamento |
| Atrasos no cronograma | Médio | Priorização do MVP para entrega acadêmica |

---

## 🧠 9. Benefícios Esperados
- Demonstração prática do uso de blockchain em aplicações seguras;
- Desenvolvimento de uma solução descentralizada de exposição e comércio digital;
- Aplicação de boas práticas de segurança, integridade e autenticação moderna;
- Contribuição acadêmica com um caso real de uso de NFTs em ambiente educativo.

---

## 📄 10. Conclusão
O projeto **Galeria de NFTs** servirá como um estudo prático e técnico sobre segurança em sistemas descentralizados, abordando desde o desenvolvimento de **smart contracts** até a **implementação de APIs seguras e autenticação por carteira**.  
Esta etapa de escopo estabelece a base conceitual e técnica que guiará todo o desenvolvimento até a entrega final em dezembro de 2025.

---
