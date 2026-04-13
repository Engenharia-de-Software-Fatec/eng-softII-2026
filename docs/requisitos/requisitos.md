# 📋 Requisitos do Sistema

## 📌 Requisitos Funcionais

| ID   | Descrição                                                             |
| ---- | --------------------------------------------------------------------- |
| RF01 | Permitir ao contador autenticar-se com CRM ou e-mail e senha          |
| RF02 | Permitir recuperação de senha                                         |
| RF03 | Permitir acesso ao painel do contador após login                      |
| RF04 | Permitir selecionar e enviar documentos                               |
| RF05 | Permitir escolher o tipo de documento (extrato, comprovante, NF, XML) |
| RF06 | Permitir upload de arquivos por arrastar e soltar                     |
| RF07 | Validar formatos de arquivo (PDF, JPG, PNG, XML)                      |
| RF08 | Validar tamanho máximo de arquivo (10MB)                              |
| RF09 | Exibir lista de arquivos selecionados                                 |
| RF10 | Permitir envio de arquivos para processamento por IA                  |
| RF11 | Extrair automaticamente dados dos documentos                          |
| RF12 | Exibir nível de confiança da extração de dados                        |
| RF13 | Sugerir lançamento contábil automaticamente                           |
| RF14 | Permitir edição dos dados extraídos                                   |
| RF15 | Permitir aprovação de lançamento                                      |
| RF16 | Permitir rejeição de lançamento                                       |
| RF17 | Permitir visualização do documento digitalizado                       |
| RF18 | Permitir seleção de cliente                                           |
| RF19 | Permitir busca de cliente por nome ou CNPJ                            |
| RF20 | Permitir filtrar clientes (todas, pendentes, em dia)                  |
| RF21 | Exibir status do cliente (pendências ou em dia)                       |
| RF22 | Exibir sugestões inteligentes baseadas em histórico                   |
| RF23 | Permitir navegação entre telas do sistema                             |
| RF24 | Exibir notificações ao usuário                                        |

---

## ⚙️ Requisitos Não Funcionais

| ID    | Descrição                                                         |
| ----- | ----------------------------------------------------------------- |
| RNF01 | Garantir autenticação segura com criptografia de dados            |
| RNF02 | Proteger os dados dos usuários e documentos                       |
| RNF03 | Controlar acesso baseado em perfis (contador/cliente)             |
| RNF04 | Processar documentos em tempo quase real                          |
| RNF05 | Garantir desempenho adequado no upload de arquivos                |
| RNF06 | Possuir interface responsiva (mobile-first)                       |
| RNF07 | Garantir usabilidade e navegação intuitiva                        |
| RNF08 | Fornecer feedback visual ao usuário (erro, sucesso, carregamento) |
| RNF09 | Exibir nível de confiança da inteligência artificial              |
| RNF10 | Permitir validação humana dos dados extraídos                     |
| RNF11 | Suportar formatos PDF, JPG, PNG e XML                             |
| RNF12 | Ser compatível com diferentes dispositivos móveis                 |
| RNF13 | Garantir integridade dos dados enviados                           |
| RNF14 | Evitar perda de arquivos durante upload                           |

---

## 📜 Regras de Negócio

| ID    | Descrição                                                         |
| ----- | ----------------------------------------------------------------- |
| RN01 | Nenhum lançamento pode ser finalizado sem aprovação do contador.   |
| RNF02 | Documentos enviados devem ser armazenados para auditoria.         |
| RNF03 | Correções feitas pelo contador devem ser registradas.             |
