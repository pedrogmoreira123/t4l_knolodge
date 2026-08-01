# SAG — Configurações

Módulo de parametrização do sistema, impressoras, integrações e permissões.

---

## Visão Geral das Configurações

O SAG possui dois níveis de configuração, acessíveis no canto superior direito da tela:

| Configuração | Escopo | Acesso |
|---|---|---|
| **Config. Terminal** | Configurações por máquina/caixa | Técnicos |
| **Config. Global** | Configurações para todo o sistema | Técnicos |

Além disso, existem configurações acessíveis pela aba **Outros** na barra superior.

---

## Configurações Avançadas (senha técnica)

Tanto o **Config. Terminal** quanto o **Config. Global** têm, no canto superior direito da janela, o checkbox **Configurações Avançadas**.

- Ele **exige senha técnica** para ser marcado.
- Enquanto está desmarcado, as abas técnicas ficam **ocultas** — o cliente nem enxerga que elas existem.

| Configuração | Abas que só aparecem com "Configurações Avançadas" marcado |
|---|---|
| **Config. Terminal** | Impressoras, NFC-e, TEF, Balança |
| **Config. Global** | Email, Etiquetadora, Módulos, NFC-e, Multiloja |

> Se o cliente disser que "não encontra a aba de impressoras", quase sempre é isso: as Configurações Avançadas estão desmarcadas.

---

## Config. Terminal (Por Máquina)

**Caminho:** Canto superior direito > **Config. Terminal**

Configurações específicas para cada terminal/caixa. Abas, na ordem em que aparecem: **Impressoras, NFC-e, TEF, Terminal PC, Caixa, Balança, Biometria, Personalizar, Produtos, Delivery, Auto Atendimento, Outros**.

### Aba: Impressoras
Configuração de impressoras para cada contexto:

**Frente de Caixa:**
- Configuração de Impressora (ex: EPSON TM-T20)
- Nº vias da Venda
- Opções de impressão: Lançamentos do Fechamento, Comprovante Cancelamento, Saldo na Caderneta, Ticket dos Itens, Comprovante Desconto
- Seção "Imprimir Fechamento": Totais das Vendas, Totais no Caixa, Divergências do Fechamento, Mapa de Vendas, Detalhamento Sangrias, Divergências do Fech. Tabelas
- Nº de vias (Caderneta) e Nº de vias (Sangria)

**Terminal PC:**
- Configuração de Impressora
- Nº vias
- Imprimir Produção (checkbox)

**Pedidos:**
- Configuração de Impressora
- Nº vias
- Imprimir Produção (checkbox)
- Imprimir Senha — Tipo Pedido (Retirada, etc.)

### Aba: NFC-e *(avançada)*
Configurações de emissão de Nota Fiscal de Consumidor Eletrônica para este terminal.

### Aba: TEF *(avançada)*
Configurações de Transferência Eletrônica de Fundos (pagamento com cartão/PIX) para este terminal.

### Aba: Terminal PC
Comportamento do Terminal de Comandas neste equipamento:

| Opção | Descrição |
|---|---|
| Utiliza Balança | Integra com balança de peso no terminal |
| Trava Pega Peso | Trava a leitura de peso |
| Comanda apenas com leitor | Exige leitor de código de barras para informar a comanda |
| Habilita Observações | Permite observação no item |
| Utiliza Usuário Padrão | Não pede operador a cada lançamento |
| Produto semi fixo - Cod Produto | Produto lançado automaticamente |
| Peso Máximo / Produto Peso Máximo | Limite de peso e produto usado quando excedido |
| Utiliza Mesa | Habilita controle de mesas |
| Inserir Acompanhamento | Pergunta acompanhamentos ao lançar |
| Terminal Cancela Antes de Finalizar | Permite cancelar itens antes de fechar a comanda |
| Usuário - Auto Atendimento | Usuário usado no modo auto-atendimento |
| Habilita Faixa de Comanda (de / à) | Restringe os números de comanda aceitos neste terminal |

### Aba: Caixa
Opções de comportamento do caixa neste terminal:

| Opção | Descrição |
|---|---|
| Acionamento Automático da Gaveta | Abre gaveta ao finalizar venda |
| Utiliza Comandas | Habilita uso de comandas |
| Quantidade Antes do Produto | Permite formato multiplicador (0,500*código) |
| Utiliza Balança | Integra com balança de peso |
| F4 Abre Terminal | F4 abre Terminal de Comandas em vez da consulta de comandas |
| Pagamento acima do saldo (Caderneta) | Permite pagar valor acima do saldo |
| Avisa Quantidade maior que 99 | Alerta para quantidades altas |
| Lançar Valores ao Finalizar Caixa | Exibe tela de valores reais no fechamento |
| Caixa Utiliza Taxa de Serviço | Habilita taxa de serviço |
| Taxa de Serviço Automática | Aplica taxa automaticamente |
| Caixa Solicita Vendedor Antes de Concluir a Venda | Pede identificação do vendedor |
| Utiliza acompanhamentos | Habilita acompanhamentos nos produtos |
| Inicia Venda com Enter | Enter inicia venda (além do F2/F3) |
| Caixa imprime descritivo venda | Imprime descrição na venda |
| Fechar Caixa Apenas Sem Comanda Aberta | Avisa/impede fechamento com comandas em aberto |
| Avisa item duplicado | Alerta ao inserir item já na venda |
| Mostra Observação do Item | Exibe observações dos itens |
| Solicita NSU para espécies sem TEF | Pede NSU para pagamentos fora do TEF |
| Comanda Apenas com Leitor | Exige leitor para comanda |
| Solicita cadastro de cliente | Solicita cadastro ao finalizar |
| Utiliza Tela Espelho — Ip Espelho | Habilita tela espelho (segundo monitor) e o IP dela |
| Avisa Sangria quando Valor é superior à | Define valor para alerta de sangria |
| Tipo Caixa | **Normal**, **Auto Atendimento Comanda**, **Auto Atendimento Pedido**, **Auto Atendimento Pedido com Comanda** ou **Auto Atendimento Mercado** |

### Aba: Balança *(avançada)*
Integração com balança de peso (leitura por porta serial):

| Campo | Valores |
|---|---|
| Porta | COM0 a COM10 |
| Nº Dígitos Quantidade | Quantidade de casas usadas na leitura |
| Modelo | Toledo, Urano US Pop ou Magellan |

### Aba: Biometria
| Campo | Valores |
|---|---|
| Utiliza Biometria | Liga/desliga o leitor biométrico |
| Leitor | Nenhum ou **Control iD** |

### Aba: Personalizar
Aparência e modo de operação do terminal:

- **Tema:** Claro ou Escuro
- **Tipo Background:** Cor ou Imagem — com Cor de Fundo Início/Fim ou Imagem de Fundo
- **Logo Frente de Caixa**
- **Tamanho da Fonte (Caixa)** e **Tamanho da Fonte (Terminal)**
- **Utiliza Touch** — modo para telas sensíveis ao toque
- **Utiliza Produtos Específicos** — usa a lista da aba Produtos
- **Teclas com Texto / Teclas com Ícones**
- **Não exibe Dashboard** — abre o sistema sem a aba Dashboard
- **Apenas Terminal** — a máquina só opera o Terminal de Comandas
- **Mensagem Promocional** — texto exibido na tela

### Aba: Produtos
Define a lista de produtos que aparece nos botões do terminal touch.

- Adicione por **Grupo**, **SubGrupo** ou **Produto** (com a opção **Adicionar Múltiplos**).
- Ao adicionar um grupo ou subgrupo, **todos** os produtos dele são utilizados.
- Se forem adicionados produtos específicos de um grupo/subgrupo, **apenas os adicionados** são mostrados.

### Aba: Delivery
Comportamento do módulo de pedidos neste terminal:

| Opção | Descrição |
|---|---|
| Inserir Acompanhamento | Pergunta acompanhamentos ao lançar item |
| Utiliza Balança | Habilita balança na tela de pedidos |
| Delivery Integra Caixa | Permite finalizar o pedido direto no caixa (F12 / F11) |
| Pedido solicita vendedor | Pede o vendedor ao lançar o pedido |
| Atualizar tela de pedidos automático | Atualiza a listagem sozinha |
| Habilita Forma Pagamento Caderneta | Permite finalizar pedido na caderneta |
| Modo Touch | Interface para tela sensível ao toque |
| Pedido padrão | Pedido, Orçamento ou Encomenda |
| Entrega padrão | Entrega ou Retirada |
| Status consulta padrão | Status pré-selecionado na consulta de pedidos |
| Tipo consulta padrão | Tipo pré-selecionado na consulta |
| Dias filtro padrão (Antes / Depois) | Período pré-carregado na consulta |
| Ordenar consulta de pedidos | Data Pedido ou Data Retirada |

### Aba: Auto Atendimento
| Campo | Descrição |
|---|---|
| Instrução da tela inicial | Mensagem exibida ao cliente (máx. 100 caracteres; em branco não exibe nada) |
| Modo de leitura inicial | Comanda e Produto, Somente Comanda ou Somente Produto |
| Tipo de Comanda | Impressa ou Física |

### Aba: Outros
| Campo | Descrição |
|---|---|
| Backup — Intervalo (horas) / Retenção (dias) / Último | Rotina de backup local do terminal |
| Faixa de mesa — Inicial / Final | Mesas que este terminal enxerga |
| Aviso por popup / Aviso sonoro | Como o terminal notifica novos pedidos/chamados |

---

## Config. Global (Todo o Sistema)

**Caminho:** Canto superior direito > **Config. Global**

Configurações que valem para todo o sistema. Abas, na ordem em que aparecem: **Email, Caixa, Delivery, Romaneio, Taxa de Entrega, Comandas, Estoque, Financeiro, Etiquetadora, Outros, Módulos, Autoatendimento, NFC-e, Multiloja**.

### Aba: Email *(avançada)*
Configurações do servidor de envio de e-mail usado pelo sistema.

### Aba: Caixa
| Campo/Opção | Descrição |
|---|---|
| Contra Vale | Produto usado como contra vale (ou "desativar") |
| Desconto Padrão | Percentual de desconto padrão |
| Taxa de Serviço (%) | Produto e percentual da taxa de serviço |
| Mensagem Taxa | Texto exibido ao cliente (ex: "Taxa de Serviço Opcional") |
| Taxa de serviço seletiva | Permite escolher em quais itens a taxa incide |
| Caixa apenas um dia | Caixa só funciona no dia da abertura |
| Nº de Vendas em Espera | Limite de vendas em espera |
| Caixa aviso sonoro para produto inexistente | Alerta sonoro para código inválido |
| Permite desconto no pagamento de caderneta | Habilita desconto na caderneta |
| Agrupa produtos na impressão | Agrupa itens iguais |
| Venda apenas com comanda | Obriga uso de comanda para vender |
| Imprimir senha venda | Imprime senha da venda |
| Quantidade de dígitos senha | Define tamanho da senha |
| Origem senha venda | Código Venda ou Código Pedido |

### Aba: Delivery
| Campo/Opção | Descrição |
|---|---|
| Integra Pedidos com Comandas | Pedidos de delivery geram comanda |
| Reimprimir Pedido Alterado | Reimprime ao alterar pedido |
| Imprime Código de Barras | Imprime código de barras no pedido |
| Gerar Código de Controle | Gera código de controle |
| Delivery Exige Entregador | Obriga selecionar entregador |
| Exibe Distância na Observação | Mostra distância no pedido |
| Ordena por | Grupo ou Inserção |
| DDD Telefone | DDD padrão (ex: 11) |
| Email Pedido | E-mail para envio de pedidos |
| Taxa de Entrega | Produto cadastrado como taxa |
| Tipo de Cálculo | **Por Cliente**, **Única**, **Distância** ou **Bairro** |
| Valor | Valor da taxa quando o tipo de cálculo é Única |
| Hora da Recontagem | Horário de virada da contagem de pedidos |
| Observação Padrão | Texto padrão nos pedidos |
| Integrações Logísticas | Botão que abre a configuração das plataformas de entrega |

### Aba: Romaneio
| Campo/Opção | Descrição |
|---|---|
| Email Romaneio / Email Fat. Online | E-mails usados pelo módulo |
| Categoria Fatura | Categoria financeira das faturas geradas |
| Permitir Todas as Formas de Faturamento | Libera todos os tipos de faturamento |
| Utilizar Valor da NFe para Faturar Pedidos | Fatura pelo valor da nota, não do pedido |
| Não permitir emissão de NFe sem fatura | Bloqueia NF-e sem fatura vinculada |
| Permitir matéria prima no romaneio | Aceita insumos no romaneio |
| Criar venda ao Faturar Pedido | Gera venda automática no faturamento |
| Observação Padrão | Texto padrão do romaneio |

### Aba: Taxa de Entrega
Tabela de taxas de entrega. O conteúdo muda conforme o **Tipo de Cálculo** escolhido na aba Delivery:

- **Bairro:** cadastra bairro, cidade e valor da taxa. O botão **pesquisar bairros** abre a seleção para preencher vários de uma vez.
- **Distância:** cadastra faixas de **Distância (Km)** e o **Valor** cobrado em cada faixa.

### Aba: Comandas
| Opção | Descrição |
|---|---|
| Permitir Abrir Comanda Simultâneo | Permite que a mesma comanda seja aberta em mais de um terminal ao mesmo tempo |

### Aba: Estoque
| Campo/Opção | Descrição |
|---|---|
| Estoque Padrão | Local de estoque usado por padrão |
| Avisa Venda de Produto com Quantidade Negativa | Alerta ao vender sem saldo |
| Importação de Nota altera o preço de custo | Atualiza o custo na entrada de nota |
| Solicita Motivo para Alterar Estoque | Exige justificativa em ajustes |
| Entrada de nota apenas com fatura | Bloqueia entrada sem fatura |
| Entrada de nota Atualiza NCM | Atualiza o NCM do produto pela nota |

### Aba: Financeiro
| Campo/Opção | Descrição |
|---|---|
| Integra Fechamento ao Financeiro | Lança o fechamento de caixa no financeiro |
| Integra Sangria ao Financeiro | Lança as sangrias no financeiro |
| Fornecedor/Cliente Obrigatórios | Exige favorecido no lançamento |
| Categoria Obrigatória | Exige categoria no lançamento |
| Categoria Apenas Filha | Só aceita categorias de último nível |
| Juros/Multa, Desconto, DIFAL | Categorias financeiras usadas nesses lançamentos |

### Aba: Etiquetadora *(avançada)*
Configurações de impressão de etiquetas de gôndola/prateleira.

### Aba: Outros
| Campo/Opção | Descrição |
|---|---|
| Sempre solicita senha | Pede senha a cada operação sujeita a permissão |
| Solicita motivo do cancelamento | Exige motivo ao cancelar item/venda |
| Usuário pode alterar todas as permissões | Libera edição irrestrita de permissões |
| Habilita Log | Ativa o registro detalhado de operações |
| Grupo de Imposto Padrão | Grupo aplicado a novos produtos (ou "desativar") |
| Email Envio NFCe | E-mail usado no envio da NFC-e ao cliente |
| Excluir ICMS destacado da base de cálculo de PIS/COFINS | Regra tributária |

### Aba: Módulos *(avançada)*
| Campo/Opção | Descrição |
|---|---|
| Módulo Pizzaria | Habilita pizza fracionada |
| Cálculo da Pizza | Por **maior** valor ou pela **média** dos sabores |
| Cálculo dos Acompanhamentos | Valor Cheio ou Valor por Partição |
| Quebra linha da descrição da pizza | Formatação da impressão |
| Módulo Restaurante | Habilita mesas/comandas de restaurante |

### Aba: Autoatendimento
Configurações do totem de auto-atendimento.

### Aba: NFC-e *(avançada)*
Configurações globais de emissão de NFC-e.

### Aba: Multiloja *(avançada)*
Restrições globais de cadastro na rede. Quando o **Ativar restrições de cadastro** está marcado, as opções abaixo bloqueiam criação e/ou alteração em **todos** os pontos do sistema (telas, importação por Excel, entrada de nota, etc.):

- Bloquear cadastro / alteração de **produtos**
- Bloquear cadastro / alteração de **grupos de acompanhamento**
- Bloquear cadastro / alteração de **grupos de imposto**
- Bloquear cadastro / alteração de **clientes**
- Bloquear cadastro / alteração de **fornecedores**
- Bloquear cadastro / alteração de **usuários**

> Use isso quando a matriz precisa ser a única a cadastrar — as filiais passam a só consumir os cadastros replicados.

---

## Aba Outros — Configurações Adicionais

**Caminho:** Aba **Outros** na barra superior

Funcionalidades de configuração e administração:

| Item | Função |
|---|---|
| **Central de Usuários** | Gerenciamento de usuários do sistema |
| **Ferramentas** | Ferramentas de manutenção e diagnóstico |
| **Grupo de Permissões** | Configuração de grupos de permissão |
| **Arqs. da Balança** | Gera arquivo de integração com a balança etiquetadora (MGV). Após gerar, o cliente importa no MGV e dá "carga na balança" para enviar os dados ao equipamento |
| **Etiquetas** | Configuração e impressão de etiquetas |
| **Impressoras Remotas** | Gerenciamento de impressoras em rede |
| **Dados Cadastrais** | Dados do estabelecimento |
| **Certificado Digital** | Instalação e gerenciamento do certificado digital |
| **Licença** | Informações da licença do sistema |
| **Config Espécies** | Configuração de espécies de pagamento |
| **Cartão de Acesso** | Configuração de cartões de acesso |
| **Lei do Imposto** | Configurações de lei do imposto |
| **Ferramentas CFe** | Ferramentas para CF-e/SAT (geração de XML, etc.) |
| **Exportar XML** | Exportação em lote dos XMLs de documentos fiscais |
| **TEF** | Configurações de TEF/SiTef |
| **Conf. Dispositivos Móveis** | Configuração de tablets e celulares |
| **Configurações de Estabelecimentos** | Cadastro e parâmetros dos estabelecimentos (multiloja) |
| **SPED** | Geração dos arquivos fiscais SPED |

> A configuração das telas **KDS (Tela de Pedidos)** **não** fica na aba Outros — ela é acessada pelo card **KDS - Tela de Pedidos** na aba **Principal**.

---

## Impressoras

**Caminho:** Config. Terminal > **Impressoras**

### Cadastrar Impressora
1. Acesse Config. Terminal > Impressoras
2. Clique em **Nova** (ícone +)
3. Informe:
   - **Nome** (identificação interna)
   - **Tipo** (USB, rede, serial)
   - **Endereço/Porta** (conforme tipo)
4. Clique em **Testar** para verificar a comunicação
5. Salve

### Regras de Impressão
Configuradas na aba Impressoras do Config. Terminal, nas seções:
- **Frente de Caixa** — impressora e vias para cupom do cliente
- **Terminal PC** — impressora e vias para terminal de comandas
- **Pedidos** — impressora e vias para pedidos de delivery

---

## Formas de Pagamento (Espécies)

No SAG as formas de pagamento se chamam **espécies**. Há dois caminhos:

| Caminho | Para que serve |
|---|---|
| **Outros → Config Espécies** | Cadastro e configuração das espécies (quais aparecem no caixa, comportamento de cada uma) |
| **Financeiro → Espécies** | Visão das espécies pelo lado financeiro |

- Habilitar ou desabilitar formas de pagamento disponíveis no caixa
- Cada forma tem um código numérico que o operador usa para selecioná-la
- Formas comuns: Dinheiro, Cartão Débito, Cartão Crédito, PIX, QR Code, Caderneta, Desconto, iFood, Ticket, etc.

> A espécie **DESCONTO** precisa estar cadastrada para que o **Ctrl + -** (desconto na venda) funcione. A espécie **CADERNETA** precisa estar cadastrada e ativa para o caixa para que o **F11** da tela de pedidos (Finalizar na Caderneta) funcione.

---

## Integrações

O SAG possui integrações com diversas plataformas:

### Cardápio / recebimento de pedidos

Tipos disponíveis no cadastro de integração: **iFood, Rappi, Uber Eats, Open Delivery, Open Delivery - Keeta, Open Delivery - 99Food, Open Delivery - ENVIO, Delivery_Direto, bedelivery, AnotaAi, OiMenu, CINNDI, 88Digital, WABIZ, Epadoca (Preço)**.

### Logística de entrega

Configuradas em **Config. Global → Delivery → Integrações Logísticas**: **Open Delivery, Uber Direct, iFood, Loocal, 99 Food**.

### Outras

| Integração | Função |
|---|---|
| TEF / SiTef | Gateway de pagamento com cartão/PIX |
| Balança | Integração com balanças de peso (Toledo, Urano US Pop, Magellan) |
| Multiloja | Sincronização com outras filiais |
| Biometria | Leitor Control iD |

> Todas as integrações são configuradas pela equipe técnica da T4L.

---

## Licença do Sistema

**Caminho:** Outros > **Licença**

- Exibe informações da licença ativa
- Número de caixas contratados
- Módulos habilitados
- Validade

> Se o sistema exibir alerta de licença expirada ou inválida, entre em contato com o suporte T4L.

---

## Programa de Fidelidade

**Caminho:** Cadastros > **Programa de Fidelidade**

- Define regras de acúmulo de pontos (ex: R$ 1,00 = 1 ponto)
- Define regras de resgate
- Configura validade dos pontos
