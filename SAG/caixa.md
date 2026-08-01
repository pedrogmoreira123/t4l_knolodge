# Caixa — Documentação de Uso

Guia completo da operação de caixa no SAG: abertura, venda, pagamentos, descontos, devoluções, sangria e fechamento.

---

## Índice

1. [Abertura do Caixa](#1-abertura-do-caixa)
2. [Frente de Caixa](#2-frente-de-caixa)
3. [Lançar Produtos](#3-lançar-produtos)
4. [Aplicar Desconto](#4-aplicar-desconto)
5. [Cancelar Item ou Venda](#5-cancelar-item-ou-venda)
6. [Formas de Pagamento](#6-formas-de-pagamento)
7. [Vendas e Caixas em Espera](#7-vendas-e-caixas-em-espera)
8. [Últimas Vendas e Reimpressão](#8-últimas-vendas-e-reimpressão)
9. [Devolução de Venda](#9-devolução-de-venda)
10. [Sangria e Suprimento](#10-sangria-e-suprimento)
11. [Bloquear o Caixa](#11-bloquear-o-caixa)
12. [Fechamento do Caixa](#12-fechamento-do-caixa)
13. [Todas as Funções (F1)](#13-todas-as-funções-f1)

---

## 1. Abertura do Caixa

Antes de realizar qualquer venda, o operador precisa abrir o caixa para registrar o troco inicial disponível.

1. Ao iniciar o sistema, a tela de abertura de caixa abre automaticamente.
2. Informe o **Troco Inicial** — o valor em dinheiro físico que está no caixa no início do turno.
3. Se precisar contar as cédulas, use o botão da **Calculadora de Cédulas**.
4. Clique em **Abrir Caixa** para confirmar.

---

## 2. Frente de Caixa

| Área | O que exibe |
|---|---|
| **Campo Comanda** | Entrada do número da comanda |
| **Campo Produto** | Entrada do código ou EAN do produto |
| **Painel esquerdo** | Nome, valor unitário, quantidade e total do item |
| **Lista central** | Todos os itens lançados na venda atual |
| **Barra de totais** | Subtotal, desconto e valor total |
| **Rodapé** | Botões de função (F1 a F12) |

### Atalhos de teclado — Frente de Caixa

| Tecla | Função |
|---|---|
| **F1** | Tela "Todas as Funções" — menu completo |
| **F2** | Inicia uma nova venda (sem pedir CPF) |
| **F3** | Inicia uma nova venda e solicita o CPF |
| **F4** | Consulta de comandas (ou abre o Terminal de Comandas, se "F4 Abre Terminal" estiver marcado no Config. Terminal) |
| **F5** | Cancela o item selecionado |
| **F6** | Cancela a venda inteira |
| **F7** | Pagamento de caderneta |
| **F8** | Consulta pedidos de delivery |
| **F9** | Consulta produtos |
| **F10** | Exibe as últimas vendas |
| **F11** | Sangria / Entradas e Saídas |
| **F12** | Fecha o caixa |
| **Ctrl + D** | Desconto no item |
| **Ctrl + -** | Desconto na venda |
| **Ctrl + E** | Venda em espera |
| **Ctrl + U** | Última venda |
| **Ctrl + F** | Comanda parcial |
| **Ctrl + L** | Extrato do programa de fidelidade |
| **Backspace / Delete** | Cancela o item selecionado na lista |
| **ESC** | Minimiza a tela do caixa |

---

## 3. Lançar Produtos

1. Pressione **F2** (ou **F3**, se quiser informar o CPF do cliente) para iniciar uma nova venda.
2. Escaneie o código de barras ou digite o código manualmente no campo **Produto** e pressione **Enter**.
3. Ajuste a **Quantidade** se necessário.
4. O produto é adicionado à lista central automaticamente.
5. Repita para os demais produtos.

> Se a opção **Inicia Venda com Enter** estiver marcada no Config. Terminal, pressionar **Enter** com o campo de produto vazio também inicia a venda.

### Quantidade antes do produto

Com a opção **Quantidade Antes do Produto** marcada no Config. Terminal, é possível digitar `quantidade * código` (ex: `0,500*123`) direto no campo de produto.

### Lançar com comanda

1. Digite o número da comanda no campo **Comanda** antes de lançar produtos.
2. O sistema associa os itens àquela comanda.
3. A comanda pode ser retomada depois sem perder os itens.

> O campo **Comanda** só aparece se **Utiliza Comandas** estiver marcado no Config. Terminal. Use as setas **←** e **→** para alternar entre os campos Comanda e Produto.

---

## 4. Aplicar Desconto

### Desconto em um item — Ctrl + D

1. Pressione **Ctrl + D**
2. Se houver um item pré-selecionado na lista, o desconto é aplicado diretamente a ele
3. Se nenhum item estiver selecionado, o sistema pede o **índice do item** — número exibido na coluna **#** à esquerda da lista
4. Escolha o tipo: **Porcentagem (%)** ou **Preço de Venda (R$)**
5. Informe o valor e confirme

> Também funciona no **Terminal de Comandas** e no **Delivery** para desconto em item.

---

### Desconto na venda inteira — Ctrl + -

1. Pressione **Ctrl + -** durante a venda
2. Escolha o tipo: **Porcentagem (%)** ou **Preço de Venda (R$)**
3. Informe o valor e confirme

> Para que o desconto na venda funcione, é necessário que a espécie **Desconto** esteja cadastrada nas formas de pagamento. Sem ela, o **Ctrl + -** não funciona.

---

### Desconto pela tela de pagamento

Na tela de formas de pagamento, se a espécie **Desconto** estiver cadastrada, basta clicar sobre ela para aplicar o desconto na venda — funciona da mesma forma que o **Ctrl + -**.

---

> Descontos podem exigir permissão configurada no Grupo de Permissões do usuário.

---

## 5. Cancelar Item ou Venda

### Cancelar um item

1. Selecione o item na lista central.
2. Pressione **F5**.
3. Informe o motivo do cancelamento.
4. O item é removido e o total é recalculado.

### Cancelar a venda inteira

1. Pressione **F6** e confirme.
2. Todos os itens são removidos e a venda é encerrada sem registro.

> O cancelamento pode exigir senha do gerente, conforme configuração.

---

## 6. Formas de Pagamento

Após lançar todos os produtos, clique no **Total** para acessar a tela de pagamento.

### Atalhos da tela de pagamento

| Tecla | Função |
|---|---|
| **F1** | Inserir CPF |
| **F2** | Pesquisa Cliente |
| **F3** | Inserir Observação |
| **F4** | Inserir Voucher |
| **F5** | Inserir Cupom Desconto |
| **F6** | Cadastrar Cliente |
| **F7** | Resgatar Benefício (programa de fidelidade) |
| **F8** | Alterar Taxa de Serviço |

### Dinheiro

1. Selecione **Dinheiro**.
2. Informe o valor recebido do cliente.
3. O sistema calcula o troco automaticamente.
4. Confirme para finalizar.

### Cartão de Débito ou Crédito

1. Selecione **Débito** ou **Crédito**.
2. O sistema aciona a maquininha (TEF) automaticamente.
3. Siga as instruções na maquininha.
4. Após aprovação, a venda é concluída.

Para **parcelamento no crédito:** selecione o número de parcelas antes de acionar a maquininha.

### PIX

1. Selecione **PIX**.
2. O sistema gera um QR Code na tela.
3. O cliente escaneia e realiza o pagamento.
4. A venda é encerrada automaticamente após confirmação.

> O QR Code tem tempo de expiração. Se expirar, cancele e gere novamente.

### Múltiplas Formas de Pagamento

1. Selecione a primeira forma e informe o valor parcial.
2. Selecione a segunda forma e informe o restante.
3. O sistema controla a diferença e o troco automaticamente.

---

## 7. Vendas e Caixas em Espera

### Colocar a venda atual em espera — Ctrl + E

1. Com a venda aberta, pressione **Ctrl + E**.
2. Se a venda já tem comanda vinculada, o sistema pergunta se deseja devolver os itens para a comanda original.
3. Se não tem comanda, o sistema pede o número da comanda em que a venda ficará guardada.

### Retomar uma venda em espera

1. Pressione **F1** e escolha **Caixa em Espera** (tecla **4**).
2. Selecione a venda para retomá-la — o sistema carrega todos os itens já lançados.

### Ver comandas em aberto

Pressione **F1 → Comandas Abertas** (tecla **3**), ou use o **F4** (Consulta de Comandas).

> O limite de vendas simultâneas em espera é definido em **Config. Global → Caixa → Nº de Vendas em Espera**.

---

## 8. Últimas Vendas e Reimpressão

### Consultar vendas recentes

1. Pressione **F10**.
2. Escolha quantas vendas exibir (10, 25, 50 ou 300).
3. Marque **Todos os Caixas** para ver vendas de outros terminais.
4. Clique duas vezes em uma venda para ver os detalhes.

### Reimprimir um cupom

1. Abra a venda em **Últimas Vendas** (duplo clique).
2. No rodapé da tela de detalhes:
   - **F1** — Imprimir Cupom Fiscal
   - **F2** — Imprimir Cupom Fiscal (com CPF)
   - **F3** — Imprimir Cupom Simples (não fiscal)
   - **F4** — Imprimir Comprovante Caderneta
   - **F6** — Cancelar Venda
   - **F7** — Trocar Formas de Pagamento

---

## 9. Devolução de Venda

O SAG tem duas devoluções distintas, ambas no **F1**:

| Função | Atalho no F1 | Quando usar |
|---|---|---|
| **Devolução de Venda** | 5 | Devolver a venda inteira |
| **Devolução de Produto** | 6 | Devolver apenas um produto de uma venda |

1. Acesse **F1 → Devolução de Venda** (ou **Devolução de Produto**).
2. Informe a **quantidade** devolvida de cada produto.
3. O sistema calcula o valor total a ser devolvido.
4. Escolha como será feita a devolução:
   - **Gerar Voucher** — cria um crédito (vale) para uso futuro
   - **Estorno direto** — dependendo da forma de pagamento original
5. Confirme.

---

## 10. Sangria e Suprimento

### Sangria — Retirada de dinheiro do caixa

1. Pressione **F11**.
2. Selecione **Saída**.
3. Informe o **Valor**, o **Motivo** e uma **Observação** se necessário.
4. Clique em **Salvar**.

### Suprimento — Adição de dinheiro ao caixa

1. Pressione **F11**.
2. Selecione **Entrada**.
3. Informe o valor e o motivo e salve.

### Pagamento direto pelo caixa

Para registrar um pagamento a fornecedor feito com dinheiro do caixa:

1. Pressione **F11** > aba **Pagamentos**.
2. Informe o **Valor**, o **Fornecedor** e uma **Descrição**.
3. Salve.

### Lançamentos para funcionários

A tela do **F11** tem uma terceira aba, **Funcionários**, para lançar valores vinculados a um funcionário:

| Tipo | Uso |
|---|---|
| **Vales** | Vale concedido ao funcionário |
| **Adiantamento** | Adiantamento de salário |
| **Desconto** | Desconto a ser aplicado |
| **Outras** | Demais lançamentos |

> Estes lançamentos dependem das permissões **Financeiro → Lançar Extrato - Funcionário** e **Lançar Financeiro - Funcionário**.

> A sangria não pode ser feita com uma venda aberta — finalize a venda antes. O SAG também avisa quando o valor ultrapassa o limite definido em **Config. Terminal → Caixa → Avisa Sangria quando Valor é superior à**.

---

## 11. Bloquear o Caixa

1. Acesse **F1 → Bloqueia Caixa** (tecla **9**).
2. O caixa fica bloqueado — nenhuma venda pode ser realizada.
3. Para desbloquear, informe a senha do operador.

---

## 12. Fechamento do Caixa

1. Pressione **F12** e confirme.
2. Se a opção **Fechar Caixa Apenas Sem Comanda Aberta** estiver marcada e existirem comandas em aberto, o SAG avisa antes de prosseguir.
3. Se a opção **Lançar Valores ao Finalizar Caixa** estiver marcada (Config. Terminal → Caixa) **e** o usuário tiver a permissão **Relatórios → Fechamento de Caixa - Lançar Valores**, abre a tela de lançamento dos valores físicos.
4. Informe o **valor físico** em dinheiro no caixa (contagem real) por espécie.
5. O sistema aponta a **diferença** entre o esperado e o informado.
6. Confirme para encerrar o turno.

> Não é possível finalizar o caixa com uma venda aberta — finalize a venda primeiro.

### Impressões do fechamento

O que sai na impressora depende do que está marcado em **Config. Terminal → Impressoras → Imprimir Fechamento**:

| Opção | O que informa |
|---|---|
| **Totais das Vendas** | Totais de venda do turno |
| **Totais no Caixa** | Totais por forma de pagamento |
| **Divergências do Fechamento** | Diferença entre o esperado e o informado |
| **Mapa de Vendas** | Vendas organizadas por produto ou grupo |
| **Detalhamento Sangrias** | Entradas e saídas do turno |
| **Divergências do Fech. Tabelas** | Divergências em formato de tabela |

---

## 13. Todas as Funções (F1)

O **F1** abre a tela **Todas as Funções**, com todos os comandos do caixa em botões. Cada botão mostra o atalho equivalente, e as teclas numéricas executam as funções que não têm tecla F própria.

| Função | Atalho | O que faz |
|---|---|---|
| **Abrir Gaveta** | 1 | Abre a gaveta da registradora sem realizar venda |
| **Comandas Abertas** | 3 | Lista as comandas em aberto |
| **Caixa em Espera** | 4 | Retoma uma venda que foi colocada em espera |
| **Devolução de Venda** | 5 | Registra a devolução de uma venda completa |
| **Devolução de Produto** | 6 | Registra a devolução de um produto específico |
| **Central NFCe** | 7 | Central de contingência e reenvio de NFC-e |
| **Central TEF** | 8 | Central de ajustes/pendências do TEF |
| **Bloqueia Caixa** | 9 | Bloqueia a tela do caixa até informar a senha |
| **Iniciar Venda** | F3 | Inicia venda solicitando o CPF |
| **Consulta de Comandas** | F4 | Consulta de comandas |
| **Cancelar Item** | F5 | Cancela o item selecionado |
| **Cancelar Venda** | F6 | Cancela a venda inteira |
| **Pag. de Caderneta** | F7 | Recebimento de caderneta |
| **Consulta de Pedidos** | F8 | Traz um pedido em aberto para o caixa |
| **Consulta de Produtos** | F9 | Busca produto sem lançar |
| **Últimas Vendas** | F10 | Histórico de vendas recentes |
| **Entradas e Saídas** | F11 | Sangria / suprimento / pagamentos |
| **Finalizar Caixa** | F12 | Fechamento do caixa |
| **Desconto (Item)** | Ctrl + D | Desconto em um item |
| **Desconto na Venda** | Ctrl + - | Desconto no total da venda |
| **Comanda Parcial** | Ctrl + F | Traz parte dos itens de uma comanda para a venda |
| **Última Venda** | Ctrl + U | Abre a última venda finalizada |
| **Venda em Espera** | Ctrl + E | Coloca a venda atual em espera |
| **Extrato Fidelidade** | Ctrl + L | Extrato do programa de fidelidade |

> **ESC** fecha a tela e volta ao caixa. Não existe a opção número **2** — a sequência é 1, 3, 4, 5, 6, 7, 8, 9.
