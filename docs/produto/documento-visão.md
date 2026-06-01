# 📄 Documento de Visão — Contabilidade Ágil

## 1. Identificação do Documento

| Campo           | Informação                |
| --------------- | ------------------------- |
| Nome do Projeto | Contabilidade Ágil        |
| Versão          | v1.0                      |
| Data            | Junho/2026                |
| Status          | Em elaboração             |
| Disciplina      | Engenharia de Software II |
| Instituição     | Fatec Sorocaba            |

### Equipe

* Antonio Victor Mello Mielitz Lopes
* Pedro Henrique Dias da Silva
* Giovanni Tomacelli

---

# 2. Introdução

## Contexto do Projeto

Escritórios contábeis lidam diariamente com uma grande quantidade de documentos fiscais, comprovantes, extratos bancários e notas fiscais que precisam ser analisados e transformados em lançamentos contábeis.

Grande parte desse trabalho ainda é realizada manualmente, exigindo tempo significativo dos profissionais e aumentando a probabilidade de erros operacionais.

## Motivação

A crescente demanda por produtividade e redução de custos tem impulsionado a adoção de tecnologias de automação e Inteligência Artificial em diversos setores, incluindo a contabilidade.

O projeto Contabilidade Ágil surge como uma solução para auxiliar escritórios contábeis a automatizar tarefas repetitivas e reduzir o tempo gasto em lançamentos manuais.

## Problema Identificado

* Alto volume de documentos para processamento.
* Dependência excessiva de trabalho manual.
* Possibilidade de erros humanos.
* Baixa escalabilidade operacional.
* Dificuldade de centralização de documentos e histórico.

---

# 3. Objetivo do Sistema

## Objetivo Principal

Desenvolver uma plataforma inteligente capaz de automatizar o processamento de documentos contábeis por meio de Inteligência Artificial, reduzindo erros manuais e aumentando a produtividade dos escritórios contábeis.

## Benefícios Esperados

* Redução do tempo de processamento.
* Redução de erros operacionais.
* Centralização documental.
* Aumento da produtividade.
* Melhoria do processo de auditoria.

## Resultado Esperado

Permitir que documentos sejam enviados, processados automaticamente e convertidos em sugestões de lançamentos contábeis para posterior validação pelo contador.

---

# 4. Visão Geral da Solução

A solução consiste em uma plataforma web integrada com tecnologias de OCR e Inteligência Artificial.

O sistema será capaz de:

1. Receber documentos contábeis.
2. Extrair dados automaticamente.
3. Interpretar informações relevantes.
4. Gerar sugestões de lançamentos contábeis.
5. Permitir revisão e aprovação humana.
6. Manter histórico completo para auditoria.

## Diferenciais da Solução

* Integração com IA generativa.
* Processamento automatizado de documentos.
* Fluxo de aprovação controlado.
* Centralização de informações.
* Histórico completo de alterações.

---

# 5. Escopo do Projeto

## Dentro do Escopo

* Autenticação de usuários.
* Cadastro de clientes.
* Upload de documentos.
* Processamento OCR.
* Integração com IA.
* Sugestão automática de lançamentos.
* Aprovação e rejeição de lançamentos.
* Histórico de documentos.
* Dashboard de acompanhamento.

## Fora do Escopo

* Aplicativo mobile nativo.
* Integração com ERPs externos.
* Emissão automática de notas fiscais.
* Automação completa do fechamento contábil.
* Processamento financeiro bancário.
* Integrações governamentais.
* Gestão empresarial completa.

---

# 6. Stakeholders

## Clientes

* Escritórios contábeis.
* Empresas clientes.

## Usuários

* Contadores.
* Analistas contábeis.
* Gestores financeiros.

## Equipe Técnica

* Desenvolvedores.
* Administradores de infraestrutura.

## Parceiros Tecnológicos

* AWS Textract.
* AWS Bedrock.
* Supabase.
* Vercel.

---

# 7. Perfis de Usuário

## Rogério Silva — Contador

### Características

* Profissional experiente.
* Responsável pela validação contábil.
* Alto volume operacional.

### Necessidades

* Reduzir retrabalho.
* Automatizar tarefas repetitivas.
* Garantir precisão.

### Objetivos

* Aumentar produtividade.
* Melhorar qualidade das entregas.

---

## Helena Souza — Gestora Financeira

### Características

* Atua no setor financeiro.
* Necessita de informações rápidas e confiáveis.

### Necessidades

* Relatórios organizados.
* Dados centralizados.

### Objetivos

* Melhorar tomada de decisão.
* Otimizar gestão financeira.

---

# 8. Problemas e Oportunidades

| Problema                 | Impacto                  | Oportunidade                 |
| ------------------------ | ------------------------ | ---------------------------- |
| Processamento manual     | Baixa produtividade      | Automação com IA             |
| Grande volume documental | Sobrecarga operacional   | OCR automatizado             |
| Erros humanos            | Retrabalho               | Sugestões inteligentes       |
| Dados descentralizados   | Dificuldade de auditoria | Centralização de informações |

---

# 9. Necessidades do Negócio

## Demandas Operacionais

* Redução do tempo de lançamento.
* Organização documental.
* Melhoria do fluxo de aprovação.

## Necessidades Estratégicas

* Aumento da produtividade.
* Escalabilidade operacional.
* Redução de custos.

---

# 10. Funcionalidades de Alto Nível

## Gestão de Usuários

Permite autenticação e controle de acesso.

## Gestão de Clientes

Permite cadastro e organização dos clientes atendidos.

## Upload de Documentos

Recebe documentos contábeis para processamento.

## OCR Inteligente

Extrai dados automaticamente dos documentos.

## Sugestão de Lançamentos

Gera lançamentos contábeis utilizando IA.

## Aprovação de Lançamentos

Permite revisão e aprovação pelo contador.

## Histórico

Mantém registro de alterações e auditoria.

---

# 11. Requisitos Gerais

## Requisitos Funcionais

* Upload de documentos.
* Processamento automático.
* Sugestão de lançamentos.
* Aprovação manual.
* Histórico de alterações.

## Requisitos Não Funcionais

* Segurança dos dados.
* Interface responsiva.
* Disponibilidade contínua.
* Boa performance.

## Restrições Técnicas

* Dependência de serviços AWS.
* Necessidade de conexão com internet.

---

# 12. Regras de Negócio

* Nenhum lançamento pode ser finalizado sem aprovação do contador.
* Todo documento deve estar vinculado a um cliente.
* XML e JSON não passam pela IA.
* Alterações devem ser auditáveis.
* Apenas usuários autorizados podem acessar documentos.

---

# 13. Premissas

* Os usuários possuem acesso à internet.
* Os documentos possuem qualidade mínima para OCR.
* Os serviços AWS estarão disponíveis.
* Os contadores revisarão os lançamentos sugeridos.

---

# 14. Restrições

## Tecnológicas

* Dependência de OCR e IA.

## Financeiras

* Uso de ferramentas gratuitas ou de baixo custo.

## Operacionais

* Equipe reduzida de desenvolvimento.

## Acadêmicas

* Desenvolvimento limitado ao calendário da disciplina.

---

# 15. Riscos Iniciais

* Falhas na interpretação da IA.
* Documentos ilegíveis.
* Dependência de APIs externas.
* Custos de processamento.
* Mudanças de escopo.
* Atrasos de cronograma.

---

# 16. Integrações Externas

| Serviço      | Finalidade              |
| ------------ | ----------------------- |
| AWS Textract | OCR                     |
| AWS Bedrock  | Inteligência Artificial |
| Supabase     | Banco de Dados          |
| Vercel       | Hospedagem              |

---

# 17. Visão Arquitetural Inicial

## Frontend

* React

## Backend

* Node.js

## Banco de Dados

* PostgreSQL (Supabase)

## Infraestrutura

* AWS
* Vercel

---

# 18. Critérios de Sucesso

* Redução do tempo de processamento contábil.
* Precisão mínima de 85% na extração de dados.
* Redução de erros manuais.
* Funcionamento estável do MVP.
* Aceitação pelos usuários finais.

---

# 19. Roadmap Inicial

## MVP

* Login
* Cadastro de clientes
* Upload de documentos
* OCR
* IA
* Sugestão de lançamentos
* Aprovação manual
* Histórico

## Próxima Fase

* Dashboard gerencial
* Relatórios automatizados
* Notificações

## Evoluções Futuras

* Integração com ERPs
* Aplicativo mobile
* Analytics avançado
* Inteligência financeira

---

# 20. Glossário

| Termo    | Definição                           |
| -------- | ----------------------------------- |
| OCR      | Reconhecimento Óptico de Caracteres |
| IA       | Inteligência Artificial             |
| AWS      | Amazon Web Services                 |
| ERP      | Sistema Integrado de Gestão         |
| MVP      | Produto Mínimo Viável               |
| Scrum    | Framework Ágil                      |
| Textract | Serviço OCR da AWS                  |
| Bedrock  | Plataforma de IA da AWS             |

---

# 21. Referências

* README do projeto
* Documento de Concepção
* Documento de Requisitos
* Casos de Uso
* Personas
* Diagrama de Classes
* AWS Textract Documentation
* AWS Bedrock Documentation
* Material de Engenharia de Requisitos
* Material de Scrum
* Repositório GitHub do projeto
