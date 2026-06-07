# 🚀 Back-end do Zero à Prática: Caderno Temático Node.js & TypeScript

Este repositório é o resultado do meu processo de **aprendizagem ativa** durante o **Bootcamp Sem Parar Corpay - Back-end do Zero à Prática**, realizado na plataforma **DIO**. O foco aqui não é apenas o código final, mas a documentação da jornada de aprendizado, curadoria de conhecimento e engenharia de prompts utilizando o **NotebookLM**.

## 📝 Contexto e Objetivos

O assunto central deste caderno temático é o **desenvolvimento de APIs escaláveis e modernas utilizando o ecossistema Node.js**. 

**Meus objetivos principais de estudo foram:**
*   **Domínio de Arquitetura:** Implementar a **arquitetura em camadas** (Routes, Controllers, Services, Repositories, Entities e Schemas) para garantir código limpo e testável.
*   **Excelência em TypeScript:** Utilizar o TypeScript como superset para prevenir bugs em tempo de desenvolvimento através de tipagem estática e interfaces.
*   **Alta Performance:** Avaliar e implementar o framework **Fastify**, comparando seu throughput e latência com o tradicional Express.
*   **Integração com IA:** Desenvolver agentes e assistentes de código integrando aplicações Node.js com a **API da OpenAI**.
*   **Cultura DevOps:** Aprender o versionamento semântico com Git e a implantação de aplicações com banco de dados **MongoDB** no **Microsoft Azure**.

## 📚 Curadoria de Fontes

Para este estudo, selecionei e analisei as seguintes fontes técnicas:

1.  **Arquitetura em camadas com Node.js, Fastify, Prisma e Zod:** Um guia sobre separação de responsabilidades (Jefferson Lima - DIO).
2.  **Guia Prático de TypeScript:** Manual sobre tipos, interfaces, generics e decorators (Thiago da Silva Adriano).
3.  **Fastify vs Express: Teste de Fogo na Prática:** Benchmark comparativo de performance entre os principais frameworks (Loomi Digital).
4.  **Tutorial de integração com APIs da OpenAI via Node.js:** Passo a passo para criar aplicações inteligentes (LuizTools).
5.  **Versionamento de Código com Git:** Boas práticas para organização de repositórios e colaboração (Monica Bomfim - DIO).

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Documentar o raciocínio por trás da interação com a IA é fundamental para o mercado atual. Abaixo, registro os desafios encontrados:

### Perguntas Estratégicas e Variações
*   **Pergunta Inicial:** "Como estruturar um projeto Node.js?"
    *   *Resultado:* Resposta genérica focada em Express.
*   **Prompt Refinado (Engenharia):** "Explique a arquitetura em camadas aplicada ao framework Fastify, detalhando o papel da camada de 'Services' em relação ao 'Repository' usando Prisma."
    *   *Referência utilizada:* Fonte, que detalha como o Service orquestra a lógica de negócio sem conhecer detalhes do banco de dados.

### "Cicatrizes" e Dificuldades
*   **O Dilema do "Any":** No início, a dificuldade foi evitar o tipo `any` em integrações de API. A solução foi criar **Interfaces** específicas para os contratos de resposta, garantindo o benefício do IntelliSense e segurança de tipo.
*   **Callback Hell:** Durante o estudo de funções assíncronas, o desafio foi o aninhamento excessivo de funções. A "cicatriz" foi corrigida através da implementação de `async/await` e `Promises`, tornando o código estruturado e legível.

## 📖 Miniguia de Estudo (Entrega Final)

### Resumo Estruturado: Arquitetura em Camadas
Para sair do "caos" e ter um backend organizado, a estrutura adotada divide a aplicação em:
1.  **Routes:** Define métodos HTTP e caminhos.
2.  **Controllers:** Ponte entre o HTTP e o domínio; extrai dados do request.
3.  **Services:** O coração da aplicação; onde vivem as regras de negócio.
4.  **Repositories:** Isola o acesso ao banco de dados (ex: Prisma).
5.  **Schemas (Zod):** Valida rigorosamente as entradas e saídas de dados.

### 📕 Glossário de Conceitos
*   **REPL (Read Eval Print Loop):** Ambiente interativo para execução de JavaScript no shell para testes rápidos.
*   **Transpilação:** Processo de converter código TypeScript em JavaScript para que os navegadores/runtime possam interpretar.
*   **Hoisting:** Mecanismo do JavaScript que move declarações de variáveis para o topo do escopo antes da execução.
*   **Singleton:** Padrão de projeto utilizado, por exemplo, na exportação de controllers para garantir uma única instância na aplicação.
*   **KQL (Kusto Query Language):** Linguagem utilizada para consultar logs no Azure Monitor.

### 🛠️ Prompts Reutilizáveis para Revisão
*   *"Resuma os principais modificadores de acesso (public, private, protected) em TypeScript com exemplos práticos baseados em uma classe 'Conta Bancária'."*
*   *"Explique a diferença de performance entre os métodos 'createReadStream' e 'readFile' para manipulação de arquivos grandes no Node.js."*
*   *"Gere um checklist de segurança para uma API Node.js incluindo sanitização de dados e tratamento de erros."*
