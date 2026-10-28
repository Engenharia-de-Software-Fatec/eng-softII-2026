
# 📋 Requisitos do Sistema

## 🎯 Requisitos de Negócio


| ID | Descrição / Objetivo |
| --- | --- |
| RNEG01 | Reduzir o tempo necessário para o processamento e o lançamento de documentos fiscais, otimizando as atividades operacionais do escritório contábil. |
| RNEG02 | Minimizar os erros manuais de digitação e classificação contábil por meio da utilização de inteligência artificial no processamento e na sugestão de lançamentos. |
| RNEG03 | Aumentar a capacidade de processamento de documentos fiscais do escritório contábil, permitindo atender a uma maior demanda sem exigir uma expansão proporcional da equipe. |
| RNEG04 | Centralizar o envio, o recebimento e o acompanhamento de documentos fiscais dos clientes em uma única plataforma digital. |
| RNEG05 | Reduzir o custo operacional por documento escriturado em comparação ao processo manual, buscando maior eficiência na utilização dos recursos do escritório. |
| RNEG06 | Assegurar a rastreabilidade das operações, a integridade das informações e o registro auditável das atividades realizadas no sistema, permitindo a consulta ao histórico de alterações e operações contábeis. |


---


## 📌 Requisitos Funcionais

| ID | Descrição |
| --- | --- |
| RF01 | Permitir a autenticação por e-mail e senha para administradores, contadores e clientes, garantindo o controle de acesso conforme o perfil de cada usuário. |
| RF02 | Permitir a recuperação de senha por e-mail para todos os perfis cadastrados no sistema. |
| RF03 | Permitir ao administrador cadastrar, gerenciar e desativar contas de contadores, além de gerenciar os acessos globais do sistema. |
| RF04 | Permitir ao contador cadastrar e gerenciar os dados das empresas clientes, incluindo razão social, CNPJ e regime tributário. |
| RF05 | Permitir ao contador criar, redefinir e gerenciar as credenciais de acesso individuais dos clientes. |
| RF06 | Permitir ao contador ativar e desativar clientes e seus respectivos acessos ao sistema. |
| RF07 | Permitir ao contador cadastrar ou importar o plano de contas individualizado de cada empresa cliente. |
| RF08 | Permitir ao cliente enviar um ou mais documentos nos formatos PDF, JPG, PNG ou XML, vinculando-os exclusivamente à sua própria empresa. |
| RF09 | Validar o formato e o tamanho máximo permitido dos arquivos enviados, informando imediatamente ao usuário eventuais inconsistências. |
| RF10 | Identificar documentos duplicados por meio da chave de acesso da NF-e ou do hash do arquivo, emitindo um aviso e impedindo o processamento de duplicatas. |
| RF11 | Permitir ao cliente acompanhar o status de processamento de cada documento enviado, com atualização das informações conforme o andamento das etapas. |
| RF12 | Permitir ao contador enviar documentos em nome de qualquer empresa cliente sob sua responsabilidade. |
| RF13 | Extrair diretamente dos arquivos XML os dados das notas fiscais, dispensando a utilização de OCR nesses documentos. |
| RF14 | Realizar o reconhecimento óptico de caracteres (OCR) em documentos PDF ou imagens, extraindo informações como data, valor, emitente, CNPJ e descrição. |
| RF15 | Gerar automaticamente, por meio de inteligência artificial, sugestões de lançamentos contábeis contendo débito, crédito, valor, data e histórico, com base no plano de contas da empresa cliente. |
| RF16 | Identificar e classificar automaticamente os tipos de documentos enviados, como notas fiscais, comprovantes e extratos. |
| RF17 | Exibir o nível de confiança do processamento realizado pela inteligência artificial e sinalizar as sugestões de lançamentos que apresentarem baixa confiança. |
| RF18 | Identificar falhas de leitura ou documentos ilegíveis, alterar o status do documento para "Com falha" e notificar o usuário responsável para que seja realizado o reenvio. |
| RF19 | Executar o processamento dos documentos e a geração de sugestões de lançamentos em segundo plano, permitindo que o usuário continue navegando pelo sistema. |
| RF20 | Disponibilizar ao contador uma fila de documentos pendentes de revisão, com filtros por cliente, status e período. |
| RF21 | Exibir, na tela de revisão, a visualização do documento original ao lado dos dados extraídos e da sugestão de lançamento contábil gerada pela inteligência artificial. |
| RF22 | Permitir ao contador editar as contas contábeis, os valores e os demais dados da sugestão de lançamento antes de sua aprovação. |
| RF23 | Permitir ao contador aprovar lançamentos contábeis, garantindo o cumprimento do princípio das partidas dobradas. |
| RF24 | Permitir ao contador rejeitar documentos mediante o preenchimento obrigatório de uma justificativa, notificando o cliente sobre a rejeição. |
| RF25 | Registrar o histórico de correções manuais realizadas pelo contador, possibilitando sua utilização na melhoria contínua das sugestões geradas pela inteligência artificial. |
| RF26 | Permitir ao contador exportar os lançamentos aprovados em formato CSV, com possibilidade de filtragem por cliente e período. |
| RF27 | Identificar e controlar os lançamentos já exportados, evitando duplicidade no envio de informações aos sistemas contábeis externos. |
| RF28 | Registrar uma trilha de auditoria dos documentos e das operações realizadas, incluindo usuário responsável, data e hora, alterações efetuadas e valores anteriores e posteriores às modificações. |
| RF29 | Permitir ao contador consultar o histórico detalhado de auditoria de qualquer documento ou lançamento contábil. |
| RF30 | Disponibilizar um painel gerencial (dashboard) com indicadores de pendências por cliente, tempo médio de revisão e taxa de acerto da inteligência artificial. |
| RF31 | Enviar notificações automáticas por e-mail aos clientes sobre o status de seus documentos e aos contadores sobre o recebimento de novos arquivos. |




---


## ⚙️ Requisitos Não Funcionais

| ID | Descrição |
| --- | --- |
| RNF01 | Garantir a autenticação segura dos usuários e a proteção dos dados por meio de mecanismos adequados de segurança e criptografia. |
| RNF02 | Proteger os dados dos usuários e os documentos armazenados contra acessos não autorizados, alterações indevidas e exposição de informações. |
| RNF03 | Garantir o controle de acesso baseado em perfis, estabelecendo permissões adequadas para contadores, clientes e administradores. |
| RNF04 | Garantir que o processamento dos documentos ocorra em tempo quase real, minimizando o tempo de espera dos usuários. |
| RNF05 | Garantir desempenho adequado durante o envio de arquivos, evitando atrasos excessivos e proporcionando uma experiência eficiente ao usuário. |
| RNF06 | Disponibilizar uma interface responsiva, com abordagem mobile-first, adaptável a diferentes tamanhos de tela e dispositivos. |
| RNF07 | Garantir usabilidade e navegação intuitiva, facilitando a utilização das funcionalidades por todos os perfis de usuários. |
| RNF08 | Fornecer feedback visual claro sobre as operações realizadas, incluindo mensagens de erro, confirmações de sucesso e indicadores de carregamento. |
| RNF09 | Permitir a validação humana dos dados extraídos dos documentos e das sugestões de lançamentos contábeis geradas automaticamente. |
| RNF10 | Garantir suporte aos formatos de arquivo PDF, JPG, PNG, XML e JSON, respeitando as funcionalidades previstas para cada formato. |
| RNF11 | Garantir compatibilidade com diferentes dispositivos móveis e navegadores web, proporcionando acesso adequado à plataforma. |
| RNF12 | Preservar a integridade dos dados enviados, evitando alterações indevidas e inconsistências durante o processamento e o armazenamento. |
| RNF13 | Minimizar o risco de perda de arquivos durante o envio, garantindo mecanismos adequados de controle e confirmação do recebimento. |
| RNF14 | Garantir o armazenamento seguro dos documentos fiscais e contábeis, protegendo-os contra acessos indevidos e perdas não autorizadas. |
| RNF15 | Registrar logs de auditoria das operações realizadas no sistema, permitindo o acompanhamento das atividades e a investigação de eventuais inconsistências. |
| RNF16 | Buscar alta disponibilidade do sistema, minimizando interrupções e permitindo o acesso à plataforma de forma contínua. |
| RNF17 | Adotar uma arquitetura escalável, capaz de suportar o crescimento do número de usuários e o processamento de múltiplas operações simultâneas. |



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

