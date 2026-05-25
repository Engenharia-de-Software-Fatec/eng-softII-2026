# 📄 Documento de Concepção — Contabilidade Ágil

## 1. Identificação do Documento

| Campo | Informação |
|---|---|
| Projeto | Contabilidade Ágil |
| Versão | 1.0 |
| Data | 25/05/2026 |
| Disciplina | Engenharia de Software II |
| Curso | Análise e Desenvolvimento de Sistemas |
| Instituição | Fatec Sorocaba |
| Status | Em desenvolvimento |

### 👥 Equipe

- Antonio Victor Mello Mielitz Lopes
- Pedro Henrique Dias da Silva
- Giovanni Tomacelli

---

# 2. Introdução

## 📌 Contexto

Escritórios contábeis lidam diariamente com um grande volume de documentos fiscais, comprovantes, notas fiscais, extratos bancários e arquivos financeiros que precisam ser analisados e lançados manualmente nos sistemas contábeis.

Grande parte desse processo ainda depende de operações repetitivas e validações humanas, tornando o trabalho operacional lento e sujeito a falhas.

---

## ⚠️ Problema Identificado

Os processos manuais de escrituração contábil geram:

- Alto tempo de processamento
- Sobrecarga operacional
- Risco elevado de erro humano
- Dificuldade de escalabilidade
- Retrabalho constante
- Baixa produtividade em escritórios contábeis

Além disso, muitos escritórios possuem dificuldades em centralizar documentos e manter um fluxo organizado de validação contábil.

---

# 3. Objetivo do Sistema

O projeto **Contabilidade Ágil** tem como objetivo desenvolver uma aplicação inteligente capaz de automatizar parte do processo de lançamentos contábeis por meio de Inteligência Artificial.

O sistema pretende:

- Automatizar interpretação de documentos
- Reduzir erros manuais
- Aumentar produtividade dos escritórios
- Centralizar documentos contábeis
- Auxiliar contadores na validação de lançamentos
- Reduzir custos operacionais

---

# 4. Visão Geral da Solução

A solução proposta consiste em uma aplicação web com dashboard administrativo voltado para escritórios contábeis.

O sistema permitirá que documentos sejam enviados pelos usuários para processamento automatizado utilizando OCR e Inteligência Artificial.

Após o envio:

1. O sistema recebe os documentos
2. O OCR realiza leitura dos dados
3. A IA interpreta as informações
4. O sistema sugere lançamentos contábeis
5. O contador revisa, aprova ou corrige os dados
6. O histórico permanece armazenado para auditoria

Arquivos XML e JSON poderão ser importados diretamente sem necessidade de interpretação por IA.

---

# 5. Stakeholders

## 👨‍💼 Stakeholders Primários

- Contadores
- Escritórios contábeis
- Empresas clientes

---

## 👨‍💻 Stakeholders Secundários

- Equipe de desenvolvimento
- Instituição acadêmica
- Usuários administrativos

---

# 6. Personas

## 👤 Rogério Silva — Contador

Profissional responsável por validar documentos e garantir precisão nos lançamentos contábeis.

### Objetivos

- Reduzir retrabalho
- Automatizar tarefas repetitivas
- Melhorar produtividade

### Frustrações

- Excesso de documentos
- Processos manuais demorados
- Erros operacionais

---

## 👤 Helena Souza — Gestora Financeira

Responsável pelo acompanhamento financeiro e apoio à tomada de decisões.

### Objetivos

- Obter relatórios rápidos
- Melhorar organização financeira
- Ter informações centralizadas

### Frustrações

- Informações descentralizadas
- Lentidão na geração de dados
- Falta de integração

---

# 7. MVP (Produto Mínimo Viável)

O MVP do sistema será composto pelas seguintes funcionalidades:

- Login e autenticação
- Cadastro de clientes
- Upload de documentos
- Validação de arquivos
- Processamento inicial por IA
- Sugestão automática de lançamentos
- Aprovação/rejeição de lançamentos
- Histórico de documentos
- Dashboard básico

---

# 8. Escopo do Projeto

## ✅ Dentro do Escopo

- Upload de documentos contábeis
- Processamento OCR
- Integração com IA
- Sugestão de lançamentos
- Gestão de clientes
- Dashboard administrativo
- Histórico de documentos
- Controle de usuários

---

## ❌ Fora do Escopo

- Emissão de notas fiscais
- Integração bancária completa
- Folha de pagamento
- Assinatura digital
- Aplicativo mobile nativo
- Integração com sistemas governamentais

---

# 9. Requisitos Principais

## 📋 Requisitos Funcionais

- Permitir autenticação de usuários
- Permitir upload de documentos
- Processar arquivos utilizando IA
- Gerar sugestões automáticas de lançamentos
- Permitir aprovação e correção manual
- Exibir histórico de documentos

---

## ⚙️ Requisitos Não Funcionais

- Garantir segurança dos dados
- Possuir interface responsiva
- Garantir boa performance
- Suportar múltiplos formatos de arquivo
- Registrar logs de auditoria

---

## 📜 Regras de Negócio

- Nenhum lançamento pode ser finalizado sem aprovação do contador
- Todo documento deve estar vinculado a um cliente
- XML e JSON não utilizam processamento por IA
- Correções devem ser registradas no histórico

---

# 10. Tecnologias Envolvidas

| Categoria | Tecnologia |
|---|---|
| Frontend | React |
| Backend | Node.js |
| Banco de Dados | Supabase/PostgreSQL |
| OCR | AWS Textract |
| Inteligência Artificial | AWS Bedrock |
| Deploy | Vercel |
| Modelagem | PlantUML |
| Gestão Ágil | Scrum |

---

# 11. Viabilidade do Projeto

O projeto apresenta viabilidade técnica devido à disponibilidade atual de tecnologias de OCR, IA e computação em nuvem.

Além disso, a solução busca reduzir significativamente os custos operacionais relacionados ao processamento manual de documentos contábeis.

### 💰 Estimativa apresentada

- Processo manual: aproximadamente R$ 109,58 por documento
- Processo automatizado: aproximadamente R$ 0,65 por documento

A utilização de serviços cloud também permite escalabilidade futura do sistema.

---

# 12. Riscos do Projeto

| Risco | Impacto |
|---|---|
| Falhas na interpretação da IA | Médio |
| Documentos ilegíveis | Alto |
| Dependência de APIs externas | Médio |
| Custos elevados de cloud computing | Médio |
| Mudanças de requisitos | Médio |

---

# 13. Metodologia

O projeto utiliza práticas ágeis baseadas no framework Scrum.

Serão utilizadas:

- Sprints
- Product Backlog
- Entregas incrementais
- Revisões contínuas
- Feedback constante

---

# 14. Considerações Finais

O projeto **Contabilidade Ágil** busca modernizar processos contábeis através da automação inteligente de documentos e lançamentos.

A proposta pretende aumentar a produtividade dos escritórios contábeis, reduzir erros operacionais e melhorar a organização das informações financeiras, oferecendo uma solução moderna, escalável e alinhada às necessidades do mercado atual.
