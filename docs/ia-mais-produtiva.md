# Por que, com IA, o desenvolvimento pode ser mais produtivo

> **Posição:** o atraso medido pelo METR mostra devs experientes usando uma ferramenta nova do jeito antigo. Quem já começa trabalhando com IA ganha mais. Esse ganho só se sustenta se a revisão e a manutenção do código continuarem sendo prioridade.

## 1. Produtividade: os números (retomando o que já foi apresentado)

| Estudo | Quem | Resultado |
|---|---|---|
| METR (BECKER et al., 2025) | 16 devs experientes, 246 tarefas, média de 5 anos no próprio repositório | **19% mais lentos** com IA, mas achavam que tinham sido **20% mais rápidos** |
| PENG et al., 2023 | Experimento controlado, tarefa isolada | **55,8% mais rápidos** com o Copilot |
| CUI et al., 2025 | 4.867 devs em Microsoft, Accenture e uma Fortune 100 | **+26,08% de tarefas concluídas** |

O resultado muda conforme **quem** usa a IA e **como** usa. O METR mediu especialistas em código que eles já dominavam. Os estudos com amostras maiores e perfis variados encontram ganho.

## 2. Custos: a ferramenta ficou mais capaz e mais barata

- **Claude Opus 5.5** (set/2026) custa US$4 por milhão de tokens de entrada e US$20 por milhão de saída, **20% menos que o Opus 5**. Segundo a Anthropic, sai **40% mais barato em cargas típicas** (ANTHROPIC, 2026).
- No **Terminal-Bench 4.0**, que testa tarefas de programação em terminal, foi de **52,3% (Opus 5) para 66,4% (Opus 5.5)** (ANTHROPIC, 2026).
- **Cuidado:** são números do fabricante e medem o modelo, não o time. Um sinal disso: só **22% das organizações** dizem ter conseguido escalar a IA entre áreas diferentes (PRESSWORKS, 2026).

## 3. Quem está começando agora x quem já tem estrada

- No estudo de Cui et al., **os devs com menos experiência adotaram mais a IA e tiveram os maiores ganhos** (CUI et al., 2025). Peng et al. já apontavam a IA como porta de entrada para quem está começando na carreira (PENG et al., 2023).
- **55,5%** dos devs em início de carreira (1 a 5 anos) usam IA todo dia, e os experientes são o grupo mais desconfiado (**20,7%** "desconfiam muito") (STACK OVERFLOW, 2025).
- **Leitura do grupo:** o ganho não depende da idade, e sim de quanto o **fluxo de trabalho** foi adaptado à IA. Quem não tem hábitos antigos para desaprender adapta mais rápido.

## 4. A ressalva: revisar e manter continua sendo obrigatório

- **66%** dos devs dizem que a maior frustração são soluções da IA "quase certas, mas não totalmente". **45,2%** dizem que depurar código gerado por IA leva mais tempo (STACK OVERFLOW, 2025).
- **Gerar código mais rápido também gera mais código para revisar, testar e manter.** O ganho real depende de práticas de Gerência de Configuração:
  - revisão humana em todo PR;
  - mudanças pequenas e rastreáveis;
  - testes automatizados;
  - histórico de versões claro.
- Código diferente do que um sênior escreveria **não é, por si só, código errado**. Mas só a revisão consegue separar um caso do outro.
