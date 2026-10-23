
# 📋 Requisitos do Sistema

## 🎯 Requisitos de Negócio

| ID | Descrição / Objetivo |
| --- | --- |
| RNEG01 | Reduzir o tempo gasto no processamento e lançamento de cada documento fiscal |
| RNEG02 | Reduzir erros manuais de digitação e classificação contábil com o uso de IA |
| RNEG03 | Aumentar a capacidade de processamento de documentos do escritório sem necessidade de expandir a equipe |
| RNEG04 | Centralizar o envio e a coleta de documentos fiscais dos clientes em uma única plataforma |
| RNEG05 | Reduzir o custo operacional por documento escriturado em relação ao processo manual |
| RNEG06 | Garantir rastreabilidade, integridade e auditoria completa de todas as operações contábeis |

---

## 📌 Requisitos Funcionais

| ID | Descrição |
| --- | --- |
| RF01 | Permitir login com e-mail e senha para administrador, contador e cliente, com controle de acesso rigoroso conforme o perfil |
| RF02 | Permitir recuperação de senha por e-mail para todos os perfis cadastrados |
| RF03 | Permitir ao administrador cadastrar, gerenciar e desativar contas de contadores e acessos globais do sistema |
| RF04 | Permitir ao contador cadastrar e gerenciar os dados cadastrais das empresas clientes (razão social, CNPJ, regime tributário) |
| RF05 | Permitir ao contador criar, redefinir e gerenciar as credenciais de acesso individuais para cada cliente |
| RF06 | Permitir ao contador ativar e desativar clientes e seus acessos ao sistema |
| RF07 | Permitir ao contador cadastrar ou importar o plano de contas individualizado de cada cliente |
| RF08 | Permitir ao cliente enviar um ou mais documentos (PDF, JPG, PNG ou XML) vinculados exclusivamente à sua empresa |
| RF09 | Validar formato e tamanho máximo permitido do arquivo, informando erros imediatamente ao usuário |
| RF10 | Detectar documentos duplicados (por chave de acesso NF-e ou hash de arquivo) e emitir aviso de bloqueio antes do processamento |
| RF11 | Permitir ao cliente acompanhar em tempo real o status de cada documento enviado |
| RF12 | Permitir ao contador enviar documentos em nome de qualquer um de seus clientes |
| RF13 | Extrair dados de notas fiscais em formato XML diretamente do arquivo, sem a necessidade de OCR |
| RF14 | Realizar leitura via OCR para documentos em PDF ou imagem (extraindo data, valor, emitente, CNPJ e descrição) |
| RF15 | Gerar automaticamente por IA a sugestão de lançamento contábil (débito, crédito, valor, data e histórico) com base no plano de contas |
| RF16 | Identificar e classificar automaticamente o tipo do documento (nota fiscal, comprovante, extrato) |
| RF17 | Exibir o nível de confiança do processamento da IA e sinalizar lançamentos com baixa confiança |
| RF18 | Tratar falhas de leitura ou documentos ilegíveis, alterando o status para "Com falha" e notificando para reenvio |
| RF19 | Processar leitura de documentos e geração de sugestões em segundo plano, sem bloquear a navegação do usuário |
| RF20 | Exibir ao contador a fila de documentos pendentes de revisão, com filtros por cliente, status e período |
| RF21 | Exibir na tela de revisão a imagem/visualização do documento original ao lado dos dados extraídos e da sugestão de lançamento |
| RF22 | Permitir ao contador editar as contas contábeis, valores e dados da sugestão antes da aprovação |
| RF23 | Permitir ao contador aprovar lançamentos contábeis garantindo o princípio de partidas dobradas |
| RF24 | Permitir ao contador rejeitar documentos informando a justificativa obrigatória e notificando o cliente |
| RF25 | Registrar histórico de correções manuais do contador para viabilizar melhorias contínuas nas sugestões futuras da IA |
| RF26 | Permitir ao contador exportar os lançamentos aprovados em formato CSV com filtros por cliente e período |
| RF27 | Sinalizar e controlar lançamentos já exportados para evitar duplicação no envio ao sistema contábil externo |
| RF28 | Registrar a trilha de auditoria completa de cada documento (usuário, data/hora, alteração realizada, valores anteriores e novos) |
| RF29 | Permitir ao contador consultar o histórico detalhado de auditoria de qualquer documento ou lançamento |
| RF30 | Disponibilizar painel gerencial (dashboard) com contadores de pendências por cliente, tempo médio de revisão e taxa de acerto da IA |
| RF31 | Enviar notificações automáticas por e-mail para clientes (status de documentos) e contadores (recebimento de novos arquivos) |
| RF32 | Permitir a importação de extratos bancários para conciliação contábil (Fase Futura) |
| RF33 | Permitir a importação de dados contábeis via arquivos em formato JSON padronizado (Fase Futura) |


---

## ⚙️ Requisitos Não Funcionais

| ID    | Descrição |
| ----- | ---------- |
| RNF01 | Garantir autenticação segura com criptografia de dados |
| RNF02 | Proteger os dados dos usuários e documentos |
| RNF03 | Controlar acesso baseado em perfis (contador, cliente e administrador) |
| RNF04 | Processar documentos em tempo quase real |
| RNF05 | Garantir desempenho adequado no upload de arquivos |
| RNF06 | Possuir interface responsiva (mobile-first) |
| RNF07 | Garantir usabilidade e navegação intuitiva |
| RNF08 | Fornecer feedback visual ao usuário (erro, sucesso e carregamento) |
| RNF09 | Permitir validação humana dos dados extraídos |
| RNF10 | Suportar formatos PDF, JPG, PNG, XML e JSON |
| RNF11 | Ser compatível com diferentes dispositivos móveis e navegadores |
| RNF12 | Garantir integridade dos dados enviados |
| RNF13 | Evitar perda de arquivos durante upload |
| RNF14 | Garantir armazenamento seguro dos documentos |
| RNF15 | Registrar logs de auditoria das operações realizadas |
| RNF16 | Garantir disponibilidade contínua do sistema |
| RNF17 | Possuir arquitetura escalável para múltiplos usuários simultâneos |


---

## 📜 Regras de Negócio

| ID   | Descrição |
| ---- | ---------- |
| RN01 | Nenhum lançamento pode ser finalizado sem aprovação do contador |
| RN02 | Documentos enviados devem ser armazenados para auditoria |
| RN03 | Correções feitas pelo contador devem ser registradas |
| RN04 | Arquivos XML e JSON devem ser importados diretamente sem processamento por IA |
| RN05 | Apenas usuários autenticados podem acessar documentos e lançamentos |
| RN06 | Todo documento deve estar vinculado a um cliente cadastrado |
| RN07 | Documentos rejeitados devem permanecer armazenados no sistema |

