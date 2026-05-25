
# 📋 Requisitos do Sistema

## 📌 Requisitos Funcionais

| ID   | Descrição |
| ---- | ---------- |
| RF01 | Permitir ao contador autenticar-se com CRC ou e-mail e senha |
| RF02 | Permitir recuperação de senha |
| RF03 | Permitir logout do sistema |
| RF04 | Permitir acesso ao dashboard após login |
| RF05 | Permitir cadastro e gerenciamento de usuários |
| RF06 | Permitir cadastro e gerenciamento de clientes |
| RF07 | Permitir selecionar e enviar documentos |
| RF08 | Permitir escolher o tipo de documento (extrato, comprovante, NF, XML, JSON) |
| RF09 | Permitir upload de arquivos por arrastar e soltar |
| RF10 | Validar formatos de arquivo (PDF, JPG, PNG, XML e JSON) |
| RF11 | Validar tamanho máximo de arquivo (10MB) |
| RF12 | Exibir lista de arquivos selecionados |
| RF13 | Permitir envio de arquivos para processamento por IA |
| RF14 | Ignorar processamento por IA para arquivos XML e JSON |
| RF15 | Extrair automaticamente dados dos documentos |
| RF16 | Exibir nível de confiança da extração de dados |
| RF17 | Sugerir lançamento contábil automaticamente |
| RF18 | Permitir edição dos dados extraídos |
| RF19 | Permitir aprovação de lançamento |
| RF20 | Permitir rejeição de lançamento |
| RF21 | Permitir correção de lançamento |
| RF22 | Permitir visualização do documento digitalizado |
| RF23 | Permitir seleção de cliente |
| RF24 | Permitir busca de cliente por nome ou CNPJ |
| RF25 | Permitir filtrar clientes (todas, pendentes, em dia) |
| RF26 | Exibir status do cliente (pendências ou em dia) |
| RF27 | Exibir sugestões inteligentes baseadas em histórico |
| RF28 | Permitir visualização do histórico de documentos |
| RF29 | Permitir geração de relatórios contábeis |
| RF30 | Permitir navegação entre telas do sistema |
| RF31 | Exibir notificações ao usuário |
| RF32 | Registrar histórico de alterações realizadas |

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
| RNF09 | Exibir nível de confiança da inteligência artificial |
| RNF10 | Permitir validação humana dos dados extraídos |
| RNF11 | Suportar formatos PDF, JPG, PNG, XML e JSON |
| RNF12 | Ser compatível com diferentes dispositivos móveis e navegadores |
| RNF13 | Garantir integridade dos dados enviados |
| RNF14 | Evitar perda de arquivos durante upload |
| RNF15 | Garantir armazenamento seguro dos documentos |
| RNF16 | Registrar logs de auditoria das operações realizadas |
| RNF17 | Garantir disponibilidade contínua do sistema |
| RNF18 | Possuir arquitetura escalável para múltiplos usuários simultâneos |

---

## 📜 Regras de Negócio

| ID   | Descrição |
| ---- | ---------- |
| RN01 | Nenhum lançamento pode ser finalizado sem aprovação do contador |
| RN02 | Documentos enviados devem ser armazenados para auditoria |
| RN03 | Correções feitas pelo contador devem ser registradas |
| RN04 | Arquivos XML e JSON devem ser importados diretamente sem processamento por IA |
| RN05 | O sistema deve alertar o contador quando a confiança da IA for inferior a 80% |
| RN06 | Apenas usuários autenticados podem acessar documentos e lançamentos |
| RN07 | Todo documento deve estar vinculado a um cliente cadastrado |
| RN08 | Documentos rejeitados devem permanecer armazenados no sistema |

