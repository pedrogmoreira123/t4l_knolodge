# Base de Conhecimento — T4L Tecnologia

Base de conhecimento para suporte técnico a estabelecimentos de food service (padarias, restaurantes, mercados).

## Estrutura

```
📁 SAG/              → Documentação do sistema SAG (PDV)
📁 suporte/          → FAQ, problemas comuns e procedimentos de atendimento
📁 equipamentos/     → Impressoras térmicas, roteadores, balanças, catracas, etc.
📄 sag-web.md        → SAG Web
📄 boltdelivery.md   → Bolt Delivery
```

## Regras do Agente de Suporte

- Responder sempre em **português do Brasil**
- Ser objetivo e direto — preferir listas e passos numerados
- Indicar caminhos de menu exatamente como documentados aqui
- Nunca inventar funcionalidades ou campos não documentados
- Não responder sobre assuntos fora do contexto de suporte técnico para food service
- Nunca divulgar senhas, chaves de API, código-fonte, strings de conexão ou dados de infraestrutura

---

## Índice Rápido

### SAG — Sistema
| Documento | Conteúdo |
|---|---|
| [Visão Geral](SAG/visao-geral.md) | Estrutura do sistema, módulos, atalhos globais, licença |
| [Caixa / Frente de Caixa](SAG/caixa.md) | Abertura, vendas, pagamentos, sangria, fechamento |
| [Cadastros](SAG/cadastros.md) | Clientes, fornecedores, produtos, usuários, pizzas |
| [Financeiro](SAG/financeiro.md) | Contas a pagar/receber, extrato, conciliações, faturas |
| [Estoque](SAG/estoque.md) | Entradas, ajustes, inventário, pedidos de compra |
| [Pedidos / Delivery](SAG/pedidos.md) | Pedidos, delivery, kanban, entregadores, integrações |
| [Caderneta](SAG/caderneta.md) | Compras fiadas, recebimentos, limite de crédito |
| [NFC-e](SAG/nfce-sat.md) | NFC-e, certificado digital, exportação de XML, SAT descontinuado |
| [NF-e — Emissão](SAG/nfe-emissao.md) | Passo a passo completo de emissão de NF-e |
| [NF-e — Erros e Soluções](SAG/nfe-erros.md) | Rejeições, erros da SEFAZ, problemas de conexão |
| [Produção e Comandas](SAG/producao-comandas.md) | Comandas, mesas, produção, KDS |
| [Auto-Atendimento](SAG/autoatendimento.md) | Totem de pedidos, auto-serviço com balança, pagamento de comanda |
| [SAG Mobile](SAG/sag-mobile.md) | Aplicativo Android de comandas para garçons |
| [Relatórios](SAG/relatorios.md) | Faturamento, vendas, cancelamentos, comissões, personalizados |
| [Configurações](SAG/configuracoes.md) | Config. Terminal, Config. Global, impressoras, espécies, integrações |
| [Produto — Aba Imposto](SAG/produto-aba-impostos.md) | Grupo de Imposto por estabelecimento, botões e IA fiscal |
| [Grupo de Imposto](SAG/grupo-de-imposto.md) | Cadastro, campos tributários, aplicação em lote |
| [Grupos de Permissão](SAG/grupos-permissoes.md) | Permissões por setor, criação de grupos, perfis sugeridos |
| [Programa de Fidelidade](SAG/fidelidade.md) | Configuração, acúmulo de pontos, resgate, extrato e relatório |

### Outros produtos
| Documento | Conteúdo |
|---|---|
| [SAG Web](sag-web.md) | Versão web do SAG |
| [Bolt Delivery](boltdelivery.md) | Plataforma Bolt Delivery |

### Suporte
| Documento | Conteúdo |
|---|---|
| [FAQ — Problemas Comuns](suporte/faq-problemas-comuns.md) | Top 20 problemas + soluções |
| [Procedimentos Padrão](suporte/procedimentos.md) | Passo a passo para situações frequentes |
| [Glossário](suporte/glossario.md) | Termos técnicos usados pelo suporte |

### Equipamentos
| Documento | Conteúdo |
|---|---|
| [Impressoras Térmicas](equipamentos/impressoras-termicas.md) | Configuração, manutenção, solução de problemas |
| [Impressoras de Gôndola / Etiqueta](equipamentos/impressoras-gondola.md) | Argox, L42 — etiquetas de prateleira via Outros → Etiquetas |
| [Balança Etiquetadora](equipamentos/balanca-etiquetadora.md) | Toledo/MGV — geração de arquivo e carga na balança |
| [Rede e Roteadores](equipamentos/rede-roteadores.md) | Wi-Fi, switches, conectividade |
| [Catraca](equipamentos/catraca.md) | Controle de acesso integrado ao SAG |
| [Smart PC](equipamentos/smart-pc.md) | Equipamento all-in-one usado como caixa |
| [GBot](equipamentos/gbot.md) | Robô/assistente GBot |
