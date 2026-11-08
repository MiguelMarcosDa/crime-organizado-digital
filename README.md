# Detecção precoce de contas laranja entre jovens, com revisão humana, contestação rápida e prevenção

## Integrantes

| Nome completo (ordem alfabética) | GitHub | Área de carreira | RGM |
|---|---|---|---|
| Kayk Alberto Santana Ferreira | [@Kayksantanaf](https://github.com/Kayksantanaf) | Engenharia de Dados | [RGM] |
| Maria Clara Farias Coelho | [@mariaclarafarias1806-web](https://github.com/mariaclarafarias1806-web) | Engenharia de Dados | [RGM] |
| Miguel Marcos da Silva Gonçalves | [@GitHub do Miguel](https://github.com/) | Engenharia de Dados | [RGM] |

**Dossiê:** 2. Crime organizado no ambiente digital: aliciamento online e contas laranja.

**Recorte:** contas de pessoas de 16 a 24 anos em bancos digitais e fintechs, nas etapas de detecção precoce de contas laranja e de prevenção.

---

## 1. Análise do problema

### 1.1 O problema

O crime organizado digital recruta jovens por redes sociais, mensageiros e jogos online. Uma das formas é o aliciamento para ceder ou abrir contas bancárias ("contas laranja"), usadas para movimentar dinheiro ilícito e dificultar a identificação dos criminosos. Muitos jovens aceitam por promessa de ganho fácil, sem entender que podem responder criminalmente e ter o nome sujo.

**O que é afetado?**
- **Jovens e adolescentes:** aliciamento, manipulação, extorsão, restrição de crédito e risco de responsabilização criminal.
- **Sistema financeiro:** contas usadas para movimentar dinheiro ilícito.
- **Bancos e fintechs:** fraudes, prejuízos e risco regulatório.
- **Sociedade:** aumento da insegurança digital.

**Onde acontece?**
- Redes sociais (Instagram, Facebook, TikTok).
- Aplicativos de mensagens (WhatsApp, Telegram).
- Jogos online.
- Plataformas bancárias e transferências digitais (Pix).

**Dados e estatísticas**

| Indicador | Dado |
|---|---|
| Exploração online | 19% dos jovens de 12 a 17 anos foram vítimas de exploração e/ou abuso sexual facilitados pela tecnologia em um ano. |
| Vítimas estimadas | Aproximadamente 3 milhões de crianças e adolescentes no Brasil. |
| Denúncias na internet | 49.336 denúncias entre janeiro e julho de 2025. |
| Contas laranja | 2,6 milhões de potenciais indivíduos ou contas com indícios de atuação como laranjas em 2025. |
| Crescimento | Aumento de 62% em relação a 2023, segundo a Serasa Experian. |

> Os números acima vêm das fontes listadas abaixo; confirme o valor e a data exatos em cada página antes da entrega.

**Exemplo real: Operação Mandacaru (Polícia Federal, 2025)**
- Investigação de organização criminosa envolvendo fraudes bancárias.
- Cerca de R$ 25 milhões movimentados em operações suspeitas.
- Uso de contas digitais e de pessoas como laranjas.

**Fontes:** [UNICEF](https://www.unicef.org/) · [SaferNet Brasil](https://new.safernet.org.br/) · [Serasa Experian](https://www.serasaexperian.com.br/) · [Polícia Federal](https://www.gov.br/pf/pt-br) · [Banco Central do Brasil](https://www.bcb.gov.br/)

### 1.2 Causas

**Causas tecnológicas**

| Eixo | Causa |
|---|---|
| Sistemas | Verificação de identidade fraca na abertura de contas; poucos mecanismos para detectar comportamento suspeito logo após a abertura. |
| Dados | Vazamento de CPF, telefone e endereço; uso de dados roubados para abrir contas falsas; comércio ilegal de dados pessoais. |
| Redes e plataformas | Redes sociais e jogos usados para aliciar; mensageiros usados para organizar a atividade. |
| Decisões de projeto | Falta de monitoramento de padrões entre contas; moderação insuficiente de perfis e anúncios criminosos; canais de contestação lentos, que levam o jovem a abandonar a conta ou aceitar a situação. |

**Conclusão:** as falhas de verificação, de monitoramento e de proteção de dados facilitam o aliciamento e o uso de contas laranja. Por isso a solução combina detecção, revisão humana e prevenção.

**Fontes:** [ANPD](https://www.gov.br/anpd/pt-br) · [CERT.br](https://cartilha.cert.br/) · [Banco Central do Brasil](https://www.bcb.gov.br/) · [SaferNet Brasil](https://new.safernet.org.br/) · [UNICEF Brasil](https://www.unicef.org/brazil/)

### 1.3 O que já existe, por que não basta e o que poderia melhorar

**O que já existe**
- **Disque 100:** denúncias de violência e exploração contra crianças e adolescentes.
- **SaferNet Brasil:** denúncias anônimas de crimes digitais e orientação.
- **Polícia Federal e Comunica PF:** investigação de crimes cibernéticos e canal de comunicação.
- **Conselho Tutelar:** proteção de crianças e adolescentes.
- **Bancos e fintechs:** sistemas de monitoramento antifraude.
- **Plataformas digitais:** ferramentas de denúncia e remoção de conteúdo.

**Por que não basta**
- Muitos casos não são denunciados; o jovem muitas vezes nem sabe que está sendo usado.
- Criminosos usam perfis falsos e identidades de terceiros.
- A detecção em cada banco é isolada e a investigação envolve várias cidades.
- Os criminosos mudam de estratégia rapidamente.
- O monitoramento atual costuma agir tarde (depois do dinheiro movimentado) e raramente explica a decisão ao cliente.

**O que poderia melhorar**
- Detectar sinais logo nas primeiras semanas da conta.
- Garantir que nenhuma restrição seja definitiva sem análise humana.
- Dar ao jovem um caminho rápido e claro para contestar.
- Combinar a detecção com educação sobre aliciamento.

**Fontes:** [Disque 100](https://www.gov.br/mdh/pt-br) · [SaferNet](https://new.safernet.org.br/) · [Polícia Federal](https://www.gov.br/pf/pt-br) · [Comunica PF](https://www.gov.br/pf/pt-br/canais_atendimento/comunicacao-de-crimes) · [Banco Central](https://www.bcb.gov.br/) · [Ministério da Justiça](https://www.gov.br/mj/pt-br)

---

## 2. Proposta tecnológica

### 2.1 A solução, do ponto de vista do usuário

**O que é:** um sistema, operado por bancos digitais e fintechs, que identifica cedo contas de jovens de 16 a 24 anos com sinais de uso como conta laranja. Ele **não bloqueia ninguém automaticamente**: gera um alerta que um analista humano revisa, permite que o jovem conteste rapidamente e entrega conteúdo de prevenção sobre aliciamento.

**Para quem:**
- **Jovens de 16 a 24 anos** titulares de contas (inclusive menores de 18 com conta autorizada).
- **Analistas de fraude** dos bancos, que revisam os alertas.
- **Pais e responsáveis** de titulares menores de idade, quando aplicável.

**Como funciona, passo a passo**

1. **Abertura e uso da conta:** o jovem usa a conta normalmente (Pix, transferências, recebimentos).
2. **Monitoramento mínimo:** o sistema analisa apenas dados de comportamento da conta (volume, velocidade, padrão de entrada e saída de valores, relação entre contas), sem ler mensagens nem acessar redes sociais.
3. **Pontuação de risco:** um modelo gera uma pontuação e os motivos principais (por exemplo: "muitos Pix recebidos de origens diferentes e repassados em minutos").
4. **Revisão humana:** se a pontuação passar do limite, um analista revisa o caso em até 4 horas úteis. Sem análise humana, nenhuma restrição é aplicada.
5. **Ação proporcional:** o analista pode (a) arquivar o alerta, (b) pedir mais informações ao jovem ou (c) aplicar restrição parcial temporária (por exemplo, limite de transferências), nunca encerramento imediato.
6. **Aviso claro ao jovem:** o jovem recebe, por app, e-mail ou SMS, uma mensagem em linguagem simples com o motivo e como contestar.
7. **Contestação rápida:** o jovem contesta pelo app, site ou telefone, anexando explicação ou documento. Resposta em até 24 horas.
8. **Prevenção:** junto ao aviso, o jovem recebe conteúdo curto sobre como o aliciamento acontece e para onde denunciar (Disque 100, SaferNet, Comunica PF).
9. **Aprendizado:** o resultado de cada revisão (confirmado ou falso positivo) volta para melhorar o modelo e o limite de alerta.

### 2.2 Arquitetura

```mermaid
flowchart LR
    A["Sistemas do banco: Pix e transações"] --> B["Ingestão em streaming (Kafka)"]
    B --> C["Mascaramento e pseudonimização"]
    C --> D["Processamento (Flink)"]
    D --> E[("Feature Store")]
    E --> F["Modelo de risco"]
    F --> G["Fila de alertas"]
    G --> H["Painel do analista humano"]
    H --> I["Decisão: arquivar, pedir informação ou restrição parcial"]
    I --> J["Notificação ao jovem"]
    J --> K["Portal de contestação"]
    K --> H
    I --> L[("Banco de auditoria")]
    H --> L
    L --> M["Auditoria de viés e métricas"]
    M --> F
    J --> N["Conteúdo de prevenção"]
```

**Que dados entram, onde ficam e quem acessa**

| Dado | Origem | Onde fica | Quem acessa |
|---|---|---|---|
| Transações (valor, horário, tipo, contraparte pseudonimizada) | Sistemas do banco | Kafka e Feature Store (identificadores pseudonimizados, retenção curta) | Pipelines e modelo; sem acesso humano direto |
| Dados cadastrais mínimos (idade, tempo de conta) | Cadastro do banco | Feature Store | Pipelines e modelo |
| Pontuação e motivos do alerta | Modelo | Banco de auditoria | Analistas e auditoria |
| Decisão do analista e justificativa | Painel do analista | Banco de auditoria | Analistas, encarregado (DPO) e auditoria |
| Contestação e documentos anexados | Jovem | Banco de auditoria (criptografado) | Analista designado e DPO |

Identificadores diretos (nome, CPF, localização) ficam fora do pipeline de modelagem. A reidentificação só ocorre na tela do analista, com registro de acesso.

### 2.3 O trabalho de cada área

Os três integrantes são da área de Engenharia de Dados e atuaram em frentes distintas da cadeia de dados.

#### Ingestão e streaming (Kayk)
Projeta os pipelines de eventos transacionais (Kafka e Flink) e a Feature Store, garantindo baixa latência entre a transação e a pontuação de risco.

#### Governança, privacidade e viés (Maria Clara)
Define o mascaramento e a pseudonimização dos dados, aplica a LGPD aos pipelines (com atenção a dados de menores) e constrói a rotina de auditoria de viés do modelo.

#### Integração e operação humana (Miguel)
Integra os pipelines às APIs bancárias, constrói o painel do analista e o fluxo de contestação, e monitora o cumprimento dos prazos (SLA).

#### Como as áreas se complementam
A ingestão entrega dados rápidos, mas só pode usá-los depois do mascaramento definido pela governança. O painel do analista depende dos dois: precisa de dados atuais (ingestão) e de dados protegidos e explicáveis (governança). A contestação gera rótulos que realimentam o modelo e a auditoria de viés, fechando o ciclo.

### 2.4 O que a tecnologia não resolve

- **Não elimina o aliciamento na origem.** Ele acontece em redes sociais e jogos fora do alcance do banco; a solução só age quando o dinheiro já começa a circular.
- **Não distingue com certeza intenção.** Um jovem pode estar sendo enganado ou ser cúmplice; só a investigação define.
- **Gera falsos positivos.** Freelancers, entregadores, quem recebe ajuda familiar ou bolsa podem parecer suspeitos; por isso a revisão humana e a contestação são obrigatórias.
- **Depende de cooperação entre instituições.** Criminosos trocam de banco; sem compartilhamento regulado de sinais, cada banco vê apenas parte do quadro.
- **Não substitui educação digital, famílias, escolas e polícia.**

---

## 3. Análise ética

### 3.1 Matriz de riscos

| # | Risco | Classificação | Impacto (quem e quão grave) | Controle |
|---|---|---|---|---|
| 1 | Falso positivo: jovem legítimo tem a conta restringida | ético | Jovem de baixa renda que depende da conta para renda ou benefício; **alto** | Revisão humana obrigatória; restrição apenas parcial; contestação em até 24 h |
| 2 | Modelo discrimina por renda, região ou perfil | viés-inclusão | Jovens da periferia e de renda variável; **alto** | Auditoria de viés por grupo antes e depois da produção; variáveis proibidas (CEP, raça, gênero); limite revisado se a disparidade passar do tolerado |
| 3 | Exposição indevida de dados de menores de 18 anos | legal-privacidade | Adolescentes de 16 e 17 anos; **alto** | Pseudonimização, acesso restrito por perfil, melhor interesse do menor (LGPD art. 14), RIPD |
| 4 | Vazamento ou acesso indevido ao banco de auditoria | segurança | Todos os titulares; **alto** | Criptografia em trânsito e repouso, controle de acesso, log de consultas, testes de invasão |
| 5 | Decisão opaca: jovem não entende o motivo da restrição | governança | Jovem sem meios de se defender; **médio-alto** | Motivos em linguagem simples em cada aviso; direito de revisão (LGPD art. 20) |
| 6 | Analista aceita a sugestão do modelo sem pensar (viés de automação) | ético | Jovens com alerta mal avaliado; **médio** | Treinamento, amostras de auditoria de decisões, métrica de taxa de concordância com o modelo |
| 7 | Estigmatização: jovem rotulado como "laranja" e o rótulo circula entre instituições | ético | Jovem com histórico manchado sem prova; **alto** | Não compartilhar rótulos sem confirmação humana; prazo de expiração; base legal e regras do BCB para compartilhamento |
| 8 | Exclusão digital: jovem sem celular próprio ou com deficiência não consegue contestar | viés-inclusão | Jovens sem acesso digital pleno; **médio** | Canais alternativos (telefone, agência, atendimento assistido); requisitos de acessibilidade (seção 4) |
| 9 | Uso do sistema para fins diferentes (ex.: vigilância ou score de crédito) | governança | Todos os titulares; **médio** | Finalidade restrita em política interna e contrato; auditoria independente |

### 3.2 Decisão

**Implantar com controles.**

A solução reduz um dano real (jovens usados em crimes e prejuízos ao sistema financeiro), mas o risco de punir injustamente jovens de baixa renda e de tratar dados de menores exige salvaguardas desde o início. Por isso a recomendação é um piloto limitado, com um banco parceiro, antes de ampliar. Nenhuma restrição é aplicada sem análise humana, toda decisão é explicada e contestável em até 24 horas, e o modelo só entra em produção depois de passar no teste de viés. Se os controles abaixo não estiverem cumpridos, a decisão passa a ser "Não implantar ainda". Após seis meses de piloto, os indicadores da seção 6 decidem a expansão ou o encerramento.

### 3.3 Controles antes de entrar em produção

| Eixo | Controle | Quem faz | Como saber que foi cumprido |
|---|---|---|---|
| Transparência | Aviso em linguagem simples com motivo da restrição e como contestar; política pública descrevendo o uso do modelo | Time de produto com o DPO | Teste de leitura com jovens (compreensão ≥ 80%); política publicada |
| Revisão humana | Nenhuma restrição sem decisão de analista; treinamento e amostragem de decisões | Operações de fraude | Log mostra 100% das restrições com analista identificado; auditoria mensal |
| Minimização de dados | Só variáveis de comportamento da conta; identificadores diretos fora do pipeline; retenção curta | Governança de dados (Maria Clara) | Inventário de variáveis aprovado pelo DPO; revisão de retenção automatizada |
| Segurança | Criptografia, controle de acesso por perfil, log de acessos, teste de invasão | Segurança da informação do banco | Relatório de pentest sem falhas críticas abertas |
| Teste de viés | Comparar taxas de alerta e de falso positivo por faixa de renda, região, idade e tipo de ocupação | Governança de dados e ciência de dados | Relatório de equidade com disparidade abaixo do limite acordado, assinado antes do go-live |
| Canal de contestação | Contestação por app, web, telefone e atendimento assistido; resposta em até 24 h | Operações e produto | Painel de SLA com ≥ 95% das contestações respondidas no prazo |

### 3.4 LGPD

| Dado pessoal | Finalidade | Base legal | Por quanto tempo | Sensível ou de criança/adolescente? |
|---|---|---|---|---|
| Histórico de transações (valor, horário, tipo, contraparte pseudonimizada) | Detectar padrões de uso como conta laranja | Cumprimento de obrigação legal ou regulatória (prevenção a fraude e lavagem de dinheiro) e legítimo interesse, com RIPD | 12 meses na Feature Store; alertas confirmados conforme prazo regulatório | Não sensível; pode ser de adolescente (16 e 17 anos) |
| Dados cadastrais mínimos (idade, tempo de conta, tipo de conta) | Contextualizar o risco | Obrigação legal ou regulatória | Enquanto a conta existir; sem cópia no pipeline de modelo além do necessário | Pode ser de adolescente |
| Pontuação de risco e motivos | Apoiar a decisão do analista | Legítimo interesse, com direito de revisão (art. 20) | 12 meses | Pode ser de adolescente |
| Decisão do analista e justificativa | Auditoria e defesa do titular | Obrigação legal e exercício regular de direitos | Prazo regulatório e prescricional aplicável | Pode ser de adolescente |
| Contestação e documentos anexados | Permitir defesa do titular | Execução de procedimento a pedido do titular e exercício regular de direitos | Até 12 meses após o encerramento do caso | Pode conter dado sensível ou de adolescente; coletar o mínimo e avisar |
| Contato (e-mail, telefone) | Notificar e atender a contestação | Execução de contrato | Enquanto a conta existir | Pode ser de adolescente |

Observações:
- Para titulares menores de 18 anos, o tratamento deve atender ao **melhor interesse da criança e do adolescente** (LGPD, art. 14), com linguagem adequada à idade nas comunicações.
- Será elaborado **RIPD/DPIA** antes do piloto.
- Revisão final das bases legais por assessoria jurídica e pelo DPO do banco parceiro.

### 3.5 Comunicado público

> Propusemos um sistema para bancos digitais detectarem cedo contas laranja entre jovens de 16 a 24 anos. Nenhuma conta é restringida só por algoritmo: todo alerta passa por analista humano, e o jovem pode contestar com resposta em até 24 horas. Usamos o mínimo de dados, protegemos informações pessoais e auditamos o modelo contra discriminação. Também oferecemos orientação sobre aliciamento online. É uma proposta acadêmica, sujeita a testes e revisão jurídica. #LGPD #Fintech #Segurança

**Contagem:** 488 caracteres

---

## 4. Acessibilidade e inclusão digital

### 4.1 Quem pode ficar de fora

| Grupo | Barreira | O que a solução faz |
|---|---|---|
| Pessoas com deficiência visual | Painel e portal de contestação inacessíveis a leitores de tela | Interface compatível com leitor de tela; textos alternativos; avisos também por áudio e telefone |
| Pessoas com deficiência auditiva | Atendimento só por telefone | Atendimento por chat e texto; vídeo com legenda e Libras no conteúdo de prevenção |
| Pessoas com deficiência intelectual ou baixa escolaridade | Termos técnicos ("risco", "contestação") | Linguagem simples, frases curtas, ícones, exemplos e atendimento assistido |
| Jovens de baixa renda sem plano de dados ou celular próprio | Dependência de app e internet | Contestação por SMS, telefone e agência; app leve que funciona em rede lenta |
| Jovens em área rural ou com internet instável | Upload de documentos falha | Envio em partes, retomada automática e alternativa presencial |
| Menores de 18 anos | Dificuldade de entender o processo e de agir sozinhos | Texto adequado à idade e opção de acionar responsável quando necessário |

### 4.2 Requisitos de acessibilidade

| Requisito | Critério WCAG 2.2 |
|---|---|
| Todo conteúdo não textual (ícones, gráficos do conteúdo educativo) com alternativa em texto | 1.1.1 Conteúdo não textual (A) |
| Vídeos de prevenção com legenda e transcrição | 1.2.2 Legendas (A) |
| Contraste de texto de ao menos 4,5:1 | 1.4.3 Contraste mínimo (AA) |
| Texto ampliável em 200% sem perda de função | 1.4.4 Redimensionar texto (AA) |
| Todo o fluxo de contestação operável só por teclado | 2.1.1 Teclado (A) |
| Tempo suficiente para preencher e enviar a contestação, com possibilidade de estender | 2.2.1 Ajuste de tempo (A) |
| Alvos de toque de ao menos 24×24 px | 2.5.8 Tamanho do alvo, mínimo (AA) |
| Erros de formulário identificados em texto e com sugestão de correção | 3.3.1 Identificação de erro (A) e 3.3.3 Sugestão de erro (AA) |
| Login e verificação sem exigir teste cognitivo (colar senha permitido; alternativa a CAPTCHA) | 3.3.8 Autenticação acessível, mínimo (AA) |
| Rótulos e instruções claros nos campos | 3.3.2 Rótulos ou instruções (A) |

Validação planejada: auditoria com leitor de tela (NVDA e TalkBack) e teste de uso com pelo menos 5 pessoas com deficiência antes do piloto.

---

## 5. Sustentabilidade

### 5.1 Impacto ambiental da solução

- **Consumo de processamento:** streaming contínuo e retreino do modelo usam energia. Mitigação: modelo leve (árvores de decisão em vez de redes profundas), retreino periódico em vez de contínuo, e escolha de região de nuvem com maior participação de energia renovável.
- **Armazenamento:** retenção curta (12 meses) e agregação reduzem volume e energia.
- **Dispositivos:** app leve evita obrigar os jovens a trocar de celular.
- **Medição:** acompanhar consumo estimado (kWh e CO₂e) por milhão de transações processadas e incluir no relatório anual.

### 5.2 Sustentabilidade do projeto

- **Quem mantém:** equipe de engenharia de dados e de fraude do banco parceiro, com o DPO responsável pela governança.
- **Quem paga:** o banco ou fintech contratante, pois o custo é compensado pela redução de perdas por fraude e de risco regulatório; o jovem não paga por nada.
- **Depois do primeiro ano:** o modelo é reavaliado a cada trimestre (golpes mudam rápido); a auditoria de viés é repetida a cada retreino; se os indicadores não forem atingidos, o projeto é revisado ou encerrado. O conteúdo de prevenção é atualizado com parceiros como a SaferNet.

---

## 6. Impacto esperado

### 6.1 Indicadores

| Indicador | Como medir | Meta | Prazo |
|---|---|---|---|
| Detecção precoce | % de contas laranja confirmadas detectadas nos primeiros 30 dias de atividade suspeita | ≥ 60% | 12 meses de piloto |
| Precisão dos alertas | % de alertas revisados que se confirmam | ≥ 40% | 6 meses |
| Falsos positivos restritos | % de contas restringidas e depois liberadas após contestação | ≤ 5% das restrições | 12 meses |
| Tempo de revisão humana | Mediana do tempo entre alerta e decisão do analista | ≤ 4 horas úteis | 3 meses |
| Tempo de resposta à contestação | % respondidas em até 24 horas | ≥ 95% | 6 meses |
| Equidade | Razão entre a taxa de falso positivo do grupo mais afetado e a do grupo menos afetado | ≤ 1,25 | Antes do go-live e a cada trimestre |
| Prevenção | % de jovens que abriram o conteúdo de prevenção após um aviso | ≥ 50% | 6 meses |
| Compreensão do aviso | % de jovens que entendem o motivo e o próximo passo (pesquisa curta) | ≥ 80% | 6 meses |

### 6.2 Como os usuários serão ouvidos

- Pesquisa de uma pergunta ao final de cada contestação ("Você entendeu o motivo? Foi fácil contestar?").
- Grupos de escuta trimestrais com jovens de 16 a 24 anos, com representação de renda, região e pessoas com deficiência.
- Canal para sugestões e reclamações, com resposta pública resumida.
- Parceria com organizações como a SaferNet para revisar o conteúdo de prevenção.
- Resultados da escuta alimentam o backlog e são reportados ao comitê de governança.

### 6.3 Se a solução não pegar

- **Poucos alertas úteis (precisão abaixo da meta):** revisar variáveis e limites; se persistir, reduzir o escopo para sinais mais simples e regras.
- **Muitos falsos positivos ou disparidade de viés:** suspender as restrições, manter só o monitoramento e voltar à fase de ajuste.
- **Jovens não leem os avisos ou não contestam:** testar novos formatos e canais com os próprios jovens.
- **Banco parceiro sem interesse após o piloto:** publicar a documentação e o aprendizado como material aberto e encerrar o projeto de forma controlada, apagando os dados conforme a política de retenção.

---

## 7. Quadro de decisões

| Decisão | Alternativas consideradas | Por que escolhemos esta |
|---|---|---|
| Revisão humana obrigatória antes de qualquer restrição | Bloqueio automático por pontuação | Reduz o dano de falsos positivos em jovens de baixa renda; o custo de analistas é menor que o dano de punir inocentes |
| Restrição parcial e temporária em vez de encerramento | Encerramento da conta; só alerta sem ação | Proporcional ao risco: contém o dano financeiro sem tirar o acesso ao dinheiro de quem é legítimo |
| Processamento em streaming (Kafka e Flink) | Processamento em lote diário | Contas laranja repassam dinheiro em minutos; o lote detectaria tarde demais |
| Modelo simples e explicável (árvores de decisão com motivos) | Rede neural profunda | Precisamos explicar o motivo ao jovem e ao analista; ganho de acurácia da rede não compensa a perda de transparência |
| Não usar CEP, raça, gênero nem dados de redes sociais | Usar mais variáveis para melhorar acurácia | Minimização de dados e redução do risco de discriminação e de vigilância |
| Contestação em até 24 horas por vários canais | Só app; prazo de 5 dias úteis | Jovem sem acesso ao dinheiro precisa de resposta rápida; canais variados evitam exclusão |
| Piloto com um banco parceiro antes de expandir | Lançamento amplo | Permite medir viés e falsos positivos em escala controlada |
| Incluir educação sobre aliciamento junto ao aviso | Só detecção e restrição | Ataca a causa (o jovem não entende o risco) e não só o sintoma |

---

## 8. Capítulos individuais

### 8.1 Kayk Alberto Santana Ferreira — Engenharia de Dados

**Papel no projeto:** responsável pelo desenho da arquitetura de ingestão de dados transacionais em tempo real (Apache Kafka e Apache Flink) e pela Feature Store, garantindo fluxo contínuo e baixa latência até o modelo de risco.

**Plano de desenvolvimento**

| Competência que a solução exige | Técnica ou comportamental | Já tenho? |
|---|---|---|
| Ingestão e streaming de dados com Apache Kafka | Técnica | Sim |
| Processamento de streams com Apache Flink | Técnica | Parcial |
| Construção e gestão de Feature Stores (Feast e Redis) para ML | Técnica | Não |
| Otimização e monitoramento de latência e concorrência | Técnica | Parcial |
| Trabalho colaborativo com equipes de segurança e ML | Comportamental | Sim |

**Metas SMART (6 a 12 meses)**
1. **Curto prazo (6 meses):** montar um ambiente de testes em contêineres (Docker Compose) com Kafka e Flink que processe 1.000 eventos transacionais simulados por segundo com latência p95 abaixo de 100 ms, registrando os resultados em relatório de teste, até **30/04/2027**.
2. **Longo prazo (12 meses):** concluir um curso de arquitetura orientada a eventos e streaming (mínimo de 20 horas, com certificado) e publicar no repositório a especificação técnica de uma Feature Store (Feast e Redis) com ao menos 10 variáveis do projeto, até **31/10/2027**.

**Feedback dos colegas**
O Kayk estruturou o pipeline de streaming do projeto e traduziu requisitos de infraestrutura em fluxos claros, o que foi essencial para a proposta de detecção em tempo real. Como ponto de evolução, sugerimos que organize sessões curtas para compartilhar a configuração dos contêineres e dos scripts de ingestão, aumentando a autonomia do restante da equipe.

### 8.2 Maria Clara Farias Coelho — Engenharia de Dados

**Papel no projeto:** responsável por governança de dados, privacidade (LGPD) e auditoria de viés. Define o mascaramento e a pseudonimização de dados (inclusive de menores de 18 anos) e a rotina de teste de equidade do modelo antifraude.

**Plano de desenvolvimento**

| Competência que a solução exige | Técnica ou comportamental | Já tenho? |
|---|---|---|
| Governança de dados e aplicação prática da LGPD em pipelines | Técnica | Sim |
| Mascaramento, pseudonimização e criptografia de dados em trânsito e em repouso | Técnica | Parcial |
| Auditoria de viés e métricas de equidade em conjuntos de dados | Técnica | Não |
| Elaboração de RIPD/DPIA | Técnica | Parcial |
| Pensamento crítico sobre o impacto ético da tecnologia em grupos vulneráveis | Comportamental | Sim |

**Metas SMART (6 a 12 meses)**
1. **Curto prazo (6 meses):** desenvolver um script em Python com Microsoft Presidio (usando Faker apenas para gerar dados de teste) que mascare ou pseudonimize CPF, nome e localização em mensagens de um tópico Kafka de teste, com taxa de detecção de pelo menos 95% em uma amostra de 1.000 registros sintéticos, até **30/04/2027**.
2. **Longo prazo (12 meses):** concluir um curso de proteção de dados e privacidade (mínimo de 20 horas, com certificado) e entregar o RIPD completo da arquitetura de streaming, junto com um relatório de auditoria de viés com ao menos 3 métricas de equidade, até **31/10/2027**.

**Feedback dos colegas**
A Maria Clara garantiu que a proposta fosse funcional e também alinhada à LGPD, com atenção à proteção dos dados dos jovens e ao risco de discriminação. Para seu desenvolvimento, recomendamos aprofundar a prática de implementação de criptografia dentro dos pipelines de dados.

### 8.3 Miguel Marcos da Silva Gonçalves — Engenharia de Dados

**Papel no projeto:** responsável pela integração dos pipelines com as APIs bancárias, pelo painel em tempo real do analista humano e pelo fluxo de contestação, incluindo o monitoramento dos prazos de resposta (SLA).

**Plano de desenvolvimento**

| Competência que a solução exige | Técnica ou comportamental | Já tenho? |
|---|---|---|
| Construção e consumo de APIs RESTful e conectores de dados | Técnica | Sim |
| Dashboards em tempo real (Grafana) | Técnica | Parcial |
| Modelagem de bancos relacionais e NoSQL para auditoria | Técnica | Sim |
| Observabilidade de dados e métricas (Prometheus) | Técnica | Não |
| Comunicação técnica entre Engenharia e Operações | Comportamental | Sim |

**Metas SMART (6 a 12 meses)**
1. **Curto prazo (6 meses):** desenvolver e documentar (OpenAPI) 4 endpoints REST do fluxo de contestação (consulta de alerta, abertura de contestação, atualização de status e trilha de auditoria), com testes automatizados cobrindo ao menos 80% do código, até **30/04/2027**.
2. **Longo prazo (12 meses):** concluir um curso de Prometheus e Grafana (mínimo de 15 horas) e montar um painel com 3 métricas de SLA (tempo de revisão do alerta, tempo de resposta à contestação e fila de alertas pendentes), com alertas automáticos quando o prazo for ultrapassado, até **31/10/2027**.

**Feedback dos colegas**
O Miguel conectou a infraestrutura de dados à interface de análise humana, com pontualidade, organização e visão orientada à solução, o que facilitou a integração dos serviços. Para seus próximos passos, recomendamos aprofundar observabilidade de dados, de modo a antecipar gargalos de rede ou perda de eventos nos pipelines antes que afetem o usuário final.

---

## 9. Referências

- BANCO CENTRAL DO BRASIL. *Portal institucional (regulamentação de prevenção a fraudes e à lavagem de dinheiro)*. Disponível em: https://www.bcb.gov.br/. Acesso em: nov. 2026.
- BRASIL. *Lei nº 13.709, de 14 de agosto de 2018 (Lei Geral de Proteção de Dados Pessoais, LGPD)*. Disponível em: https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm. Acesso em: nov. 2026.
- ANPD. *Autoridade Nacional de Proteção de Dados*. Disponível em: https://www.gov.br/anpd/pt-br. Acesso em: nov. 2026.
- CERT.br. *Cartilha de Segurança para Internet*. Disponível em: https://cartilha.cert.br/. Acesso em: nov. 2026.
- POLÍCIA FEDERAL. *Portal institucional e Comunica PF*. Disponível em: https://www.gov.br/pf/pt-br. Acesso em: nov. 2026.
- SAFERNET BRASIL. *Portal institucional e canal de denúncias*. Disponível em: https://new.safernet.org.br/. Acesso em: nov. 2026.
- SERASA EXPERIAN. *Dados sobre contas laranja e fraudes (2025)*. Disponível em: https://www.serasaexperian.com.br/. Acesso em: nov. 2026.
- UNICEF BRASIL. *Proteção de crianças e adolescentes no ambiente digital*. Disponível em: https://www.unicef.org/brazil/. Acesso em: nov. 2026.
- MINISTÉRIO DOS DIREITOS HUMANOS E DA CIDADANIA. *Disque 100*. Disponível em: https://www.gov.br/mdh/pt-br. Acesso em: nov. 2026.
- W3C. *Web Content Accessibility Guidelines (WCAG) 2.2*. Disponível em: https://www.w3.org/TR/WCAG22/. Acesso em: nov. 2026.




