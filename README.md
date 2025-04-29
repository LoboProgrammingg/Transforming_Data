# Transformação de Dados - CSV para Markdown

Este repositório contém dois scripts para transformar arquivos CSV em arquivos Markdown (.md). Ele é dividido em duas partes: 
1. Processamento local de arquivos CSV.
2. Processamento de arquivos armazenados no Google Drive.

## 📂 Estrutura do Repositório

```plaintext
Transformação de Dados/
│
├── CSV TO MD LOCAL/
│   ├── transforming_csv_to_md_doc_local.py  # Script para transformar arquivos CSV locais
│
├── Google Drive/
│   ├── transforming_csv_to_md_google.py     # Script para transformar arquivos do Google Drive
│   ├── client_secrets.json                  # Configuração para autenticação no Google Drive
│
├── documentation/
│   ├── dados.csv                            # Arquivo CSV de exemplo
│   ├── dados.xlsx                           # Arquivo XLSX de exemplo
│   ├── dados.md                             # Arquivo Markdown gerado
│
└── README.md
```

---

## 🛠️ Funcionalidades

### **1. CSV TO MD LOCAL**
- Transforma arquivos CSV armazenados localmente em arquivos Markdown.
- Local do script: `CSV TO MD LOCAL/transforming_csv_to_md_doc_local.py`.

### **2. Google Drive**
- Faz o download de arquivos XLSX do Google Drive.
- Converte os arquivos XLSX para CSV.
- Transforma o CSV em Markdown.
- Local do script: `Google Drive/transforming_csv_to_md_google.py`.

---

## 🏁 Como Usar

### **1. CSV TO MD LOCAL**
1. Coloque o arquivo CSV no diretório `documentation/`.
2. Execute o script:
   ```bash
   python CSV\ TO\ MD\ LOCAL/transforming_csv_to_md_doc_local.py
   ```
3. O arquivo Markdown será gerado no mesmo diretório (`documentation/dados.md`).

---

### **2. Google Drive**
#### Pré-requisitos:
1. Configure a API do Google Drive:
    - Baixe o arquivo `client_secrets.json` do Google Cloud Console.
    - Coloque o arquivo em `Google Drive/`.
2. Instale as dependências:
   ```bash
   pip install pandas pydrive openpyxl
   ```

#### Execução:
1. Substitua `SEU_ARQUIVO_ID_AQUI` no script `transforming_csv_to_md_google.py` com o ID do arquivo no Google Drive.
2. Execute o script:
   ```bash
   python Google\ Drive/transforming_csv_to_md_google.py
   ```
3. O arquivo Markdown será gerado no diretório `documentation/`.

---

## 🌟 Agradecimentos

Obrigado por conferir este projeto! Se você gostou, deixe uma estrela no repositório.