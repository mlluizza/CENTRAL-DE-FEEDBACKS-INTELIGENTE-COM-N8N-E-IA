# Central de Feedbacks Inteligente: Pipeline de Análise com IA

## 📖 Sobre o Projeto
A Mercattone é um e-commerce com cerca de 200 pedidos por dia. Todo o feedback dos clientes chega à mesma caixa de entrada, o que gera um caos:
* **Bugs perdem-se:** Ficam enterrados entre elogios e não são tratados com prioridade.
* **Sugestões desaparecem:** A equipa de produto nunca chega a conhecer as boas ideias dos clientes.
* **Urgências chegam tarde:** A equipa de CX lê dezenas de e-mails por dia e, ainda assim, erra na triagem.

Para resolver isto, criámos um **Pipeline de Análise com IA** baseado em 5 LLM Chains.

## 🚀 Como Funciona
O sistema atua sozinho a cada e-mail recebido. Um e-mail entra e cinco ações saem, sem que ninguém precise de fazer nada:
1. **E-mail chega**
2. **IA analisa**
3. **Deteta urgência**
4. **Roteia no Slack**
5. **Envia resposta automática**

## 🧠 Porquê LLM Chains em vez de AI Agents?
Embora os **AI Agents** sejam ótimos para conversas abertas e chatbots (são autónomos e usam *tools*), eles também são mais caros, consomem mais *tokens* e podem ser imprevisíveis.

Para um processamento em escala, optámos pelo mundo das **LLM Chains**. São nós especializados de IA onde cada um faz uma tarefa específica sem improvisar.
* **Determinística:** Faz exatamente o que foi definido.
* **Mais barata:** Consome menos *tokens* e tem mais eficiência.
* **Mais previsível:** Entrega resultados consistentes.
* **Pipeline de dados:** Perfeita para processar grandes volumes em escala.

## ⚙️ As 5 LLM Chains (Os 5 Superpoderes)
Cada nó resolve um problema específico. Juntos, formam o pipeline de análise completo:

* **Information Extractor:** Transforma texto livre em dados estruturados (JSON).
* **Sentiment Analysis:** Deteta o sentimento do cliente (positivo, neutro ou negativo).
* **Text Classifier:** Classifica o feedback em categorias predefinidas.
* **Summarization Chain:** Resume textos longos com precisão.
* **Basic LLM Chain:** Chamada genérica com *prompt* livre para total flexibilidade.

### 📸 Demonstração do Projeto

**Envio da Mensagem Automática no Slack:**
