# 🚀 QA Testing - Natura Gamification Platform (Web)

![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
![Abordagens](https://img.shields.io/badge/Abordagens-Web%20%7C%20Mobile%20%7C%20API-blue)
![Ferramentas](https://img.shields.io/badge/Ferramentas-Postman%20%7C%20Jira-lightgrey)

Este repositório documenta o esforço de testes do projeto Ficha de Produtos Natura, incluindo validação funcional na Web e em dispositivos móveis, além de verificação de APIs relacionadas a favoritos e integração com o LMS. O objetivo é assegurar a qualidade, a confiabilidade e a coerência dos dados apresentados ao usuário final.

---

# 🎯 Objetivo do Projeto

Garantir que a Ficha de Produtos Natura exiba corretamente produtos, conquistas, selos, recompensas e demais elementos de gamificação, refletindo de forma consistente as informações provenientes do LMS.

## Foco Principal

- Cobertura funcional dos fluxos críticos
- Garantia de integridade dos dados entre LMS e frontend
- Validação multiplataforma (Web, iOS e Android)
- Verificação de estabilidade e tempos de resposta das APIs

---

# 🧠 Escopo e Abordagem

## Web

- Navegadores: Microsoft Edge e Google Chrome
- Verificações: exibição de produtos (nome, descrição, imagem), conquistas, selos, recompensas e contadores de gamificação
- Integração: conferência de regras de negócio associadas ao LMS

## Mobile (iOS e Android)

- Validação de responsividade, navegação, acessibilidade básica e comportamento dos mesmos elementos de gamificação
- Checagem de consistência com a versão Web

## API (Postman)

- Foco em favoritos de cursos e trilhas
- Validação de status codes, headers, tempos de resposta e conteúdo
- Endpoints exercitados (ambiente de staging):
  - CourseUserFavorite/MarkAsFavorite e UnmarkAsFavorite
  - TrackUserFavorite/MarkAsFavorite e UnmarkAsFavorite

---

# 🔄 Fluxos Validados

1. Consulta e exibição de produtos
2. Exibição de conquistas, selos e recompensas
3. Marcação e desmarcação de favoritos (cursos e trilhas) via API
4. Sincronização entre ações no LMS e visualização na Ficha de Produtos

---

# 📁 Estrutura do Repositório

```bash
.
├── Api de Favoritos.postman_collection.json
├── Cenarios de Teste - Funcionalidade 1.docx
├── Cenarios de Teste - Funcionalidade 2.docx
├── Cenarios de Teste - Funcionalidade 3.docx
├── Cenarios de Testes API - Funcionalidade 1.docx
├── Plano de Projeto.pdf
├── Thumb.png
└── README.md
```

# ▶️ Como Executar os Testes de API

## Postman (Interface)

1. Abra o Postman
2. Importe a coleção: [Api de Favoritos.postman_collection.json]
3. Ajuste o corpo das requisições (CourseID, TrackID, UserID) conforme necessário
4. Execute as requisições e verifique os testes embutidos (status, headers, tempo e conteúdo)

## Newman (Opcional)

Se tiver o Newman instalado localmente:

```bash
newman run "Api de Favoritos.postman_collection.json"
```

Observação: ajuste URLs, IDs e autenticação conforme o ambiente de teste.

---

# ⚙️ Ambiente e Ferramentas

- Ambiente principal de API: https://isatcorp-vlec-stg.neolude.com.br
- Navegadores: Edge, Chrome
- Plataformas Mobile: iOS, Android
- Ferramentas: Postman (coleção), Jira (gestão de tarefas/defeitos)

---

# 🧪 Boas Práticas Adotadas

- Separação entre documentação funcional e scripts de API
- Casos de teste versionados e organizados por funcionalidade
- Testes de API com validações de status, headers, tempo de resposta e conteúdo
- Evidências e defeitos registrados em ferramenta de gestão (Jira)

---

# 📊 Gestão de Riscos

## Principais Riscos Mitigados

- Inconsistência entre LMS e Ficha de Produtos
- Regressões em exibição de gamificação
- Falhas de favoritos (cursos e trilhas)
- Variações de comportamento entre Web e Mobile

## Estratégias de Mitigação

- Execução de testes focados nos fluxos críticos
- Checagem cruzada entre plataformas
- Validações automatizadas básicas na coleção Postman
- Registro e acompanhamento sistemático de defeitos

---

# 📈 Resultados

- Validação bem-sucedida de exibição de produtos e elementos de gamificação
- Cobertura de favoritos via API com testes e asserções embutidas
- Evidências consolidadas nos documentos de cenários e no plano de projeto

---

# 🤝 Conclusão

Este repositório consolida os artefatos do processo de garantia de qualidade da Ficha de Produtos Natura, cobrindo Web, Mobile e API. O material serve de base para manutenção, regressão e futuras evoluções do produto.

