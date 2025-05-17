# ImersaoIA_InMathMate
![Logo InMathMate](https://github.com/user-attachments/assets/8fa02f4d-b3b1-4fed-976d-6fe26b738e04)


# 📚 InMathMate: Seu Amigo de Matemática Acessível e Empático com IA! 🚀

## ✨ InMathMate: Transformando Desafios em Vitórias para Cada Criança ✨

Imagine um mundo onde a matemática não é um bicho-papão, mas um playground divertido e acessível para todas as crianças. Para muitos alunos do 6º ano do Ensino Fundamental, a realidade é outra: a frustração com números e conceitos complexos pode levar à desmotivação e impactar toda a jornada escolar. Pense na realidade de **21 de 28 alunos com notas abaixo de 7** em uma única prova, este é um fato real – um sinal claro de que o método tradicional nem sempre alcança a todos. E para crianças com necessidades especiais de aprendizado, as barreiras são ainda maiores, tornando o acesso a um reforço de qualidade quase inexistente.

![03 - InMath](https://github.com/user-attachments/assets/5cb5a9c5-76df-4d20-899f-b948ee23c726)


O **InMathMate** nasceu dessa urgência. Somos uma plataforma inovadora, impulsionada por **Inteligência Artificial**, que atua como um tutor de matemática completo, personalizado e, acima de tudo, humano. Nosso projeto vai além do reforço escolar comum; ele é uma resposta direta à necessidade de **inclusão e apoio emocional** no aprendizado.

### **Por Que o InMathMate é Essencial e Único?**

Em um mercado saturado de ferramentas educacionais, o InMathMate se destaca por seus diferenciais inegáveis, que são o coração da nossa solução:

1. **Tutoria Multimodal Hiper-Acessível: Aprendizado 100% Adaptado e Sem Barreiras.**
    - Não oferecemos apenas "acessibilidade"; nós a **integramos ativamente no processo de aprendizado**. Nossa IA avançada se molda ao **estilo ÚNICO de cada criança**. Seja através de explicações em **texto simplificado** para dislexia, **analogias visuais ricas com sugestões de imagem** para aprendizes visuais, ou **linguagem otimizada para ser lida em voz alta** para quem prefere áudio, o InMathMate garante que a criança aprenda da forma que melhor absorve. Rompemos barreiras para que a matemática seja "vista" e "compreendida" por todos, celebrando a diversidade no aprendizado.
2. **Apoio Emocional e Psicopedagógico Contínuo: Mais Que um Tutor, Um Guia para a Confiança.**
    - Damos adeus à rigidez da correção! Nosso agente de IA é um **verdadeiro orientador de aprendizado, paciente e empático**. Ele é treinado para **NUNCA criticar ou invalidar o erro**, mas sim para transformá-lo em uma oportunidade de brilho. Com feedback positivo e construtivo, que celebra cada tentativa e esforço, o InMathMate **cultiva a autoconfiança** da criança. Aqui, errar faz parte de brilhar, e a matemática se torna uma jornada de descobertas, não de medos.

**O InMathMate não é apenas um software; é um amigo que entende, apoia e capacita, garantindo que cada criança encontre seu próprio caminho para o sucesso na matemática.**

**Visite a Página do InMathMate para uma melhor experiência de compreensão das suas soluções:** [Acesse InMathMate.io](https://jaleenpe.manus.space/)

---

## 💡 **Como o InMathMate Funciona: A Orquestra Inteligente de Agentes**

Nosso serviço é impulsionado por um sistema de quatro agentes de Inteligência Artificial, cada um com uma especialidade, trabalhando em conjunto para oferecer uma experiência de tutoria completa e fluida:

- **Agente 1: Analisador de Dificuldades (O Detetive Curioso)**
    - **Função:** O ponto de entrada do sistema. Utiliza a capacidade de **processamento de linguagem natural (NLP)** e **raciocínio lógico** do Gemini para interpretar a dificuldade do aluno e suas preferências de acessibilidade.
    - **Como atua:** Formula perguntas diagnósticas estratégicas e estrutura a saída em um **JSON validado**, contendo o diagnóstico específico e a preferência de aprendizado, essencial para a comunicação inter-agentes. Também pode realizar **grounding (busca na web via `Google Search` no prompt)** para contextualizar o currículo.
    - **Saída:** JSON com `diagnostico_dificuldade_especifica`, `preferencia_aprendizado_confirmada`, `necessita_interacao_adicional`, etc.
- **Agente 2: Explicador Criativo (O Professor Brilhante)**
    - **Função:** Aproveita a **capacidade generativa avançada do Gemini** para transformar conceitos matemáticos complexos em explicações multimodais e personalizadas.
    - **Como atua:** Decompõe o conceito em passos didáticos, utilizando analogias adaptadas e gerando **descrições de imagem (prompts textuais para Image Generation)** para aprendizes visuais, tudo estruturado em JSON para o fluxo posterior.
    - **Saída:** JSON com `explicacao_texto`, `sugestao_imagem_prompt` e `mensagem_transicao_desafios`.
- **Agente 3: Gerador de Desafios (O Mestre dos Desafios Matemáticos)**
    - **Função:** Emprega a **proficiência matemática e a criatividade textual do Gemini** para criar exercícios práticos e personalizados.
    - **Como atua:** Gera enunciados com linguagem e estrutura adaptadas à acessibilidade, variando entre cálculo direto e problemas contextualizados, sempre retornando um JSON claro com os desafios.
    - **Saída:** JSON com `titulo_desafios`, `instrucao_geral` e uma lista de `exercicios` (com `id`, `enunciado`, `formato_sugerido_resposta`).
- **Agente 4: Corretor e Motivador (O Coach Inclusivo)**
    - **Função:** Beneficia-se da **capacidade analítica e de síntese do Gemini** para comparar respostas, realizar cálculos complexos e gerar feedback psicopedagógico.
    - **Como atua:** Fornece correção detalhada (passo a passo), sempre com um **foco inabalável na motivação e empatia**, transformando o erro em aprendizado. Sua saída em JSON inclui `solucao_calculada` e `sugestao_pedagogica_proximo_passo`.
    - **Saída:** JSON com `titulo_feedback`, `feedbacks_individuais`, `mensagem_final_motivacional` e `sugestao_pedagogica_proximo_passo`.

---

## 🛠️ **Tecnologias Fundamentais**

O InMathMate é construído sobre tecnologias de ponta para garantir inteligência, escalabilidade e uma experiência de usuário rica:

- **Google Gemini API:** A inteligência central que potencializa a capacidade de compreensão, geração de texto e raciocínio lógico dos nossos agentes. É o cérebro que permite a personalização e empatia.
- **Google ADK (Agent Development Kit):** O framework que orquestra a comunicação e o fluxo inteligente entre os diversos agentes, permitindo a construção de um sistema complexo e modular.
- **Python:** A linguagem de programação robusta e flexível que serve como base para todo o desenvolvimento do serviço.
- **Google Colab:** Ambiente de desenvolvimento interativo utilizado para prototipagem e demonstração do código, facilitando o acesso e teste do projeto.
- **Capacidade de Grounding (Google Search):** Integrada aos modelos Gemini via `system_instruction` (instrução textual no prompt), permite que agentes como o Analisador busquem informações atualizadas sobre currículos matemáticos ou exemplos para enriquecer o diagnóstico e as explicações.
- **Geração de Imagens (Via Sugestão de Prompt):** O Agente 2 gera prompts de imagem que podem ser usados em ferramentas como Google AI Studio, permitindo a criação de recursos visuais personalizados para cada explicação – um forte diferencial de acessibilidade.

---

## 🚀 **Como Executar o InMathMate (Passo a Passo para Desenvolvedores)**

Para testar o **InMathMate** e ver a mágica acontecer em seu ambiente Google Colab, siga estes passos cuidadosamente:

1. **Obtenha sua API Key do Google Gemini:**
    - Acesse o [Google AI Studio](https://aistudio.google.com/app/apikey).
    - Crie ou copie sua API Key.
    - No Google Colab, clique no ícone de "chave" (Secrets) no menu lateral esquerdo.
    - Crie um novo "Secret" com o nome `GOOGLE_API_KEY_1` e cole sua API Key lá.
2. **Abra o Notebook no Google Colab:**
    - Clique neste link: [Projeto InMathMate 3.0.ipynb](https://github.com/acamilasarmento/ImersaoIA_InMathMate/blob/main/Projeto_InMathMate_3_0.ipynb)
    - Vá em `Ambiente de execução` (Runtime) -> `Reiniciar ambiente de execução` (Restart runtime) para garantir um ambiente limpo.
3. **Execute as Células em Ordem:**
    - **Célula 1 (Instalação das Dependências):** Execute a primeira célula do notebook. Ela irá instalar as bibliotecas necessárias.
    - **Célula 2 (Configuração da API Key e Importações Principais):** Execute a segunda célula para carregar sua API Key e configurar a biblioteca Gemini.
    - **Célula 3 (Imports do ADK e Funções Auxiliares):** Execute a terceira célula para importar as classes do ADK e definir as funções `call_agent` e `to_markdown`.
    - **Definição dos Agentes (Células 4, 5, 6 e 7):** Execute **cada uma das células 4, 5, 6 e 7** individualmente. Elas definem os quatro agentes do InMathMate.
    - **Inicie a Interação com o InMathMate (Célula 8):** Execute a última célula (Célula 8). O programa irá começar a interagir com você no console do Colab, pedindo o tópico de matemática e sua preferência de aprendizado.

---

## 📺 **Demonstração do InMathMate **

- Vídeo Demonstrativo: (https://www.loom.com/share/53efb207aa5f48b1b64c25139399fd3a?sid=c33d129b-77ac-4b51-9ef6-e027428a1538)

---

## 🤝 **Contribuições e Feedback**

Sua opinião é muito importante para nós! Se tiver sugestões, ideias para melhorias ou encontrar algum problema, sinta-se à vontade para abrir uma *issue* (um problema) neste repositório ou enviar um *pull request* (sugestão de código).

---

## 📝 **Licença**

Este projeto está sob a [Licença MIT](https://github.com/acamilasarmento/ImersaoIA_InMathMate/blob/main/LICENSE)

---

## 🏆 **Para a Imersão IA Alura + Google Gemini**

O **InMathMate** foi desenvolvido para o desafio da Imersão IA da Alura com o Google Gemini, e ele se alinha de forma excepcional com todos os critérios de avaliação:

- **Utilidade:** Resolve um problema real e urgente na educação do Ensino Fundamental, auxiliando crianças com dificuldades em matemática e promovendo a inclusão de forma ativa.
- **Criatividade:** Aplica a Inteligência Artificial de forma inovadora para criar um **tutor personalizado, multimodal e empático**, representando um diferencial significativo e disruptivo no mercado educacional.
- **Eficácia:** O sistema de agentes funciona de ponta a ponta, gerando diagnósticos precisos, explicações claras, exercícios relevantes e feedback construtivo, adaptando-se às necessidades individuais do aluno.
- **Apresentação:** Este `README.md` detalhado e a demonstração em vídeo garantirão uma apresentação clara, impactante e completa do projeto.

  ---

  ## 🙏 **Agradecimentos**

Gostaríamos de expressar nossa sincera gratidão à **Alura** e ao **Google Gemini** por proporcionarem esta incrível Imersão em IA. Foi uma jornada de aprendizado transformadora, que nos capacitou a desenvolver soluções inovadoras como o InMathMate. Agradecemos a toda a equipe de instrutores, mentores e à comunidade pelo apoio e inspiração constantes. Muito obrigado!

 ---

 Tecendo um futuro onde a matemática é uma experiência acessível e cheia de confiança para todas as crianças! ✖️➗➕➖
