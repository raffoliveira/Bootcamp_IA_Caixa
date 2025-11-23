# PRD – Assistente de Organização de Finanças Pessoais (Conversacional)

## 1. Visão Geral

Criar um aplicativo de organização de finanças pessoais que funcione por meio de conversas com o usuário.  
A proposta é substituir formulários e planilhas complexas por uma experiência de chat em linguagem natural, onde o usuário registra gastos, acompanha metas e recebe orientações de forma simples e acessível.

## 2. Problema

Hoje, muitas pessoas desistem de controlar seus gastos porque:

- Os apps de finanças exigem muita entrada manual (categorizar tudo, preencher muitos campos).
- A experiência é pouco personalizada e focada em telas complexas, cheias de gráficos e opções.
- Falta orientação prática sobre como economizar e criar hábitos financeiros saudáveis.

Consequência: o usuário até instala o app, mas abandona o uso em poucos dias.

## 3. Objetivo do Produto (MVP)

Entregar um assistente financeiro conversacional que:

- Permita registrar e organizar gastos principalmente via chat em linguagem natural.
- Ofereça uma visão simples da situação financeira (resumo de gastos, categorias principais, metas).
- Envie recomendações básicas de economia, em tom educativo e amigável.
- Seja fácil de começar a usar, sem necessidade de configuração complexa.

## 4. Público-Alvo

- Pessoas que querem começar a organizar suas finanças pessoais de forma prática e sem complicação.
- Principalmente iniciantes em controle financeiro, que não têm hábito de usar planilhas ou apps avançados.
- Faixa etária estimada: 18 a 40 anos, com uso diário de smartphone e familiaridade com aplicativos de mensagens.

## 5. Proposta de Valor

- Controle financeiro “falando” com um assistente, em vez de preencher planilhas.
- Menos fricção: bastam mensagens simples como “gastei 35 reais no mercado hoje”.
- Organização automática: o app classifica e resume os gastos para o usuário.
- Orientação prática: o “Agente Financeiro” ajuda com dicas de economia e metas simples.

## 6. Escopo do MVP

### 6.1 Funcionalidades-Chave

1. Registro de gastos via chat
   - O usuário informa o gasto em linguagem natural (ex.: “hoje gastei 50 reais com delivery”).
   - O sistema extrai valor, data (assumir hoje se não informado) e categoria sugerida.

2. Classificação automática de transações
   - Algoritmo simples de categorização (ex.: alimentação, transporte, lazer, contas fixas).
   - Possibilidade de o usuário corrigir a categoria no chat (“isso não é lazer, é alimentação”).

3. Definição e acompanhamento de metas financeiras
   - Metas simples por categoria (ex.: “quero gastar no máximo 500 reais com alimentação este mês”).
   - Resumo do progresso na meta (quanto já foi gasto, quanto ainda resta).

4. Dicas de economia do “Agente Financeiro”
   - Mensagens educativas baseadas no comportamento de gastos (sem necessidade de ser altamente personalizada no MVP).
   - Exemplos:
     - “Você já gastou 70% da sua meta de alimentação neste mês.”
     - “Percebi muitos gastos com delivery; que tal definir um limite semanal?”

5. Visualização de relatórios simples
   - Resumo mensal em formato de texto e, se possível, gráficos simples:
     - Total gasto no período.
     - Gastos por categoria.
     - Progresso das metas.
   - Foco em visualização clara e direta, sem telas complexas.

### 6.2 Fluxos Principais do Usuário (MVP)

1. Onboarding básico
   - Usuário informa nome e, opcionalmente, renda aproximada e objetivo (ex.: “quero economizar para montar uma reserva”).
   - Apresentação breve do funcionamento do chat e das principais funções.

2. Registro de gasto
   - Usuário envia mensagem com gasto.
   - Sistema interpreta, confirma o registro e mostra categoria e saldo aproximado da meta relevante.

3. Criação de meta
   - Usuário define meta por categoria ou geral (ex.: “meta de 1000 reais para todos os gastos no mês”).
   - Sistema registra e passa a acompanhar automaticamente.

4. Consulta de situação financeira
   - Usuário pode perguntar: “como estão meus gastos este mês?” ou “quanto já gastei com alimentação?”.
   - Sistema responde com resumo textual e, se houver, gráficos simples.

## 7. Requisitos Funcionais

1. Chat em linguagem natural
   - Interface com histórico de mensagens.
   - Suporte a português do Brasil.
   - Reconhecimento de:
     - Valores monetários.
     - Categorias básicas.
     - Datas simples (hoje, ontem, este mês).

2. Persistência dos dados
   - Armazenar transações (valor, data, categoria, descrição).
   - Armazenar metas e progresso.
   - Associar tudo ao usuário autenticado (MVP pode usar login simples ou até um único usuário de teste).

3. Motor de categorização
   - Regras simples baseadas em palavras-chave (ex.: “mercado”, “supermercado” → alimentação).
   - Permitir correção pelo usuário e atualizar o registro.

4. Relatórios básicos
   - Endpoint ou lógica para sumarizar:
     - Total por período.
     - Total por categoria.
     - Comparação com metas.

5. Configuração de metas
   - Criar, listar e editar metas (pelo menos ajuste de valor e categoria).
   - Notificações/resumos no chat quando o usuário estiver se aproximando ou ultrapassando a meta.

## 8. Requisitos Não Funcionais

- Linguagem: português, tom acessível e educativo.
- Usabilidade: experiência focada em poucos cliques, guiada por conversa.
- Desempenho: respostas rápidas na interação via chat.
- Privacidade: dados financeiros devem ser tratados de forma confidencial (mesmo que em ambiente de teste).

## 9. Personalidade do “Agente Financeiro”

- Tom educativo, claro e amigável.
- Evitar jargão financeiro complexo.
- Focar em orientação simples:
  - Explicar termos quando necessário (ex.: “meta”, “categoria”, “reserva financeira”).
- Não fazer julgamentos morais sobre os gastos do usuário; apenas orientar.

## 10. Métricas de Sucesso (MVP)

- Engajamento básico:
  - Número de registros de gastos por usuário em uma semana.
  - Número de interações de consulta (“quanto gastei?”, “como está minha meta?”).
- Retenção inicial:
  - Usuário voltar a usar o app pelo menos 3 vezes na primeira semana.
- Usabilidade:
  - Usuário conseguir registrar um gasto sem precisar de instruções técnicas.

## 11. Fora de Escopo (MVP)

- Conexão automática com contas bancárias ou cartões.
- Planejamento financeiro avançado (investimentos, dívidas complexas).
- Regras sofisticadas de machine learning para categorização (pode ser evoluído depois).
- Exportação em planilha ou integração com outros sistemas.

## 12. Entregável Esperado da IA (Lovable)

A partir deste PRD, a IA deve:

1. Gerar um plano de MVP com:
   - Lista das principais telas ou seções (ex.: tela de chat, tela de resumo, tela de metas).
   - Recursos técnicos necessários (modelos de dados, endpoints básicos, componentes principais).
2. Produzir um esboço de fluxo de validação inicial:
   - Como testar o registro de gastos.
   - Como testar a criação e acompanhamento de metas.
   - Como validar a clareza das mensagens do “Agente Financeiro”.
3. Manter todo o texto gerado em português e com linguagem acessível e educativa.
