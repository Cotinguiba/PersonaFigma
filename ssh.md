# Selfsame Hub (SSH) — Documentação da Fase 01

**Projeto:** Selfsame Hub (SSH)  
**Domínio:** Açougue / Gestão de vendas e operação  
**Status:** Documentação Completa da Fase 01  

---

## 1. Briefing e Visão do Projeto

O **Selfsame Hub (SSH)** é um sistema de gestão integrado voltado para açougues e boutiques de carnes. O seu objetivo principal é centralizar e organizar as operações do negócio, conectando em um único ecossistema o controle de estoque, vendas de balcão, pedidos digitais (app/web), entregas e gestão financeira/gerencial.

### Objetivos Principais
* Reduzir processos manuais e erros na venda por peso.
* Garantir rastreabilidade e controle de estoque em tempo real.
* Oferecer uma experiência de compra moderna e ágil para os clientes finais.
* Unificar pedidos presenciais e digitais num único painel de controlo.

---

## 2. Benchmarking (Análise de Mercado)

| # | Problema Mapeado no Mercado | Solução Proposta pelo Selfsame Hub |
|---|---|---|
| **1** | Sistemas antigos e pouco intuitivos | Interface moderna, responsiva, organizada por categorias e intuitiva. |
| **2** | Falta de controle de estoque | Baixa automática e alertas de estoque mínimo/validade. |
| **3** | Erros no cálculo de venda por peso | Cálculo automático de valor final ao inserir peso e preço/kg. |
| **4** | Processos de pagamento demorados | Fechamento de compras otimizado e métodos de pagamento integrados. |
| **5** | Falta de relatórios gerenciais | Dashboard com vendas do dia, faturamento e produtos mais vendidos. |
| **6** | Dependência de canais informais (WhatsApp) | Aplicativo próprio para o cliente consultar o catálogo e pedir diretamente. |
| **7** | Acompanhamento do pedido pelo cliente | Notificações de status (*Recebido → Em Preparação → Saiu p/ Entrega → Entregue*). |
| **8** | Personalização dos cortes no pedido | Campo de seleção para tipo de corte, espessura e observações específicas. |

---

## 3. Personas

### Persona Dono / Gerente
![Persona Dono](https://github.com/Cotinguiba/PersonaFigma/blob/develop/Persona%20Dono.png?raw=true)

* **Perfil:** Proprietário ou gerente do açougue responsável pela operação e decisão estratégica.
* **Necessidades:** Visão clara do faturamento, controle rígido de estoque, gestão de funcionários e agilidade no atendimento.

---

### Persona Cliente
![Persona Cliente](https://github.com/Cotinguiba/PersonaFigma/blob/develop/Persona%20Cliente.png?raw=true)

* **Perfil:** Consumidor final que busca praticidade na compra de carnes e cortes especiais.
* **Necessidades:** Visualizar catálogo atualizado, preços transparentes por kg, opção de entrega/retirada e personalização do corte.

---

## 4. Requisitos do Sistema

### 4.1 Requisitos Funcionais (RF)

* **RF-001 — Autenticação de Usuários:** Login seguro para administradores, atendentes, estoquistas e clientes.
* **RF-002 — Cadastro de Usuários:** Gestão de perfis e níveis de permissão.
* **RF-003 — Cadastro de Produtos & Categorias:** Organização de carnes bovinas, suínas, aves, cortes nobres e acompanhamentos.
* **RF-004 — Controle de Estoque:** Entrada, saída, saldo e baixa automática após vendas.
* **RF-005 — Registro de Vendas & Cálculo Por Peso:** Registro de pedidos presenciais e digitais calculando valor por peso.
* **RF-006 — Dashboard Gerencial:** Indicadores de vendas diárias, produtos mais vendidos e alertas de estoque baixo.
* **RF-007 — Catálogo Digital & Pedido do Cliente:** Interface móvel/web para o cliente montar o carrinho e pagar.
* **RF-008 — Acompanhamento e Notificação de Pedidos:** Atualização do status da entrega para o cliente em tempo real.

### 4.2 Requisitos Não Funcionais (RNF)

* **RNF-001 — Desempenho:** Resposta das operações comuns em até 2 segundos.
* **RNF-002 — Segurança:** Criptografia de dados sensíveis e autenticação segura.
* **RNF-003 — Usabilidade:** Interface intuitiva voltada para agilidade operacional no balcão e facilidade no app do cliente.
* **RNF-004 — Responsividade:** Layout adaptável a ecrãs de smartphones, tablets e computadores.

---

## 5. User Stories (Casos de Uso)

* **US-001 — Realizar Venda (Atendente):** Como atendente, quero registrar os produtos e pesos escolhidos pelo cliente para finalizar a venda de forma rápida.
* **US-002 — Consultar Estoque (Estoquista):** Como estoquista, quero visualizar as quantidades disponíveis e alertas para saber o que repor.
* **US-003 — Cadastrar Produto (Admin):** Como administrador, quero cadastrar e atualizar preços/cortes no catálogo.
* **US-004 — Realizar Pedido (Cliente):** Como cliente, quero escolher o corte, a quantidade e a forma de entrega diretamente no aplicativo.
* **US-005 — Acompanhar Entrega (Cliente):** Como cliente, quero receber notificações sobre o andamento do meu pedido.

---

## 6. Style Guide (Guia de Estilo)

### 6.1 Brand / Logo
![Logo Selfsame Hub](logo_selfsame_hub.png)

O logótipo combina o monograma **"S"** com elementos tecnológicos (circuitos integrados) e a forma de uma placa/ecrã móvel, simbolizando a fusão entre a tradição da carne e a tecnologia do ecossistema **Selfsame Hub**.

---

### 6.2 Paleta de Cores
![Paleta de Cores](paleta_de_cores.png)

* **Gold:** `#A98C2D` | `rgb(169, 140, 45)`
* **White:** `#D9D9D9` | `rgb(217, 217, 217)`
* **Red (Principal):** `#9C0404` | `rgb(156, 4, 4)`
* **Wine:** `#780606` | `rgb(120, 6, 6)`
* **Black:** `#000000` | `rgb(0, 0, 0)`
* **Light Pink:** `#FFD3D3` | `rgb(255, 211, 211)`
* **Watergreen:** `#4CB6AC` | `rgb(76, 182, 172)`
* **Aqua Green:** `#3C837C` | `rgb(60, 131, 124)`

---

### 6.3 Tipografia e Iconografia
![Interface Base - Tipografia e Iconografia](interface_base.png)

* **Tipografia:** Sans-Serif Geométrica e Limpa (estilo Inter / Plus Jakarta Sans).
  * **Headings:** Negrito / Semi-bold para títulos de produtos e preços.
  * **Body / Labels:** Regular para descrições, especificações dos cortes e menus.
* **Iconografia:** Estilo *Outlined* (Linhas finas e minimalistas) incluindo ícones de Lupa, Carrinho, Perfil, Camião de Entrega, QR Code e Selos de Garantia.

---

## 7. Moodboard
![Moodboard](moodboard.png)

O Moodboard reúne referências visuais de e-commerce de gastronomia de alta qualidade, boutiques de carnes, tons terrosos/amadeirados e componentes visuais de login e navegação limpa.

---

## 8. Sitemap e User Flow (Fluxograma)
![Sitemap e User Flow](sitemap_userflow.png)

### Estrutura do Sistema (Sitemap)
1. **Página Inicial / Landing Page / Login**
2. **Área do Cliente (App/Web):**
   * Catálogo de Produtos (Filtros por categoria)
   * Detalhes do Corte (Escolha de peso/espessura)
   * Carrinho de Compras
   * Checkout & Opções de Pagamento (PIX/Cartão)
   * Acompanhamento de Pedido
3. **Painel de Gestão do Açougue:**
   * Gestão de Pedidos (Recebidos, Em Preparação, Prontos)
   * Controlo de Estoque & Produtos
   * Gestão de Clientes & Vendas
   * Relatórios & Dashboard
4. **Módulo de Caixa / PDV (Balcão)**

---

## 9. Wireframes & Protótipos de Alta Fidelidade

### Protótipos Mobile
![Wireframes e Protótipo Mobile](wireframe_mobile.png)

### Protótipos Web / Desktop
![Wireframes e Protótipo Web](wireframe_web.png)

A aplicação conta com layout responsivo desenhado para Web e Dispositivos Móveis, cobrindo todo o fluxo desde a autenticação, navegação por cortes nobres, seleção personalizada por peso, checkout com QR Code PIX até ao rastreamento em tempo real do pedido.