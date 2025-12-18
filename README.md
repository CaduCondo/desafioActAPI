# 🚀 Desafio ACT - Automação Full Stack (API)

Este repositório apresenta uma solução robusta para o desafio técnico de automação, integrando testes de serviços (API) utilizando o ecossistema **Robot Framework**.

---

## 🛠️ Configuração e Requisitos

| Requisito | Versão Mínima | Finalidade |
| :--- | :--- | :--- |
| **Python** | 3.10+ | Linguagem base do projeto |

### 📥 Instalação
1. Clone o repositório.
2. Na raiz do projeto, instale as dependências:
   ```bash
   pip install -r requirements.txt
---

## 📂 Estrutura de Pastas

O projeto utiliza uma estrutura modular para separar as tecnologias e contextos de teste:

```text
├── resources/           # Keywords e Variáveis (Lógica de Teste)
│   ├── web/             # Recursos do Blog Agibank (Selenium)
│   └── api/             # Recursos da Dog API (Requests)
├── tests/               # Casos de Teste (Cenários BDD)
│   ├── web/             # Automação de Interface (UI)
│   └── api/             # Automação de Integração (API)
├── results/             # Relatórios, Logs e Screenshots
├── requirements.txt     # Dependências do projeto (Python)
└── README.md            # Documentação principal
```

---
## 🌐 Projeto: Automação de API (Dog API)

**Objetivo:** Garantir a integridade dos dados e a disponibilidade dos serviços da Dog API.

**Tecnologia:** Robot Framework + RequestsLibrary.

**Qualidade:** Inclui validações de SLA (tempo de resposta) e tratamento de erros.

### 🔍 Endpoints Testados
```text
Método  Endpoint                Descrição
GET     /breeds/list/all        Valida a listagem completa de raças.
GET     /breed/{breed}/images   Verifica o retorno de imagens por raça específica.
GET     /breeds/image/random    Valida o formato e integridade da URL aleatória.
```

### Como rodar os testes:
```bash
robot -d results .
```

---
## 📊 Resultados e Evidências
Após a execução, os artefatos estarão disponíveis na pasta /results:

**report.html:** Visão executiva dos testes.

**log.html:** Detalhamento técnico e screenshots de cada passo.