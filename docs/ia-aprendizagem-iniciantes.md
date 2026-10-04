# A IA ajuda o iniciante a aprender ou apenas a terminar a tarefa?

**Material de pesquisa para a apresentação de Gerência de Configuração.**

**Tema do grupo:** produtividade — “A IA torna os desenvolvedores melhores?”

## 1. Recorte e posicionamento proposto

O texto [ia-mais-produtiva.md](ia-mais-produtiva.md) já discute ganhos de execução, custos e revisão. Este material acrescenta a questão da formação de conhecimento: o que a pessoa consegue explicar, corrigir e fazer depois de receber ajuda?

**Tese proposta para o grupo:** a IA pode ajudar a executar tarefas, mas a aprendizagem precisa ser avaliada separadamente. Para dizer que alguém se tornou um desenvolvedor melhor, precisamos observar compreensão, capacidade de manutenção e autonomia, além da entrega inicial.

Esta é uma síntese argumentativa, não uma citação literal de pesquisador. Os resultados das fontes estão identificados abaixo; as perguntas de avaliação e práticas sugeridas são propostas para discussão.

“Iniciante” pode significar três situações diferentes:

- Uma pessoa começando a programar, ainda aprendendo lógica e estruturas básicas.
- Um profissional com pouca experiência de trabalho, mas que já sabe programar.
- Um desenvolvedor experiente aprendendo uma tecnologia que ainda não conhece.

Não podemos usar um resultado obtido com um desses públicos como descrição automática dos outros.

**Atualização temporal:** em fevereiro de 2026, o METR explicou que seu experimento posterior teve problemas na seleção de participantes e tarefas, além de dificuldades para medir o tempo com agentes simultâneos. Os autores consideram os dados um sinal pouco confiável do efeito atual. Isso impede usar o resultado de 2025 como retrato permanente das ferramentas. [Fonte: atualização do METR][r7].

## 2. Perguntas e respostas

### 1. Se o código funciona, por que importa saber se a pessoa aprendeu?

Porque o software continuará mudando. Será preciso adaptar requisitos, investigar falhas e revisar alterações. Uma solução pronta pode resolver a demanda inicial sem revelar se quem a entregou consegue manter o sistema. Para o trabalho, podemos distinguir **entrega funcional**, **compreensão naquele momento** e **capacidade de aplicar o conhecimento depois**.

### 2. A IA pode aumentar a produtividade de quem tem menos experiência?

Pode, em determinados contextos. Cui et al. encontraram ganhos maiores de execução entre profissionais menos experientes. Isso apoia o argumento de que a assistência pode reduzir barreiras no trabalho, mas não demonstra que alunos aprendem mais. [Fonte: Cui et al.][r5].

### 3. Então a IA necessariamente prejudica a aprendizagem?

Não há base para uma afirmação universal. O experimento de Shen e Tamkin encontrou menor compreensão na avaliação imediata após aprender a biblioteca Trio com assistência de IA. Os participantes já usavam Python, mas não conheciam essa biblioteca. A pergunta mais útil é como o conhecimento prévio, a tarefa e a forma de assistência alteram o resultado. [Fonte: Shen e Tamkin][r1].

### 4. Existem sinais de benefício para alunos iniciantes?

Sim. Kazemitabaar et al. estudaram alunos que estavam começando na programação textual e combinaram geração de código com exercícios de modificação manual. O resultado oferece um contraponto à ideia de que qualquer geração de código necessariamente prejudica o aprendizado. [Fonte: Kazemitabaar et al., 2023][r12]. Isso não comprova ausência de prejuízo em todo contexto. O CodeAid também exemplifica assistência concebida para apoiar o raciocínio. [Fonte: CodeAid][r3].

### 5. Qual é a diferença entre receber ajuda e depender dela?

Para nossa discussão, receber ajuda é usar apoio e ainda conseguir justificar decisões ou resolver uma variação do problema. Dependência seria precisar de uma nova resposta pronta sempre que algo muda. Essa distinção é um critério proposto para avaliação, não um diagnóstico sobre qualquer pessoa que utilize IA.

### 6. Por que uma explicação clara não garante que eu aprendi?

Entender uma explicação enquanto ela está na tela não é a mesma coisa que conseguir usar a ideia em outra situação. Uma verificação simples é fechar a resposta, explicar o raciocínio com suas palavras e resolver um caso diferente. Se surgir dificuldade, ela indica o que ainda precisa ser estudado; não significa que toda a ajuda foi inútil.

### 7. Pedir explicações à IA é melhor do que pedir código pronto?

É uma prática que vale experimentar. Shen e Tamkin observaram padrões de interação com envolvimento conceitual associados a melhores resultados. Esses padrões **não foram sorteados entre participantes**, portanto a associação não prova que pedir explicações, isoladamente, causou a melhora. [Fonte: Shen e Tamkin][r1]. Nossa proposta é combinar explicações com aplicação e verificação independente.

### 8. Como o iniciante pode avaliar uma resposta que ainda não sabe julgar?

Pode reduzir o problema, consultar documentação, criar exemplos de entrada e saída e pedir revisão de um professor, monitor ou colega mais experiente. Solicitar outra resposta à mesma IA pode ajudar a explorar dúvidas, mas não constitui validação independente. O objetivo é encontrar evidências sobre o comportamento do código, além da justificativa apresentada pela ferramenta.

### 9. Se os testes passaram, a compreensão está comprovada?

Os testes verificam comportamentos previstos em seus casos; não avaliam diretamente o entendimento do autor. Para investigar compreensão, podemos pedir que ele explique a solução, altere um requisito e localize um defeito. Um programa pode passar em testes insuficientes, inclusive quando o código e os testes compartilham a mesma interpretação errada do requisito.

### 10. A sensação de produtividade é uma evidência confiável?

É uma evidência sobre a experiência percebida, que deve ser comparada ao desempenho observado. Ziegler et al. associaram a aceitação de sugestões do Copilot à percepção de produtividade; isso não é um teste de domínio dos conceitos. [Fonte: Ziegler et al.][r8]. No estudo do METR, os desenvolvedores percebiam uma economia de tempo, embora o tempo medido tivesse aumentado. [Fonte: METR 2025][r6].

### 11. “A IA me ajudou a depurar” significa que aprendi a depurar?

Não necessariamente. Uma correção pode ter sido aplicada sem que a pessoa identifique a causa do problema. Na pesquisa Stack Overflow 2025, 66% dos respondentes à pergunta sobre frustrações citaram respostas quase corretas e 45% apontaram maior trabalho para depurar código gerado. São **autorrelatos**, não um experimento de aprendizagem. [Fonte: Stack Overflow][r11]. Podemos avaliar o aprendizado pedindo a explicação da falha e a correção de um defeito semelhante.

### 12. A IA pode substituir o professor ou o mentor?

As fontes reunidas não demonstram essa substituição. Uma possibilidade prática é usar a IA para obter apoio entre encontros e levar dúvidas mais específicas ao professor. O mentor também acompanha objetivos, dificuldades recorrentes e decisões no contexto do projeto. A eficácia dessa combinação precisaria ser avaliada, não presumida.

### 13. Aprender exige escrever tudo sem nenhuma ajuda?

Não é esse o critério que propomos. Documentação, exemplos e revisão de colegas também fazem parte do trabalho. Autonomia não significa memorizar todas as APIs: significa conseguir formular o problema, escolher uma abordagem, verificar a resposta e reconhecer quando precisa de ajuda. Uma atividade com assistência e outra com menos assistência podem responder a perguntas complementares sobre desempenho.

### 14. Se os modelos ficarem melhores, a preocupação com aprendizagem desaparece?

Uma ferramenta mais capaz pode executar melhor a tarefa. Isso, por si só, não informa o que o usuário aprendeu durante o processo. Para responder, seriam necessárias avaliações de competência usando as ferramentas atuais, inclusive acompanhamento posterior. A atualização do METR ilustra como mudanças no uso também dificultam medir produtividade. [Fonte: METR 2026][r7].

### 15. Qual é a ligação com Gerência de Configuração?

Podemos observar entendimento nas decisões de mudança: explicar a comparação entre versões (diff), registrar por que uma dependência foi incluída, reproduzir o ambiente, criar um teste de regressão e planejar uma reversão. A IA pode auxiliar nessas atividades; a equipe precisa conseguir interpretar seus efeitos. Essa é uma aplicação proposta para a disciplina, não uma conclusão experimental das fontes.

### 16. Qual posicionamento equilibrado podemos defender?

Podemos defender a adoção de IA acompanhada de objetivos de aprendizagem e critérios de revisão. O ganho na entrega tem valor, mas chamar alguém de “melhor desenvolvedor” exige critérios adicionais. O SPACE fundamenta a necessidade de tratar produtividade como algo que não cabe em uma única medida; não é, porém, um estudo de aprendizagem com IA. [Fonte: Forsgren et al.][r9].

## 3. Referências

- **SHEN, Judy Hanwen; TAMKIN, Alex (2026).** [*How AI Impacts Skill Formation*][r1].
- **CUI, Kevin Zheyuan et al. (2026).** [*The Effects of Generative AI on High-Skilled Work: Evidence from Three Field Experiments with Software Developers*][r5]. *Management Science*. Publicado on-line em 27 fev. 2026.
- **KAZEMITABAAR, Majeed et al. (2023).** [*Studying the effect of AI Code Generators on Supporting Novice Learners in Introductory Programming*][r12]. CHI.
- **KAZEMITABAAR, Majeed et al. (2024).** [*CodeAid: Evaluating a Classroom Deployment of an LLM-based Programming Assistant that Balances Student and Educator Needs*][r3]. CHI. PDF disponibilizado por um coautor.
- **ZIEGLER, Albert et al. (2022).** [*Productivity Assessment of Neural Code Completion*][r8]. MAPS.
- **BECKER, Joel; RUSH, Nate; BARNES, Elizabeth; REIN, David (2025).** [*Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity*][r6]. METR.
- **BECKER, Joel et al./METR (2026).** [*We are Changing our Developer Productivity Experiment Design*][r7]. 24 fev. 2026.
- **STACK OVERFLOW (2025).** [*2025 Developer Survey: AI*][r11].
- **FORSGREN, Nicole et al. (2021).** [*The SPACE of Developer Productivity: There's more to it than you think*][r9]. *ACM Queue*. Página oficial da Microsoft Research.

[r1]: https://arxiv.org/abs/2601.20245
[r3]: https://austinhenley.com/pubs/Kazemitabaar2024CHI_CodeAid.pdf
[r5]: https://pubsonline.informs.org/doi/10.1287/mnsc.2025.00535
[r6]: https://arxiv.org/abs/2507.09089
[r7]: https://metr.org/blog/2026-02-24-uplift-update/
[r8]: https://arxiv.org/abs/2205.06537
[r9]: https://www.microsoft.com/en-us/research/publication/the-space-of-developer-productivity-theres-more-to-it-than-you-think/
[r11]: https://survey.stackoverflow.co/2025/ai
[r12]: https://arxiv.org/abs/2302.07427
