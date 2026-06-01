## Caso de uso: Enviar e Processar Documentos

**Atores:** Cliente, Contador, Sistema de IA  
**Interessados:** Escritório contábil, Clientes, Setor financeiro  

---

### Precondições
- O contador está autenticado no sistema  
- O cliente já está cadastrado  
- Os documentos estão disponíveis para envio  

---

### Pós-condições
- Os documentos foram processados  
- Os dados foram extraídos e armazenados  
- Um lançamento contábil foi gerado (aprovado ou rejeitado)  

---

### Requisitos correlacionados
RF04, RF10, RF11, RF13, RF15, RF16  

---

### Variações tecnológicas
- Upload pode ser feito via seleção de arquivo ou arrastar e soltar  
- Processamento pode usar diferentes motores de IA  
- Visualização pode variar entre mobile e desktop  

---

### Questões em aberto
- Quais tipos de documentos terão prioridade no processamento?  

---

## Fluxo principal

1. O cliente ou contador acessa a funcionalidade de envio de documentos
2. O cliente ou contador seleciona o cliente relacionado
3. O cliente ou contador seleciona o tipo de documento
4. O cliente ou contador adiciona os arquivos
5. [EV] O sistema valida os arquivos (formato e tamanho)  
6. O contador confirma o envio  
7. [EV] O sistema envia os documentos para processamento  
8. [EV] O Sistema de IA extrai os dados dos documentos  
9. O sistema exibe os dados extraídos  
10. O contador revisa as informações  
11. O contador aprova o lançamento  
12. O sistema registra o lançamento contábil  

---

## Fluxos Alternativos

### FA01. Envio realizado pelo cliente

1. O cliente acessa sua área de documentos
2. O cliente seleciona os arquivos
3. O cliente envia os documentos
4. O sistema associa os documentos ao cliente
5. O sistema disponibiliza os documentos para revisão do contador
6. Continua no passo 7 do fluxo principal

---

## Tratamento de exceções

### 2a. Cliente não selecionado
- 2a.1 O sistema solicita a seleção de um cliente  
- 2a.2 Retorna ao passo 2  

### 4a. Nenhum arquivo selecionado
- 4a.1 O sistema solicita inclusão de pelo menos um arquivo  
- 4a.2 Retorna ao passo 4  

### 5a. Arquivo inválido (formato ou tamanho)
- 5a.1 O sistema informa erro no arquivo  
- 5a.2 O contador remove ou substitui o arquivo  
- 5a.3 Retorna ao passo 4  

### 7a. Arquivo XML ou JSON
- 7a.1 O sistema identifica que o arquivo é XML ou JSON
- 7a.2 O sistema importa os dados diretamente
- 7a.3 O processamento por OCR e IA é ignorado
- 7a.4 O sistema gera os dados para revisão do contador
- 7a.5 Continua no passo 9

### 8a. Falha no processamento da IA
- 8a.1 O sistema informa erro no processamento  
- 8a.2 O sistema permite nova tentativa  
- 8a.3 Retorna ao passo 7

### 11a. Contador rejeita o lançamento
- 11a.1 O sistema marca o lançamento como rejeitado  
- 11a.2 O sistema armazena o documento sem contabilização  
