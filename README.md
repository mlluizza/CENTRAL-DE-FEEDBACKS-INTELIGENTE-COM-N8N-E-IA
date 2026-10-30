# Pipeline de Análise com IA: Central de Feedbacks Inteligente

### 1️⃣ Descrição do Projeto
Este projeto foi desenvolvido para a Mercattone, um e-commerce com cerca de 200 pedidos diários, com o objetivo de organizar o caos na caixa de entrada de atendimento. O fluxo utiliza um pipeline de análise baseado em nós especializados de IA (LLM Chains) que recebe o e-mail, analisa o conteúdo, deteta urgências, roteia a mensagem para o Slack e gera uma resposta automática.

### 2️⃣ Objetivo
Automatizar a triagem de mensagens de clientes para garantir que bugs não se percam, que sugestões valiosas cheguem à equipe de produto e que urgências sejam tratadas a tempo. O foco é substituir a triagem manual demorada e sujeita a erros por um processo escalável, eficiente e determinístico.

### 3️⃣ Funcionalidades
- Processamento autônomo disparado a cada novo e-mail recebido.
- Classificação de textos em categorias predefinidas utilizando o *Text Classifier*.
- Extração de texto livre para dados estruturados (formato JSON) através do *Information Extractor*.
- Deteção do tom da mensagem (positivo, neutro ou negativo) com o nó de *Sentiment Analysis*.
- Criação de resumos precisos de mensagens longas com a *Summarization Chain*.
- Roteamento inteligente de alertas críticos para a equipa diretamente no Slack.
- Envio de respostas automáticas iniciais para os clientes.

### 4️⃣ Informações analisadas
- O nível de urgência do feedback recebido.
- Relatos de bugs que antes ficavam perdidos no meio de elogios.
- Sugestões de melhorias invisíveis para a equipe de produto.
- O sentimento geral do cliente em relação ao e-commerce.

### 5️⃣ Tecnologias utilizadas
- n8n (Múltiplos nós de LLM Chains baseados em previsibilidade)
- Slack (Para recebimento de roteamentos e notificações)
- Google Sheets (Planilha para registo estruturado dos dados)
- E-mail (Entrada de dados)

### 6️⃣ Benefícios da automação
- Operação mais barata, consumindo menos tokens e com maior eficiência do que um *AI Agent* tradicional.
- Resultados consistentes e previsíveis que não dependem da "improvisação" da IA a cada execução.
- Fim do atraso na identificação de urgências, que antes ocorria porque a equipa de CX precisava de ler dezenas de mensagens manualmente por dia.
- Geração de um pipeline robusto perfeitamente adequado para processamento de dados em larga escala.

### 📸 Demonstração do Projeto

**Envio da Mensagem Automática no Slack:**
<br><br>
<img width="1378" height="202" alt="Image" src="https://github.com/user-attachments/assets/adb6ac6a-a307-4ab1-9867-1b725ce74cac" />
<br><br>
<img width="1377" height="201" alt="Image" src="https://github.com/user-attachments/assets/402e82fb-2cfc-4738-8639-fdf2c89fb1f7" />
<br><br>
<img width="1390" height="157" alt="Image" src="https://github.com/user-attachments/assets/0df14f8d-60b6-4ad0-b90c-8ce615d3bea2" />
<br><br>

**Envio da Mensagem Automática no E-mail:**
<br><br>
<img width="1127" height="274" alt="Image" src="https://github.com/user-attachments/assets/f3fa3082-6be6-413b-92f3-7aedaa674b10" />
<br><br>
<img width="1597" height="665" alt="Image" src="https://github.com/user-attachments/assets/76c04361-5334-42fe-99ca-cdd0705b7c8d" />
<br><br>

**Fluxo construído no n8n:**
<br><br>
<img width="1535" height="514" alt="Image" src="https://github.com/user-attachments/assets/a270b50c-02d1-42a0-9165-92d78b3ce400" />
<br><br>

**📊 Extração de Dados e Registo Estruturado (Google Sheets):**
<br><br>
<img width="1857" height="222" alt="Image" src="https://github.com/user-attachments/assets/cfcf1f77-aa4e-4cfa-86ad-c44332b612d1" />
**Fluxo construído no n8n:**
<br>
<img width="1535" height="514" alt="Image" src="https://github.com/user-attachments/assets/a270b50c-02d1-42a0-9165-92d78b3ce400" />

