# A sensação de produzir mais é prova de maior produtividade?

> **Posição:** a IA pode facilitar o desenvolvimento. Mas a sensação de avançar mais rápido precisa ser acompanhada de resultados: uma solução que funcione, considerando também o esforço de revisão e correção.

## 1. O que mostra o artigo científico

Em **The Fast and Spurious: Developer Productivity with GenAI**, Afroz et al. (2026) analisaram **415 respostas válidas** de profissionais de software. “Usuários frequentes” são aqueles que responderam usar IA **frequentemente ou sempre**.

| Entre os usuários frequentes de IA | Resultado relatado |
|---|---|
| Linhas de código alteradas por dia | **72,7%** relataram aumento: **47,2%** “mais” e **25,5%** “muito mais” |
| Tempo dedicado à revisão de código | **84,3%** relataram que a IA **não reduziu** esse tempo |

Esses percentuais representam participantes, não o tamanho da mudança: **72,7% não é o aumento na quantidade de código**, e **84,3% não significa que todos passaram a revisar por mais tempo**.

**Onde encontrar:** seção **4.1 — “Productivity Across SPACE Dimensions (RQ1)”**, parágrafos **“Performance”** (P1) e **“Activity”** (A7). A definição de frequência está na seção **3.2**.

**Limite:** o estudo analisa percepções, não produtividade medida diretamente; não demonstra causalidade. Os autores reconhecem limitações da amostra na seção **5**. A versão consultada é a **v2, de 5 de abril de 2026**; a primeira versão é de **28 de outubro de 2025**.

## 2. Gerar mais código pode mudar onde o esforço acontece

- Na análise geral, as medianas das cinco dimensões avaliadas ficaram na faixa neutra. Os resultados variaram entre os indicadores (AFROZ et al., 2026, seção 4.1).
- Participantes relataram trocar parte da escrita manual por verificação, revisão e correção das respostas da IA (AFROZ et al., 2026).
- **Leitura desta contribuição:** precisamos acompanhar o trabalho até a entrega aceita para avaliar se essa mudança trouxe ganhos.
- **Exemplo ilustrativo:** uma função gerada em poucos segundos ainda pode exigir ajustes para atender aos requisitos do projeto.

**Onde encontrar os relatos sobre mudança de esforço:** seção **6.1 — “The Redistribution of Effort”**.

## 3. Os dados da OpenAI como complemento

- Na publicação de **6 de setembro de 2026**, a OpenAI relata que seus pesquisadores escrevem código mais rápido e realizam mais experimentos. A empresa reconhece, porém, que a relação entre quantidade de código e avanço da pesquisa é incerta (OPENAI, 2026).
- No período descrito como **“últimos 6 meses”**, mais da metade das tarefas bem-sucedidas da faixa de **4 a 8 horas** exigiu uma ou mais intervenções humanas. Essa faixa indica o **tempo estimado que uma pessoa levaria para executar a tarefa**, não a duração do trabalho do agente (OPENAI, 2026).

**Onde encontrar na página em português:**

- Seção **2 — “Pesquisadores escrevem mais código e realizam mais experimentos”**, para os ganhos relatados.
- Seção **“Apêndice: métodos usados nesta publicação”**, primeiro parágrafo. Use Ctrl + F e procure **“Alguns indicadores”**.
- Seção **3 — “O trabalho delegado a agentes está mudando”**. Procure **“mais da metade”**.

**Limite:** são dados internos e preliminares. A OpenAI também informa que seus recursos computacionais cresceram, portanto o aumento nos experimentos não pode ser atribuído apenas à IA. A análise de sucesso exclui resultados incertos.

**Tipo de fonte:** publicação institucional, usada como complemento ao artigo científico.

## 4. A conclusão: acompanhar a entrega completa

**Proposta desta contribuição:** avaliar o uso da IA com três perguntas:

- Quanto tempo de trabalho foi necessário até a mudança ser aceita?
- A solução atende aos requisitos e passa nos testes relevantes?
- Quanto esforço foi necessário para revisar e corrigir o código?

Na Gerência de Configuração, os **pull requests, testes e histórico de alterações** ajudam a acompanhar a entrega. Para avaliar o tempo de trabalho, também precisamos registrar o esforço empregado, pois o intervalo entre abrir e aceitar um pull request pode incluir espera.

**Nossa resposta:** sentir-se mais produtivo é uma informação relevante, mas para afirmar que houve ganho, precisamos observar também a entrega e o esforço de toda a equipe.