# Saúde · Grande Porto Alegre — Console ABM DataCentrics (v01)

Console de inteligência do cluster **Saúde** do programa ABM 360°, entregue pela
Esparta à DataCentrics. Arquivo único de 1,4 MB, sem dependência externa — abre
offline com duplo clique.

> Este é o segundo cluster do programa. O primeiro, **Serviços Financeiros**,
> tem console próprio com 606 decisores em 31 contas.

## O que tem dentro

| Camada | Volume |
|---|---|
| Decisores com papel, senioridade e confiança | **81** |
| Contas com comitê, roteamento e evidência de nuvem | **8** |
| Contas com perfil DISC | 6 |
| Avatares embutidos | 64 |
| Produtos do Catálogo DCX v10 | 13 |
| Copy por papel · Challenger · frameworks | 13 papéis |

## As 8 contas

| Conta | UF | Segmento | Decisores | Comitê | D4 |
|---|---|---|---|---|---|
| Hospital Mãe de Deus | RS | Hospital privado | 20 | 4/7 | 3 |
| Hapvida NotreDame Intermédica | SP | Operadora nacional | 15 | 5/7 | **10** |
| Unimed Porto Alegre | RS | Operadora | 15 | 6/7 | 3 |
| Grupo Dimed / Panvel | RS | Farma/varejo | 15 | 5/7 | 6 |
| Pixeon | SC | ISV healthtech | 12 | 4/7 | 8 |
| Grupo São Pietro | RS | Hospital privado | 4 | 2/7 | 2 |
| Clinoson | RS | Clínica | 0 | 0/7 | 0 |
| Radimagem | RS | Diagnóstico por imagem | 0 | 0/7 | 0 |

**Concentração no Rio Grande do Sul**: 6 das 8 contas, o que é coerente com a
operação da DCX ser gaúcha — diferente do cluster financeiro, concentrado em SP.

## Abas

- **Mapa** — distribuição das contas por estado e região
- **Contas** — filtros por conta, região, porte, segmento, nuvem, roteamento e sinal;
  cada conta abre com comitê, ordem de entrada, roteamento e a aba de Tecnologia
- **Decisores** — busca e filtros cumulativos por conta, papel, senioridade e confiança;
  cada pessoa tem ficha de abordagem e exportação para Pipedrive
- **Sinais** — contas ordenadas pela força do gatilho
- **Referência** — catálogo, copy, Challenger, battlecard, regra de stack, método WAR,
  cobertura, technográfico e geografia

## Acessibilidade

Navegação por teclado nos elementos clicáveis, seleção exposta a leitor de tela e
atalhos: `/` busca · `↑ ↓` andam na lista · `Enter` abre a ficha · `Esc` sai.

## Procedência dos dados

| Camada | Origem |
|---|---|
| Decisores e cargos | LinkedIn via Apify |
| Evidência de nuvem | DNS de subdomínios de aplicação e de serviços internos |
| Sinais de timing | troca de liderança, notícias e vagas abertas |
| DISC | análise comportamental por decisor |

## Limites declarados

- **O papel é inferido do cargo**, exceto os marcados como `validado`. A coluna
  Confiança indica onde confiar — a validação por amostra ainda não foi feita.
- **Duas contas estão com zero decisores mapeados** — Clinoson e Radimagem. Não é
  falha de exibição: a coleta não retornou perfis. Ou não há presença digital
  suficiente, ou o porte não comporta comitê formal.
- **Nenhuma conta tem executivo designado.** Diferente do cluster financeiro, a
  atribuição de carteira ainda não foi feita neste cluster.
- **Sinal de timing expira**: liderança 6 meses · M&A e captação 9–12 · incidente 6 ·
  vaga 3. Sem rescore mensal, a lista envelhece.
- **O D4 está baixo em quase todas** — só Hapvida (10) atinge o gate de abordagem.
  Cluster com menos gatilhos noticiados que o financeiro.

## Publicar

1. Subir `index.html`, `robots.txt` e `.gitignore` na raiz do repositório
2. **Settings → Pages** → Source: `main` / root → Save
3. O link sai em `https://<usuario>.github.io/<repo>/`

A meta tag `noindex` e o `robots.txt` impedem que o painel apareça em busca.
O link segue acessível a quem o tiver.

Para exigir login, colocar **Cloudflare Access** na frente do Pages — gratuito
até 50 usuários, libera por e-mail com código de uso único.

## Governança

Dados de decisores tratados sob legítimo interesse para prospecção B2B, com
finalidade restrita à abordagem comercial. O perfilamento comportamental usa apenas
informação pública e profissional. Não há decisão automatizada que afete direitos do
titular — o score prioriza a fila; a decisão de abordar é humana.

---
Esparta · Confidencial — DataCentrics
