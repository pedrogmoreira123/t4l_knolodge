# SAG — Visão Geral do Sistema

O SAG é um sistema de PDV (Ponto de Venda) para Windows, desenvolvido para estabelecimentos de food service como padarias, restaurantes, mercados, lanchonetes e fábricas. Funciona como um ERP organizado em abas na barra de navegação superior.

---

## Barra de Navegação Superior (Abas Principais)

O sistema é dividido nas seguintes abas, acessíveis pela barra superior:

| Aba | Função Principal |
|---|---|
| **Dashboard** | Resultados do faturamento diário, semanal e mensal do estabelecimento |
| **IA** | Módulo de inteligência artificial integrado ao SAG |
| **Principal** | Tela principal com atalhos para Caixa, Terminal de Comandas, Caderneta, Comandas, Novo Pedido e Tela de Pedidos |
| **Cadastros** | Produtos, Clientes, Fornecedores, Funcionários, Grupos, Promoções, etc. |
| **Produções** | Receitas, Nova Produção, Consultar Produção, Embalagens, Relatórios |
| **Estoque** | Entrada de Nota, Relatórios, Locais de Estoque, Estoque Atual, Ajustes, Inventário, Pedido de Compra, etc. |
| **Financeiro** | Contas a Pagar/Receber, Contas Bancárias, Categorias, Conciliação, Extratos, Relatórios |
| **Delivery** | Novo Pedido, Pedidos - Listagem, Pedidos - Kanban, Relatórios, Origens, Integrações |
| **Romaneio** | Módulo voltado para fábricas e distribuição — Novo Pedido, Romaneio - Lista, Romaneio - Kanban, Relatórios, Origens |
| **NFe** | Emitir, Gerenciar, Configuração, Inutilizar, NFe Recebidas, Vendas, Pedidos, Perfil de Impostos, Exportar |
| **Relatórios** | Personalizados, Fechamento de Caixa, Faturamento, Consultas, Itens Cancelados, Notas, Vendas, Listagem, Caderneta, Entradas e Saídas, Comandas Abertas, Venda por Usuário, Comissões, Lucros e MarkUp, Compras, Outros |
| **Outros** | Central de Usuários, Ferramentas, Grupo de Permissões, Arqs. da Balança, Etiquetas, Impressoras Remotas, Dados Cadastrais, Certificado Digital, Licença, Config Espécies, Cartão de Acesso, Lei do Imposto, Ferramentas CFe, Exportar XML, TEF, Conf. Dispositivos Móveis, Configurações de Estabelecimentos, SPED |

---

## Canto Superior Direito — Configurações e Acesso

No canto superior direito da tela, além do nome do usuário logado, existem os seguintes acessos:

| Item | Função |
|---|---|
| **Notificações** (ícone de sino) | Central de Notificações. Exibe um badge vermelho com a quantidade de notificações não lidas |
| **Suporte** | Acesso ao suporte T4L |
| **Config. Terminal** | Configurações específicas por terminal/caixa (Impressoras, NFC-e, TEF, Terminal PC, Caixa, Balança, Biometria, Personalizar, Produtos, Delivery, Auto Atendimento, Outros). Acesso restrito a técnicos. |
| **Config. Global** | Configurações que valem para todo o sistema (Email, Caixa, Delivery, Taxa de Entrega, Romaneio, Comandas, Estoque, Financeiro, Etiquetadora, Outros, Módulos, Autoatendimento, NFC-e, Multiloja). Acesso restrito a técnicos. |
| **Nome do usuário** | Menu com **Alterar Senha** e **Sair** |

> **Config. Terminal** define comportamentos por máquina (ex: qual impressora usar, se pede CPF, se utiliza comandas, se lança valores no fechamento). **Config. Global** define comportamentos para o sistema todo (ex: taxa de serviço, taxa de entrega, DDD padrão, integrações logísticas).

---

## Dashboard

**Caminho:** Aba **Dashboard** na barra superior

Tela de acompanhamento dos resultados do negócio, com saudação personalizada e logo do estabelecimento. É dividida nas seguintes seções:

**Seção "Hoje" — cartões configuráveis**

Faixa de cartões que o próprio cliente escolhe. Métricas disponíveis:

| Métrica | O que mostra |
|---|---|
| Faturamento Hoje | Receita total do dia |
| Vendas Hoje | Quantidade de vendas fechadas hoje |
| Ticket Médio Hoje | Valor médio por venda realizada hoje |
| Pedidos Hoje | Quantidade de pedidos do dia |
| Pedidos Cancelados Hoje | Pedidos cancelados no dia |
| Itens Cancelados Hoje | Itens removidos de pedidos/comandas hoje |
| Média de Itens por Venda (hoje) | Média de itens por venda |
| Hora de Pico Hoje | Horário de maior movimento |
| Faturamento Semana Atual / Mês Atual | Receita da semana / do mês corrente |
| Faturamento (7 dias) / (30 dias) | Receita dos últimos 7 ou 30 dias |
| Vendas (30 dias) | Quantidade de vendas dos últimos 30 dias |
| Ticket Médio (30 dias) | Ticket médio do período |
| Itens Cancelados (30 dias) | Itens cancelados no período |
| Item Mais Vendido (30 dias) | Produto de maior volume |
| Produto Mais Rentável (30 dias) | Produto de maior margem |
| Hoje vs Ontem | Comparativo direto entre os dois dias |
| Variação 30 dias vs 30 anteriores | Comparativo entre os dois períodos |

**Seção "Comparativo — últimos 30 dias vs período anterior"**

Cartões de KPI com indicador de tendência (alta/baixa em relação aos 30 dias anteriores): Faturamento, Vendas, Ticket Médio, Comandas, Pedidos, Sangrias, Cancelados e Horário de Pico.

**Gráficos e painéis:**
- Faturamento Comparativo — evolução do faturamento no período contra o período anterior
- Top Produtos — produtos mais vendidos
- Pedidos por Origem — distribuição dos pedidos por canal
- Mapa de Calor — concentração de vendas por dia/horário

**Botões da tela:**

| Botão | O que faz |
|---|---|
| **Configurar** | Abre "Personalizar cartões" — escolhe quais cartões da seção "Hoje" aparecem, o título de cada um e permite criar métrica personalizada |
| **Atualizar** | Recarrega os dados do dashboard |

---

## Módulo IA

**Caminho:** Aba **IA** na barra superior (identificada com badge "NEW")

Módulo de inteligência artificial integrado ao SAG. A IA consegue:
- Orientar o cliente em dúvidas sobre relatórios
- Gerar informações e análises puxando dados do banco de dados do estabelecimento

**Plano de uso:**
- Cliente **sem o módulo IA contratado**: 20 perguntas gratuitas
- Cliente **com o módulo IA contratado**: 100 perguntas
- A tela mostra o contador "Perguntas gratuitas restantes: X de Y"
- Ao atingir o limite, o SAG exibe o painel com a opção de contratação
- O acesso ao módulo depende da permissão **Outros → Módulo IA** no grupo do usuário

---

## Tela Principal

**Caminho:** Aba **Principal** na barra superior

Tela com atalhos em cards coloridos para os módulos mais usados:

| Card | Função |
|---|---|
| **Caixa** | Abre a Frente de Caixa (PDV) para efetuar vendas |
| **Terminal de Comandas** | Terminal de lançamento de produtos em comandas (fluxo: Operador > Comanda > Produtos) |
| **Caderneta** | Gerenciamento de caderneta — recebimento, extrato, compras, pagamentos, resumo, canceladas |
| **Comandas** | Visualização e gestão das comandas (status, bloqueio, exclusão, etc.) |
| **Novo Pedido** | Atalho para cadastrar um pedido no delivery (mesma tela do módulo Delivery) |
| **KDS - Tela de Pedidos** | Tela tipo KDS (Kitchen Display System) — semelhante ao painel de pedidos de redes de fast food. O card abre a lista de telas KDS configuradas |
| **Alertas Garçom** | Painel de alertas/chamados de garçom vindos das mesas |
| **Auto Serviço** | Tela de auto-serviço (self-service). Requer a permissão **Outros → Auto Serviço** |

---

## Estrutura de Módulos

```
SISTEMA SAG
├── Dashboard (KPIs, comparativos e gráficos)
├── IA (Inteligência Artificial integrada)
├── Principal
│   ├── Caixa (Frente de Caixa / PDV)
│   ├── Terminal de Comandas
│   ├── Caderneta
│   ├── Comandas
│   ├── Novo Pedido
│   ├── KDS - Tela de Pedidos
│   ├── Alertas Garçom
│   └── Auto Serviço
├── Cadastros
│   ├── Produtos
│   ├── Clientes
│   ├── Grupos
│   ├── Funcionários
│   ├── Cupom Desconto
│   ├── Entregadores
│   ├── Programa de Fidelidade
│   ├── Transportadoras
│   ├── Fornecedores
│   ├── Alteração de Preço Programada
│   ├── Grupos de Impostos
│   ├── Grupos de Acompanhamento
│   ├── Grupo de Preço Diferenciado
│   ├── Promoção
│   └── Gerenciador de Pizzas
├── Produções
│   ├── Receitas
│   ├── Nova Produção
│   ├── Consultar Produção
│   ├── Embalagens
│   └── Relatórios
├── Estoque
│   ├── Entrada de Nota
│   ├── Relatórios
│   ├── Locais de Estoque
│   ├── Estoque Atual
│   ├── Consulta de Notas
│   ├── Saída de Produtos
│   ├── Ajuste de Estoque
│   ├── Transferência de Estoque
│   ├── Inventário
│   ├── Pedido de Compra
│   ├── Cotação
│   ├── Produtos Fornecedores
│   ├── Transferência de Estoque Multiloja
│   ├── CFOP Parametrização
│   └── Análise de Preços
├── Financeiro
│   ├── Contas a Pagar
│   ├── Contas a Receber
│   ├── Contas Bancárias
│   ├── Categorias
│   ├── Conciliação Bancária
│   ├── Transferência Bancária
│   ├── Extratos
│   ├── Relatórios
│   ├── Ajuste de Conta
│   ├── Espécies
│   ├── Central de Faturas
│   └── Conciliação de Recebíveis
├── Delivery
│   ├── Novo Pedido
│   ├── Pedidos - Listagem
│   ├── Pedidos - Kanban
│   ├── Relatórios (Produção, Pedidos Resumidos, Por Origem, Completos, Por Entregador, Por Usuário, Consulta de Vendas, Produtos por Pedido, Resumo, Histórico, Taxas por Origem, Tempo por Status, Exportar Dados, Pedidos Alterados)
│   ├── Origens
│   └── Integrações (vínculo de produtos com as plataformas)
├── Romaneio (Fábricas — NF-e, boletos, faturas)
│   ├── Novo Pedido
│   ├── Romaneio - Lista
│   ├── Romaneio - Kanban
│   ├── Relatórios
│   └── Origens
├── NFe
│   ├── Emitir
│   ├── Gerenciar
│   ├── Configuração
│   ├── Inutilizar
│   ├── NFe Recebidas
│   ├── Vendas
│   ├── Pedidos
│   ├── Perfil de Impostos
│   └── Exportar
├── Relatórios
│   ├── Personalizados
│   ├── Fechamento de Caixa
│   ├── Faturamento
│   ├── Consultas
│   ├── Itens Cancelados
│   ├── Notas
│   ├── Vendas
│   ├── Listagem
│   ├── Caderneta
│   ├── Entradas e Saídas
│   ├── Comandas Abertas
│   ├── Venda por Usuário
│   ├── Comissões
│   ├── Lucros e MarkUp
│   ├── Compras
│   └── Outros
├── Outros
│   ├── Central de Usuários
│   ├── Ferramentas
│   ├── Grupo de Permissões
│   ├── Arqs. da Balança
│   ├── Etiquetas
│   ├── Impressoras Remotas
│   ├── Dados Cadastrais
│   ├── Certificado Digital
│   ├── Licença
│   ├── Config Espécies
│   ├── Cartão de Acesso
│   ├── Lei do Imposto
│   ├── Ferramentas CFe
│   ├── Exportar XML
│   ├── TEF
│   ├── Conf. Dispositivos Móveis
│   ├── Configurações de Estabelecimentos
│   └── SPED
└── Integrações
    ├── Cardápio / recebimento de pedidos
    │   ├── iFood
    │   ├── Rappi
    │   ├── Uber Eats
    │   ├── Open Delivery (genérico, Keeta, 99Food, ENVIO)
    │   ├── Delivery Direto
    │   ├── BeDelivery
    │   ├── AnotaAi
    │   ├── OiMenu
    │   ├── CINNDI
    │   ├── 88Digital
    │   ├── WABIZ
    │   └── Epadoca (Preço)
    ├── Logística de entrega
    │   ├── iFood Delivery
    │   ├── 99 Food
    │   ├── Uber Direct
    │   ├── Loocal
    │   └── Open Delivery
    ├── TEF / SiTef
    ├── Multiloja
    └── Automatizador
```

---

## Login

- Campo: **Usuário**
- Campo: **Senha**
- Após login, o menu superior exibe: **Alterar Senha** e **Sair**

---

## Atalhos de Teclado — Frente de Caixa

| Tecla | Função |
|---|---|
| F1 | Abre a tela **Todas as Funções** (ver seção abaixo) |
| F2 / Enter | Iniciar Venda (sem pedir CPF) |
| F3 | Iniciar Venda (solicita CPF em seguida) |
| F4 | Consulta de Comandas — se a opção **F4 Abre Terminal** estiver marcada no Config. Terminal, abre o Terminal de Comandas em vez da consulta |
| F5 | Cancelar Item |
| F6 | Cancelar Venda (sem venda aberta, oferece cancelar a última venda) |
| F7 | Pagamento de Caderneta |
| F8 | Consulta de Pedidos (abre tela para inserir código do pedido em aberto para finalização no caixa) |
| F9 | Consulta de Produtos |
| F10 | Últimas Vendas efetuadas |
| F11 | Entradas e Saídas (Sangria — registrar saídas e entradas de valores físicos) |
| F12 | Finalizar Caixa (pergunta confirmação; se habilitado no Config. Terminal e o usuário tiver permissão, aparece a função de lançar valores reais para o fechamento) |
| Ctrl + D | Desconto no Item (se nenhum item estiver selecionado, pergunta o número do item) |
| Ctrl + - | Desconto na Venda |
| Ctrl + E | Venda em Espera (se tem comanda vinculada, pergunta se deseja voltar para comanda original; se não tem, pede a comanda) |
| Ctrl + U | Última Venda |
| Ctrl + F | Inserir Comanda Parcial (inserir um ou mais produtos das comandas) |
| Ctrl + L | Extrato Programa de Fidelidade |
| Ctrl + B | Liga/desliga o bloqueio do F2 (grava na configuração do terminal) |
| Backspace / Delete | Cancela o item selecionado na lista |
| ESC | Minimiza a tela do caixa (sai do modo tela cheia) |

---

## Tela "Todas as Funções" (F1) — Frente de Caixa

O F1 abre um painel com todas as funções do caixa. Cada botão mostra o atalho equivalente, e as teclas numéricas executam as funções que não têm tecla F própria.

| Função | Atalho |
|---|---|
| Abrir Gaveta | 1 |
| Comandas Abertas | 3 |
| Caixa em Espera | 4 |
| Devolução de Venda | 5 |
| Devolução de Produto | 6 |
| Central NFCe | 7 |
| Central TEF | 8 |
| Bloqueia Caixa | 9 |
| Iniciar Venda | F3 |
| Consulta de Comandas | F4 |
| Cancelar Item | F5 |
| Cancelar Venda | F6 |
| Pag. de Caderneta | F7 |
| Consulta de Pedidos | F8 |
| Consulta de Produtos | F9 |
| Últimas Vendas | F10 |
| Entradas e Saídas | F11 |
| Finalizar Caixa | F12 |
| Desconto (Item) | Ctrl + D |
| Desconto na Venda | Ctrl + - |
| Comanda Parcial | Ctrl + F |
| Última Venda | Ctrl + U |
| Venda em Espera | Ctrl + E |
| Extrato Fidelidade | Ctrl + L |

> **ESC** fecha a tela de funções e volta ao caixa. Não existe a opção número **2** — a sequência de números é 1, 3, 4, 5, 6, 7, 8, 9.

---

## Atalhos — Tela de Formas de Pagamento

| Tecla | Função |
|---|---|
| F1 | Inserir CPF |
| F2 | Pesquisa Cliente |
| F3 | Inserir Observação |
| F4 | Inserir Voucher |
| F5 | Inserir Cupom Desconto |
| F6 | Cadastrar Cliente |
| F7 | Resgatar Benefício (programa de fidelidade) |
| F8 | Alterar Taxa de Serviço |

---

## Atalhos — Visualizador de Venda (Últimas Vendas)

| Tecla | Função |
|---|---|
| F1 | Imprimir Cupom Fiscal |
| F2 | Imprimir Cupom Fiscal (com CPF) |
| F3 | Imprimir Cupom Simples |
| F4 | Imprimir Comprovante Caderneta |
| F6 | Cancelar Venda |
| F7 | Trocar Formas de Pagamento |

---

## Atalhos — Terminal de Comandas

| Tecla | Função |
|---|---|
| F1 | Cancela Item (pergunta o número do item) |
| F2 | Pesquisar Produtos |
| F3 | Comandas Abertas |
| F4 | Limpar Comanda |
| F7 | Imprimir Prévia (pergunta o número de pessoas) |
| F8 | Transferir Comanda |
| F9 | Finalizar no Caixa |
| F10 | Inserir Pizza |
| F11 | Transferir Itens |
| F12 / ESC | Finalizar Terminal |
| Ctrl + D | Desconto no Item |
| Ctrl + - | Desconto na Comanda |
| Ctrl + E | Central de Mesas |
| Ctrl + F | Trocar Mesas |
| Backspace | Cancela Item Selecionado |

---

## Atalhos — Tela de Comandas (Gestão)

| Tecla | Função |
|---|---|
| F2 | Limpar Comanda |
| F3 | Bloquear Comanda |
| F4 | Desbloquear Comanda |
| F5 | Liberar Comanda |
| F6 | Adicionar Comandas |
| F7 | Excluir Comandas |
| F8 | Bloquear Comandas (lote) |
| F9 | Desbloquear Comandas (lote) |

---

## Atalhos — Tela de Novo Pedido

| Tecla | Função |
|---|---|
| F1 | Cancela Item |
| F2 | Consulta Produtos |
| F3 | Cancelar Pedido |
| F4 | Detalhes do Pedido |
| F5 | Consulta de Pedidos |
| F6 | Pedido Vinculado a Comanda |
| F7 | Últimos Pedidos Realizados |
| F10 | Inserir Pizza |
| F11 | Finalizar na Caderneta |
| F12 | Exibir Caixa |
| Ctrl + D | Desconto Item |
| Ctrl + - | Desconto no Pedido |
| ESC | Sair |

---

## Licença e Validação de Serial

O SAG é licenciado mensalmente. Normalmente a renovação é automática (feita online pelo próprio sistema). Quando por algum motivo a licença não é renovada automaticamente, o sistema exibe a **tela de Validar Serial** ao iniciar.

### Tela de Aviso de Licença

Aparece quando a licença está próxima do vencimento ou não foi renovada. Contém três botões:

| Botão | O que faz |
|---|---|
| **Validar Online** | Busca e aplica a serial atualizada pela internet. Use este botão primeiro — resolve na maioria dos casos. |
| **Gerenciador** | Abre o Gerenciador de Licença, com as informações do equipamento e o campo para digitar a serial manualmente. Se o computador não tiver internet, o cliente informa esses dados ao suporte T4L para receber a serial. |
| **Continuar** | Permite avançar sem renovar. |

**Comportamento conforme os dias restantes:**

| Situação | O que o SAG faz |
|---|---|
| Faltam **3 dias ou mais** | Mostra "Restam N dias de uso do sistema." e o botão **Continuar** já fica liberado |
| Faltam **1 ou 2 dias** | O texto fica em vermelho e o botão **Continuar** só é liberado após uma contagem regressiva de **30 segundos** ("Continuar em XXs") |
| Licença **expirada** | Título muda para "Licença Expirada" e o botão **Continuar** fica desabilitado — só é possível seguir renovando a licença |

> **Fluxo recomendado:** Tentar **Validar Online** primeiro. Se não funcionar (sem internet ou outro problema), acionar o suporte T4L e usar o **Gerenciador de Seriais** para renovar manualmente.

---

## Arquitetura Geral

- **Servidor:** computador central que hospeda o banco de dados. Todos os caixas e tablets se conectam a ele.
- **Caixas:** estações que rodam o SAG conectadas ao servidor pela rede local.
- **Tablets/Celulares:** usam o app SAG para lançar pedidos e comandas, sincronizando com o servidor.
- **Acesso remoto:** via AnyDesk, o suporte pode acessar o computador do cliente remotamente.

---

## Tipos de Estabelecimento Atendidos

| Tipo | Funcionalidades Mais Usadas |
|---|---|
| Padaria | Caixa, Balança, Produção, Caderneta |
| Restaurante | Comandas, Mesas, Produção, Relatórios |
| Pizzaria | Cadastro de Pizza, Acompanhamentos, Comandas |
| Mercado | Caixa, Estoque, NFC-e, Balança |
| Lanchonete | Caixa, Pedidos, Totem de Auto-Atendimento |
| Delivery | Pedidos, iFood, Open Delivery (Keeta/99Food), Romaneio |
| Fábrica | Romaneio, NF-e, Boletos, Faturas |
