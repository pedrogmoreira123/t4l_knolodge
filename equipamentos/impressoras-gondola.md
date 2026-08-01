# Equipamentos — Impressoras de Etiqueta / Gôndola

Impressoras utilizadas para geração de etiquetas de gôndola (preço de prateleira) em estabelecimentos como mercados e padarias.

---

## Modelos Comuns

| Modelo | Observação |
|---|---|
| **Argox** | Linha de impressoras de etiqueta térmica — modelos OS, CP, etc. |
| **L42** | Impressora de etiquetas térmica |

---

## Função no SAG

**Caminho:** Outros → **Etiquetas**

O SAG gera as etiquetas de gôndola em **PDF** para impressão. O fluxo é:

1. Acesse **Outros → Etiquetas**
2. Filtre e selecione os produtos desejados
3. Clique no botão de **imprimir etiquetas**
4. O sistema gera um arquivo PDF com as etiquetas formatadas
5. Imprima o PDF na impressora de etiqueta configurada

> As etiquetas de gôndola são geradas como PDF — a impressão é feita pelo próprio Windows, assim como qualquer outro documento. Não é uma impressão direta via SAG como nos cupons fiscais.

### Filtros e opções da tela

| Opção | O que faz |
|---|---|
| **Recém Alterados** | Traz só produtos alterados em um período: Ontem, Hoje, Uma Semana, Quinze Dias ou Um mês — ideal para reetiquetar apenas o que mudou de preço |
| **Ocultar Matéria Prima** | Remove insumos da lista |
| **Converte Kg para 100g** | Imprime o preço por 100 g em vez de por quilo |
| **Selecionar todos / Desselecionar todos** | Marca ou desmarca a lista inteira |

A lista mostra Código, Descrição, Cod Barras, Preço, Grupo e SubGrupo.

### Editor de modelo de etiqueta

O botão de **configuração** (engrenagem) da tela de Etiquetas abre o **Editor de Etiqueta**, onde é possível:

- Criar, duplicar e excluir **Modelos** de etiqueta
- Definir **Largura (cm)** e **Altura (cm)** da etiqueta
- Montar os **Campos da etiqueta**: tipo, posição X/Y em cm, largura, altura, fonte, negrito e texto fixo

> Este editor fica dentro do SAG e pode ser usado pelo cliente. Ainda assim, para o primeiro ajuste de layout do rolo instalado, é mais rápido acionar o suporte T4L.

---

## Conexão

As impressoras de etiqueta podem ser conectadas via:

- **USB** — mais comum, conectada diretamente ao computador
- **Rede (TCP/IP)** — conectada via cabo de rede ou Wi-Fi

---

## Manutenção de Hardware

Qualquer dúvida ou dificuldade com a parte física da impressora (troca de ribbon, troca de rolo, limpeza de cabeçote, travamento de papel, etc.) **faz parte do escopo de suporte da T4L** — não orientar o cliente a consultar o fabricante ou manual por conta própria.

> Para manutenção física da impressora → **ESCALAR_SUPORTE** para atendimento remoto via AnyDesk ou visita técnica.

---

## Problemas Frequentes

### Etiqueta não imprime ou sai em branco
- Verifique se o rolo de etiqueta está posicionado corretamente
- Confirme que o lado sensível está voltado para o cabeçote
- Teste a impressora imprimindo um documento qualquer pelo Windows

### PDF gerado mas impressão não sai
- Verifique se a impressora correta está selecionada na janela de impressão do PDF
- Confirme que a impressora está online no Windows (Painel de Controle → Dispositivos e Impressoras)

### Etiqueta descentralizada ou cortando o texto
- O tamanho do papel configurado no PDF pode não bater com o rolo instalado
- Para ajuste de tamanho e layout das etiquetas → acionar suporte T4L

---

## Configuração

- **Layout da etiqueta** (tamanho e campos): pelo **Editor de Etiqueta**, dentro de Outros → Etiquetas → botão de configuração.
- **Parâmetros da etiquetadora** no sistema: **Config. Global → Etiquetadora** — aba técnica, só aparece com **Configurações Avançadas** marcado (senha técnica).

> Para o ajuste inicial ou qualquer dúvida de configuração, acionar o suporte T4L.
