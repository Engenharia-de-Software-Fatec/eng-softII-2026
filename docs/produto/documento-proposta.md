# Proposta de Projeto Integrador

**Disciplina:** Engenharia de Software 2  
**Turma:** ADS 3° Semestre — Fatec Sorocaba  
**Professor:** Glauco Todesco  
**Data:** 25/05/2026  
**Grupo:** Contabilidade Ágil  

---

## Nome do Projeto

Contabilidade Ágil

## Nome de Usuário no GitHub

[Engenharia-de-Software-Fatec](https://github.com/Engenharia-de-Software-Fatec/eng-softII-2026)

---

## Grupo de Alunos

| RA | Nome | E-mail |
|----|------|--------|
| 0030482511008 | Antonio Victor Mello Mielitz Lopes | tonymielitz@gmail.com |
| 0030482511042 | Pedro Henrique Dias da Silva | 21pedrohds@gmail.com |
| 0030482511037 | Giovanni Tomacelli | giovannitomacelli06@gmail.com |

---

## 1. Compreensão do Problema

Escritórios contábeis lidam diariamente com um grande volume de documentos fiscais, comprovantes, extratos bancários e notas fiscais que precisam ser analisados e lançados manualmente nos sistemas contábeis. Esse processo exige muito tempo dos profissionais e está sujeito a falhas humanas, retrabalho e atrasos, principalmente em períodos de fechamento contábil.

Além disso, muitas empresas possuem documentos descentralizados e pouco organizados, dificultando o acesso rápido às informações financeiras e aumentando a complexidade da rotina operacional. A dependência de processos manuais reduz a produtividade dos escritórios e dificulta a escalabilidade do serviço prestado.

Outro problema identificado é a dificuldade em manter padronização e agilidade na contabilização de documentos. Pequenos erros de digitação, classificação incorreta de contas e demora na conferência dos lançamentos podem impactar diretamente a qualidade das informações financeiras entregues aos clientes.

---

## 2. Proposta de Solução de Software e Viabilidade

A proposta do projeto **Contabilidade Ágil** é desenvolver uma aplicação web capaz de automatizar parte do processo contábil utilizando Inteligência Artificial e OCR para interpretação de documentos fiscais e financeiros.

O sistema permitirá que usuários realizem upload de documentos, que serão processados automaticamente para extração de dados e sugestão de lançamentos contábeis. O contador poderá revisar, corrigir e aprovar os lançamentos antes da contabilização final, garantindo segurança e validação humana.

A solução é viável por utilizar tecnologias modernas baseadas em nuvem, frameworks web amplamente utilizados e serviços de IA já disponíveis no mercado, reduzindo custos de infraestrutura e acelerando o desenvolvimento do sistema.

---

## 3. Visão Geral dos Pré-Requisitos

**Atores do sistema:**
- **Cliente (Empresa):** responsável por enviar os documentos contábeis
- **Contador (Administrador):** responsável por validar, corrigir e aprovar os lançamentos
- **Sistema de IA:** responsável por interpretar os documentos e gerar os lançamentos automaticamente

**Funções do sistema:**
- Autenticação segura com diferentes perfis de usuário (Administrador, Contador e Cliente)
- Upload de documentos nos formatos PDF, JPG, PNG, XML e JSON, com validação de formato e tamanho
- Processamento automático por IA (OCR + Bedrock) para extração de dados contábeis
- Importação direta de dados para documentos estruturados (XML/JSON), sem necessidade de OCR
- Geração de sugestões de lançamentos contábeis a partir dos documentos enviados
- Revisão, correção e aprovação dos lançamentos pelo contador antes da contabilização final
- Histórico de documentos enviados e lançamentos realizados
- Geração de relatórios contábeis (Balancete, DRE, Razão, Diário)
- Gerenciamento de clientes e usuários pelo administrador

**Atributos desejados do sistema:**
- Interface responsiva e navegação intuitiva (desktop e mobile)
- Processamento rápido dos documentos
- Segurança e privacidade dos dados
- Escalabilidade para atender múltiplos clientes simultaneamente

---

## 4. Conceitos e Tecnologias Envolvidos

**Conceitos:** Engenharia de Software, Inteligência Artificial, OCR (Reconhecimento Óptico de Caracteres), sistemas web, banco de dados relacional, automação contábil e metodologia ágil.

**Tecnologias:**

| Camada | Tecnologia |
|--------|------------|
| Frontend | React |
| Backend | Node.js |
| Banco de Dados | Supabase / PostgreSQL |
| OCR | Amazon Textract |
| IA | Amazon Bedrock |
| Deploy | Vercel |
| Versionamento | GitHub |
| Metodologia | Scrum |

> As tecnologias listadas são iniciais e podem ser alteradas no decorrer do projeto.

---

## 5. Situação Atual (Estado-da-Arte)

Atualmente existem sistemas contábeis tradicionais que auxiliam no armazenamento de documentos e geração de relatórios financeiros, porém muitos deles ainda dependem fortemente de lançamentos manuais realizados pelos contadores.

Algumas soluções modernas utilizam OCR para leitura de documentos, porém frequentemente apresentam dificuldades na interpretação contextual dos dados ou exigem grande intervenção manual para validação das informações extraídas.

O diferencial do projeto **Contabilidade Ágil** será integrar OCR com Inteligência Artificial para sugerir automaticamente lançamentos contábeis, mantendo o contador no processo de aprovação final. Também será realizada pesquisa com possíveis usuários — contadores e gestores financeiros — para identificar dificuldades da rotina atual e validar as funcionalidades mais importantes para o sistema.

---

## 6. Estimativa de Custo do Projeto

**Impacto financeiro da solução:**

| Cenário | Custo estimado por documento |
|---------|------------------------------|
| Sem a aplicação (processo manual) | ~R$ 109,58 |
| Com a aplicação (automatizado) | ~R$ 0,65 |

A redução de custo por documento representa uma economia significativa para escritórios contábeis que processam grandes volumes de documentos mensalmente.

**Custos de infraestrutura do projeto:**

| Item | Custo Estimado |
|------|----------------|
| Hospedagem Frontend (Vercel) | Gratuito / baixo custo |
| Banco de Dados (Supabase) | Gratuito no plano inicial |
| OCR (AWS Textract) | Variável conforme uso |
| IA (AWS Bedrock) | Variável conforme processamento |
| Domínio do sistema | ~R$ 40,00/ano |
| Ferramentas de desenvolvimento | Gratuitas |

**Estimativa geral:** baixo custo em ambiente acadêmico, utilizando majoritariamente planos gratuitos e créditos educacionais das plataformas.

---

## 7. Glossário

| Termo | Definição |
|-------|-----------|
| OCR | Tecnologia de reconhecimento óptico de caracteres em imagens e documentos |
| IA | Inteligência Artificial |
| Lançamento Contábil | Registro financeiro realizado na contabilidade |
| Dashboard | Painel visual com indicadores e informações resumidas |
| Documento Fiscal | Arquivo relacionado a movimentações financeiras ou tributárias |
| XML | Formato de arquivo estruturado utilizado em documentos fiscais |
| Conta Contábil | Categoria utilizada para classificar movimentações financeiras |
| Upload | Envio de arquivos pelo usuário para o sistema |
| Scrum | Framework de gerenciamento ágil de projetos |
| Backlog | Lista priorizada de tarefas do projeto |
