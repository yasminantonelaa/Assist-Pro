# AssistPro — Assistente Pessoal para Negócios

> Plataforma web de apoio executivo que centraliza gestão de agenda, e-mails, viagens corporativas e relatórios de despesas em um único painel.

---

## Visão Geral

A **AssistPro** é um produto voltado para executivos e empresas que precisam delegar tarefas administrativas e operacionais a um serviço especializado. O front-end estático apresenta a proposta de valor, permite o cadastro de novos usuários e oferece um painel de gestão pós-login com acesso rápido aos principais módulos do serviço.

---

## Estrutura de Páginas

| Arquivo          | Rota / Finalidade                                                                 |
|------------------|-----------------------------------------------------------------------------------|
| `index.html`     | **Landing page** — apresentação da plataforma, serviços, planos e chatbot de vendas |
| `cadastro.html`  | **Cadastro** — formulário de criação de conta gratuita (trial de 14 dias)         |
| `login.html`     | **Login** — autenticação de usuários já cadastrados                               |
| `dashboard.html` | **Painel do executivo** — visão consolidada de agenda, e-mails, viagens e despesas |
| `perfil.html`    | **Meu Perfil** — configurações e dados da conta do usuário                        |

---

## Funcionalidades

### Landing Page (`index.html`)
- Seção hero com chamada para ação e criação de conta
- Apresentação dos quatro serviços principais: Agenda, E-mails, Viagens e Despesas
- Seção de planos (Starter, Professional, Enterprise)
- Depoimentos de clientes
- **Chatbot de atendimento** com base de conhecimento local que responde perguntas sobre serviços, preços, segurança e contratação

### Cadastro e Login
- Formulário de registro com validação de campos
- Tela de autenticação com redirecionamento para o painel

### Painel (`dashboard.html`)
- Sidebar de navegação fixa
- Cards de resumo: próximos compromissos, e-mails pendentes, viagens e saldo de despesas
- Layout responsivo com colapso da sidebar em telas menores

### Perfil (`perfil.html`)
- Edição de dados pessoais e preferências da conta
- Gerenciamento de plano e assinatura

---

## Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura de todas as páginas |
| CSS3 (customizado) | Estilos globais, componentes e responsividade |
| [Tailwind CSS](https://tailwindcss.com/) v3 (CDN) | Utilitários de layout e espaçamento |
| [Google Fonts](https://fonts.google.com/) | Tipografia — Inter (corpo) e Playfair Display (destaques) |
| JavaScript (vanilla) | Chatbot, interatividade do painel e validações |

---

## Paleta de Cores

| Token | Hex | Uso |
|---|---|---|
| Teal | `#2A9D8F` | Cor primária, botões de ação |
| Teal Dark | `#1F7268` | Hover de botões primários |
| Slate / Navy | `#3D5A6B` | Header, sidebar, fundos escuros |
| Background | `#F4F7F7` | Fundo do painel |
| Text principal | `#2D3D3A` | Cor base de texto |

---

## Como Executar Localmente

O projeto é composto exclusivamente por arquivos estáticos — não há dependência de servidor back-end ou processo de build.

```bash
# 1. Clone ou baixe o repositório
git clone https://github.com/seu-usuario/assistpro.git
cd assistpro

# 2. Abra diretamente no navegador
# Opção A — abertura direta
open index.html

# Opção B — servidor local simples (recomendado)
npx serve .
# ou
python -m http.server 8000
```

Acesse `http://localhost:8000` no navegador.

---

## Estrutura de Arquivos

```
assistpro/
├── index.html       # Landing page
├── cadastro.html    # Página de cadastro
├── login.html       # Página de login
├── dashboard.html   # Painel do executivo
├── perfil.html      # Perfil do usuário
└── README.md
```

---

## Acessibilidade

- Foco visível em todos os elementos interativos via `:focus-visible`
- Suporte a `prefers-reduced-motion` para usuários sensíveis a animações
- Atributos `aria-label` e `aria-expanded` nos componentes interativos do chatbot

---

## Contato (conteúdo fictício do projeto)

- **E-mail:** contato@assistpro.com.br
- **Telefone:** +55 (11) 3245-6789
- **Endereço:** Av. Paulista, 1000 – 12º andar, São Paulo – SP
- **Atendimento:** segunda a sexta, 08h às 18h
