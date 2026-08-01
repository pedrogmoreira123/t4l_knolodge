# SAG — NFC-e

Módulo fiscal para emissão de documentos eletrônicos ao consumidor final.

---

## Conceitos

| Sigla | Nome | Uso |
|---|---|---|
| NFC-e | Nota Fiscal de Consumidor Eletrônica | Emitida diretamente pelo SAG na venda ao consumidor final |
| NF-e | Nota Fiscal Eletrônica | Para vendas entre empresas (B2B) |
| XML | Arquivo eletrônico | Representação digital do documento fiscal |
| Certificado Digital | Arquivo de autenticação | Obrigatório para emissão de NFC-e |

---

## NFC-e — Emissão na Venda

A NFC-e é emitida automaticamente ao finalizar a venda, desde que:
- O caixa tenha NFC-e habilitado
- O cliente informe CPF/CNPJ (ou a venda seja sem identificação, conforme legislação estadual)
- Os produtos tenham CST e CFOP configurados corretamente

---

## NFC-e — Problemas Frequentes

### Erro ao emitir — produto sem configuração fiscal
- Acesse: **Cadastros > Produtos** > selecione o produto > aba **Imposto**
- Verifique se o produto tem um **Grupo de Imposto** vinculado — sem ele, a emissão não funciona
- O CST e o CFOP são definidos dentro do **Grupo de Imposto** vinculado ao produto — consulte a contabilidade para ajustar

### NFC-e não emite mas venda passa
- Verifique se NFC-e está habilitado no caixa específico
- Reinicie o SAG após qualquer alteração de configuração

---

## SAT / CF-e — Descontinuado

O SAT (Sistema Autenticador e Transmissor) foi descontinuado em 2025.
Estabelecimentos que utilizavam SAT para emissão de cupom fiscal devem
migrar para **NFC-e**, que passa a ser o único modelo aceito para emissão
de cupom ao consumidor final.

> Dúvidas sobre a migração: entrar em contato com o suporte T4L.

---

## XML — Exportar e Baixar

### XML em lote por período — envio mensal para contabilidade

**Caminho:** Outros > **Exportar XML**

1. Informe o **período** (Início e Término)
2. Selecione os tipos a incluir: **NFCe**, **NFE - Emitidas**, **NFE - Recebidas**
3. Marque as opções desejadas:
   - **Incluir Canceladas**
   - **Incluir Relatório**
   - **Incluir Inutilizadas**
   - **Incluir DANFE**
   - **Buscar Online Cupons Faltantes (SAE SP)** — apenas para SP, busca na SEFAZ os cupons que não estão no banco local
4. Em **Escolher pasta de destino**, clique em **Selecionar...** e indique onde salvar
5. Para enviar por e-mail: marque **Enviar arquivos por email** e informe o **Email** (e a **Cópia**, se quiser)
6. Clique em **gerar** — o arquivo é gerado na pasta escolhida ou enviado por e-mail

> Use este caminho para enviar os XMLs mensais à contabilidade.

---

### XML individual de NF-e

**Caminho:** NFe > **Gerenciar**

1. Localize a nota na lista
2. Na linha da nota com status **Autorizada**, clique no **segundo botão** (ícone XML)
3. O arquivo é baixado no computador

---

### XML individual de NFC-e

**Caminho:** Relatórios > **Consultas** > **Vendas**

1. Localize a venda na lista
2. Clique no botão **XML** na linha da venda
3. O arquivo é baixado no computador

---

## Certificado Digital

O certificado digital é obrigatório para emissão de NFC-e. Existem dois tipos:

| Tipo | Formato | Descrição |
|---|---|---|
| **A1 - Arquivo** | `.pfx` / `.p12` | Arquivo digital salvo no computador — o mais comum (**recomendado** pelo SAG) |
| **A3 - Cartão** | Token / Smart Card | Dispositivo físico conectado por USB |

### Aplicar Certificado A1 no SAG

1. Acesse **Outros > Certificado Digital**
2. Na pergunta "Qual o tipo do seu certificado?", escolha **A1 - Arquivo**
3. Clique em buscar arquivo e selecione o arquivo `.pfx` ou `.p12`
4. Informe a **senha do certificado**
5. Clique em **Salvar**
6. **Feche e reabra o SAG** para aplicar

> A tela de certificado também tem as opções **Trocar Certificado** (substituir o atual) e **Adquirir Novo Certificado**.

### Informações Importantes

- O certificado pode ser aplicado em **qualquer computador que tenha o SAG instalado**
- Qualquer usuário consegue aplicar seguindo o passo a passo acima
- Validade: geralmente 1 ou 3 anos — monitorar vencimento
- Se certificado **vencido**: o cliente renova junto à contabilidade ou certificadora e fornece novo arquivo `.pfx`
- Se o cliente tiver dificuldade após seguir os passos: acionar suporte T4L para auxílio remoto via AnyDesk

### Erros Comuns

| Mensagem | Causa | Ação |
|---|---|---|
| "Certificado vencido" | Certificado expirou | Renovar com a contabilidade |
| "Senha incorreta" | Senha do `.pfx` errada | Confirmar senha com quem gerou o certificado |
| NFC-e não emite após aplicar | SAG não foi reiniciado | Fechar e reabrir o SAG |

---

## NF-e

Para emissão de nota fiscal eletrônica entre empresas (B2B), consulte os guias específicos:

- [Guia de Emissão Passo a Passo](nfe-emissao.md)
- [Erros, Rejeições e Soluções](nfe-erros.md)
