# # Miniguia de Estudos: Inteligência Artificial Generativa no Desenvolvimento

## 🎯 Contexto e Objetivos
O tema escolhido para este caderno temático é **Inteligência Artificial Generativa aplicada ao Desenvolvimento de Software**. 
O objetivo de estudo com este material é entender como ferramentas de IA (como LLMs e o próprio NotebookLM) podem ser integradas no dia a dia do programador para acelerar o desenvolvimento, melhorar a qualidade do código, auxiliar na resolução de problemas complexos e dominar a arte da engenharia de prompts.

## 📚 Curadoria de Fontes
As seguintes fontes foram selecionadas e feito o upload no NotebookLM para basear meus estudos:
1. [Engenharia de Prompts - Guia Oficial da OpenAI](https://platform.openai.com/docs/guides/prompt-engineering) (Texto web importado)
2. [Artigo: Práticas recomendadas para desenvolvimento com IA](https://developers.google.com/machine-learning/crash-course) (Artigo em PDF)
3. [Documentação do Google sobre IA Generativa](https://ai.google/discover/generativeai/) (Texto web importado)
4. [Repositório Awesome Prompt Engineering](https://github.com/promptslab/Awesome-Prompt-Engineering) (Texto importado em PDF)

## 🛠️ Engenharia de Prompts e "Cicatrizes"

Aqui registro meu processo de tentativa e erro ao interagir com a IA para extrair as melhores respostas.

**Teste de Prompt 1: Geração de Código Básica**
* **Prompt Inicial:** "Crie uma função em Python para calcular a sequência de Fibonacci."
* **Resposta Obtida:** A IA gerou o código corretamente usando recursão, mas sem nenhum tratamento de erros e com baixa performance para números grandes.
* **Troubleshooting (Cicatrizes):** Percebi que a IA tende a ir pelo caminho mais simples se não impormos restrições. Faltou especificar a necessidade de performance e validação de inputs.
* **Prompt Refinado:** "Atue como um desenvolvedor Sênior. Crie uma função em Python para calcular a sequência de Fibonacci de forma iterativa (para garantir performance O(n)). Inclua validação para garantir que o input seja um número inteiro positivo e adicione docstrings."

**Teste de Prompt 2: Explicação de Conceitos Complexos**
* **Prompt Inicial:** "Explique o que é RAG (Retrieval-Augmented Generation)."
* **Resposta Obtida:** A resposta foi extremamente densa, cheia de jargões acadêmicos sobre vetores e embeddings, difícil de digerir rapidamente.
* **Troubleshooting (Cicatrizes):** Não defini o público-alvo ou o nível de complexidade desejado na explicação.
* **Prompt Refinado:** "Explique o conceito de RAG (Retrieval-Augmented Generation) como se eu fosse um desenvolvedor júnior que acabou de começar a estudar IA. Use uma analogia simples, como uma pesquisa em uma biblioteca, para ilustrar o conceito."

## 📖 Miniguia de Estudo

### 📝 Resumos Estruturados
* **IA Generativa no Código:** Modelos de linguagem são excelentes "pair programmers". Eles podem auxiliar em tarefas repetitivas, escrever boilerplate, documentar código e gerar testes unitários, liberando o desenvolvedor para focar na arquitetura.
* **Engenharia de Prompts:** É a arte de formular instruções precisas. O uso de Contexto, Restrições e Exemplos (técnica de few-shot prompting) melhora drasticamente a qualidade e a utilidade das respostas da IA.
* **Limitações e Segurança:** IAs podem ter "alucinações" (inventar fatos ou bibliotecas que não existem) e gerar código com vulnerabilidades de segurança. A revisão e validação humana continuam sendo indispensáveis em 100% dos casos.

### 🧠 Glossário
* **LLM (Large Language Model):** Modelo de inteligência artificial treinado em quantidades massivas de texto para entender e gerar linguagem natural ou código.
* **Prompt:** A instrução, pergunta ou contexto fornecido à IA para iniciar uma interação.
* **Few-shot Prompting:** Técnica onde se fornece alguns exemplos de entradas e saídas esperadas junto com o prompt para guiar o comportamento da IA.
* **Alucinação:** Fenômeno onde a IA gera informações falsas, incorretas ou inexistentes com um tom de extrema confiança.
* **RAG:** Técnica que melhora a precisão da IA conectando-a a uma base de dados externa (como os seus PDFs no NotebookLM) antes dela gerar a resposta, garantindo que ela consulte fontes confiáveis.

### 💡 Prompts Reutilizáveis
Guarde estes templates para revisões futuras ou para usar no dia a dia:
1. **Para Refatoração:** "Atue como um Engenheiro de Software Sênior. Revise o código abaixo, sugira melhorias de performance e legibilidade, e aplique os princípios de Clean Code: [COLE O CÓDIGO AQUI]"
2. **Para Documentação:** "Gere a documentação em formato JSDoc/Docstring para a seguinte função, explicando o que ela faz, seus parâmetros, o que ela retorna e quais exceções pode disparar: [COLE O CÓDIGO AQUI]"
3. **Para Debugging:** "Estou recebendo o seguinte erro: '[COLE O ERRO AQUI]' ao executar este trecho de código: [COLE O CÓDIGO AQUI]. Liste as possíveis causas desse erro e me dê o passo a passo de como posso resolver cada uma delas."
