# O que é ser produtivo e por que é tão difícil medir

> **Posição:** terminar uma tarefa mais rápido é velocidade, e produtividade inclui mais coisas. Os estudos sobre IA vão de **55,8% mais rápido** a **19% mais lento** porque medem coisas diferentes, em pessoas diferentes, com métodos diferentes.

## 1. Velocidade é a mesma coisa que produtividade?

O framework SPACE divide a produtividade de desenvolvedores em cinco dimensões, e velocidade é só uma parte de uma delas (FORSGREN et al., 2021):

| Dimensão | O que observa |
|---|---|
| Satisfação e bem-estar | como a pessoa se sente no trabalho |
| Performance | o resultado entregue (defeitos, confiabilidade) |
| Atividade | volume de ações (commits, linhas, PRs) |
| Comunicação e colaboração | trabalho em equipe |
| Eficiência e fluxo | progresso sem interrupção |

Para os autores, produtividade não cabe numa métrica só.

O DORA 2024 mostra isso na prática. Um aumento de 25% na adoção de IA esteve associado a ganhos para a pessoa e a perdas na entrega (DORA, 2024):

| Indicador | Associação com +25% de adoção de IA |
|---|---|
| Qualidade da documentação | +7,5% |
| Qualidade do código | +3,4% |
| Velocidade da revisão de código | +3,1% |
| Throughput de entrega | −1,5% |
| Estabilidade de entrega | −7,2% |

A pessoa pode ficar mais rápida enquanto a entrega da equipe fica mais lenta e mais instável. O relatório diz que isso não melhora sem o básico, como lotes pequenos e testes robustos. No DORA 2025, com quase 5.000 profissionais, a relação com throughput virou positiva, mas a relação com estabilidade continuou negativa (DORA, 2025).

**Limite:** o DORA é questionário. Mostra associação, não causa.

## 2. Por que os estudos discordam

| Estudo | Quem | O que mediu | Resultado |
|---|---|---|---|
| PENG et al., 2023 | 95 freelancers (45 com Copilot, 50 sem), tarefa de laboratório | tempo para criar um servidor HTTP em JavaScript | **55,8% mais rápido** (IC 95%: 21% a 89%) |
| ZIEGLER et al., 2022 | 2.047 respostas de usuários do Copilot, casadas com dados de uso | qual métrica de uso acompanha a percepção de produtividade | taxa de aceitação, com correlação de **0,24** |
| BECKER et al., 2025 (METR) | 16 devs experientes, 246 tarefas nos próprios repositórios | tempo para fechar issues reais | **19% mais lento** (IC: +2% a +39%) |
| DORA, 2024 | questionário com profissionais de várias empresas | entrega da equipe | throughput **−1,5%**, estabilidade **−7,2%** |

Peng mede uma tarefa pequena e nova, o cenário mais favorável à IA. O METR mede issues reais em projetos que os devs conhecem há anos, o menos favorável. Ziegler não mede tempo; procura a métrica que acompanha a sensação de produtividade. O DORA olha para a equipe, e não para a pessoa. Os números respondem perguntas diferentes.

## 3. Por que é tão difícil medir

### A percepção erra nos dois sentidos

| Estudo | O que os devs achavam | O que foi medido |
|---|---|---|
| METR (BECKER et al., 2025) | 20% mais rápidos | 19% mais lentos |
| PENG et al., 2023 | 35% mais rápidos | 55,8% mais rápidos |

Os próprios autores do Ziegler, que são do GitHub, escrevem que produtividade percebida não é necessariamente produtividade real (ZIEGLER et al., 2022). O arquivo [produtividade-percebida.md](produtividade-percebida.md) aprofunda esse ponto.

### Métricas de atividade enganam

Linhas de código e sugestões aceitas medem atividade. A correlação de 0,24 do Ziegler deixa a maior parte da percepção sem explicação, e os autores lembram que uma tecla Tab com defeito aceitaria sugestões sozinha sem ninguém produzir mais por isso (ZIEGLER et al., 2022).

### O próprio METR não conseguiu repetir a medição

O METR tentou repetir o estudo a partir de agosto de 2025, com 57 devs e mais de 800 tarefas (METR, 2026):

- de 30% a 50% dos devs deixaram de enviar tarefas que não queriam fazer sem IA, então os mais otimistas saíram da amostra;
- com vários agentes rodando ao mesmo tempo, o dev fazia outra coisa enquanto esperava, e o tempo por tarefa perdeu o sentido;
- as novas estimativas (−18% e −4% no tempo) tiveram intervalos que incluem zero, e os autores chamam a evidência de "muito fraca".

No estudo original, 56% dos participantes nunca tinham usado o Cursor. Willison levanta a hipótese de que a curva de aprendizado pesou no resultado (WILLISON, 2025).

## 4. Tipos de fonte

| Fonte | Tipo | Sustenta | Não sustenta |
|---|---|---|---|
| METR, 2025 | preprint, experimento controlado | efeito naquele cenário, com IA do início de 2025 | efeito com as ferramentas atuais |
| PENG et al., 2023 | preprint, autores da Microsoft e do GitHub | ganho em tarefa curta e isolada | ganho em sistemas grandes |
| ZIEGLER et al., 2022 | artigo arbitrado, autores do GitHub | qual métrica acompanha a percepção | ganho real de produtividade |
| DORA 2024 e 2025 | pesquisa por questionário | associações em larga escala | causalidade |
| METR, 2026 | nota metodológica | que o desenho antigo deixou de medir bem | um número novo confiável |
| WILLISON, 2025 | opinião (blog) | hipótese para o resultado do METR | evidência |

Dois dos estudos (Peng e Ziegler) avaliam o Copilot e foram feitos por quem vende o Copilot. Isso não invalida o método, mas vale lembrar ao comparar com o METR, que é independente.

## 5. Ligação com Gerência de Configuração

As métricas DORA (frequência de deploy, lead time, taxa de falha e tempo de recuperação) saem do controle de versão e do pipeline, dados que a Gerência de Configuração já produz. Para avaliar a IA numa equipe, a proposta é:

- comparar essas métricas no mesmo time, antes e depois da adoção;
- olhar estabilidade junto com throughput, porque entregar mais rápido e reverter mais vezes não é ganho;
- usar a percepção do dev como uma das dimensões, nunca como a medida.

**Nossa resposta:** velocidade é só uma parte da produtividade, e nenhuma medida isolada mostra com confiança o efeito da IA. A medida mais defensável combina várias dimensões e acompanha a mudança até ela estar entregue e estável.
