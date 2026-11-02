# 🐾 miauFOOD — Assinatura Inteligente de Ração e Petiscos

> **O miauFOOD** é um serviço de assinatura recorrente para entrega programada de ração e petiscos para cães e gatos, operando inicialmente em Fortaleza (CE). O objetivo é garantir que o tutor nunca fique sem suprimentos em casa, unindo praticidade no webapp e relacionamento humanizado via WhatsApp.

---

## 1. A Dor Escolhida e por que ela Vale um Negócio

* **A Dor do Consumidor:** Tutores de pets têm rotinas corridas e frequentemente enfrentam o problema da **ruptura de estoque em casa** (a ração acaba de surpresa, exigindo compras de última hora em pet shops físicos por preços mais altos ou gerando estresse). Outro ponto é o peso e o trabalho logístico de carregar sacos pesados de ração mensalmente.
* **Por que vale um negócio:** O mercado de *pet food* (alimentação animal) é o motor do setor pet no Brasil, representando a maior fatia de faturamento com recompra obrigatória e previsível. O modelo de assinatura resolve a dor da conveniência para o cliente e garante receita recorrente previsível (LTV alto) para a operação.

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/300facd5-9513-4d34-9bbb-4b7a46bfc4b6" />

---

## 2. Tamanho de Mercado (TAM / SAM / SOM) e Business Model Canvas

O dimensionamento de mercado foi estruturado para guiar a expansão gradual da operação:
* **TAM (Total Addressable Market - Brasil):** ~50 milhões de domicílios/pets com forte presença no mercado nacional de pet food.
* **SAM (Serviceable Available Market - Ceará):** ~3 milhões de lares e pets no estado do Ceará, que se destaca nacionalmente pela alta penetração de lares com felinos.
* **SOM (Serviceable Obtainable Market - Fortaleza):** ~100 mil domicílios-alvo nas regiões de maior densidade e poder aquisitivo em Fortaleza (como Aldeota, Meireles, Cocó, etc.).

### Business Model Canvas resumido:
* **Segmento de Clientes (ICP):** "Pais de pet" urbanos (classes B/C) em Fortaleza que valorizam tempo, saúde animal e conveniência.
* **Proposta de Valor:** Ração na porta de casa na frequência exata do consumo, com desconto de assinatura e sem burocracia.
* **Canais:** Instagram (captação), WhatsApp (relacionamento/fechamento) e Webapp (gestão do plano).
* **Parceiros-Chave:** Distribuidores de ração, pet shops locais e parceiros logísticos de entrega rápida.

<img width="904" height="438" alt="image" src="https://github.com/user-attachments/assets/0dcbf09a-540d-4c0e-9f2c-0e19dacb9279" />

---

## 3. A Tese que o MVP Testa e o que Ficou Manual de Propósito

* **A Tese:** Queremos validar se o consumidor de Fortaleza aceita o conceito de **assinatura recorrente de ração** (em vez de compra avulsas) e se o fluxo digital simplificado gera intenção real de compra através da conveniência de receber em casa.
* **O que ficou manual de propósito (Estratégia de MVP Lean):** 
  * **Meios de Pagamento e Assinatura Digital:** Para evitar atritos de desenvolvimento e burocracia de gateways de recorrência no dia zero, o checkout simula as opções de Pix/Cartão. Quando o cliente preenche o formulário, o sistema dispara um alerta por e-mail, e a equipe comercial **entra em contato manualmente via WhatsApp** para validar o endereço, fechar o pagamento e ativar o cliente.
  * **Painel Administrativo Próprio:** Criamos um dashboard interno integrado na própria aplicação (acessado pelo canto superior direito) para centralizar a visualização dos leads/pedidos capturados e facilitar o disparo do atendimento via WhatsApp.

<img width="1132" height="655" alt="image" src="https://github.com/user-attachments/assets/71382f0a-66ee-49de-af65-1f358cb7a233" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/28f2c492-5519-4b7a-b8a7-4b7c0822981a" />

<img width="1135" height="512" alt="image" src="https://github.com/user-attachments/assets/492c002d-88b3-4cd9-b115-c9a8335b984a" />

<img width="637" height="378" alt="image" src="https://github.com/user-attachments/assets/b48d285a-ca65-470b-92a6-13f7279b551e" />

<img width="337" height="204" alt="image" src="https://github.com/user-attachments/assets/c9f80502-9af7-4de7-9874-9b591d3a14ae" />

---

## 4. O Mega Prompt e as Iterações de Refinamento

O projeto foi inteiramente estruturado e gerado utilizando inteligência artificial com o seguinte prompt base (já adaptado com a identidade visual do **cachorro caramelo e gatas tricolores** — tons de branco, marrom claro e marrom escuro):

```markdown
# Prompt de Desenvolvimento: miauFOOD - Webapp de Assinatura de Ração e Petiscos

## 1. Visão Geral do Projeto
- **Nome da Solução:** miauFOOD
- **Propósito:** Webapp de assinatura recorrente de ração e petiscos para cães e gatos em Fortaleza.
- **Identidade Visual e Cores:** Paleta inspirada no "cachorro caramelo" e "gatos tricolores". Use tons de branco, marrom claro (caramelo/beige quente) e marrom escuro (chocolate/café) para os textos e elementos de destaque. Estilo limpo, moderno, acolhedor e focado em conversão.

## 2. Arquitetura de Navegação e Telas do Cliente
- **Tela 1: Home:** Hero Section com headline de conversão, CTA principal ("Montar Plano do Meu Pet") e seções de Como Funciona, Benefícios e Prova Social.
- **Tela 2: Quiz / Configurador do Plano:** Etapas interativas para dados do pet (cão/gato, idade, peso), escolha de ração (Standard/Premium/Super Premium), frequência de entrega em dias e resumo com desconto de assinatura.
- **Tela 3: Checkout Simples:** Captura de nome, WhatsApp e endereço em Fortaleza, com seleção simulada de Pix/Cartão e envio de notificação via e-mail.
- **Tela 4: Área do Cliente ("Minha Assinatura"):** Status da próxima entrega programada, opções de pular entrega, alterar endereço e botão de suporte via WhatsApp.

## 3. Painel Administrativo (Admin Dashboard)
- Acesso discreto no **canto superior direito da tela** (ícone de engrenagem/admin) listando os pedidos capturados com dados do tutor, pet, plano e um botão de ação rápida para "Chamar no WhatsApp".

## 4. Requisitos Técnicos
- Stack moderna (React, Tailwind, Lucide Icons) com persistência em banco de dados e integração de e-mail na nuvem.
```

## 5. Endereço da Aplicação Publicada
Acesse e teste o MVP em funcionamento: https://miaufood.lovable.app/
