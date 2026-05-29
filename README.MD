# 🗂️ Automação de Organização de Arquivos

Este projeto tem como objetivo **organizar automaticamente arquivos em pastas** de acordo com suas extensões (por exemplo, imagens e PDFs).  
Ele utiliza a biblioteca **tkinter** para permitir que o usuário selecione uma pasta e a biblioteca **os** para manipular arquivos e diretórios.

---

## 🚀 Funcionalidades

- Seleciona uma pasta através de uma janela gráfica.  
- Cria subpastas automaticamente conforme o tipo de arquivo.  
- Move arquivos para suas respectivas pastas:
  - Imagens (`.png`, `.jpg`)
  - PDFs (`.pdf`)

---

## 🧠 Como funciona

1. O programa solicita ao usuário que escolha uma pasta.  
2. Ele lista todos os arquivos dentro dessa pasta.  
3. Para cada arquivo, verifica sua extensão.  
4. Se a extensão corresponder a uma das categorias definidas:
   - Cria a pasta correspondente (caso não exista).
   - Move o arquivo para dentro dessa pasta.

---

## 🧩 Estrutura do código

- **tkinter.filedialog.askdirectory** → abre a janela para seleção da pasta.  
- **os.listdir()** → lista os arquivos da pasta escolhida.  
- **os.path.splitext()** → separa o nome e a extensão do arquivo.  
- **os.mkdir()** → cria pastas conforme necessário.  
- **os.rename()** → move os arquivos para suas novas localizações.

---

## 💻 Como executar

1. Certifique-se de ter o **Python 3** instalado.  
2. Salve o código em um arquivo chamado `main.py`.  
3. Execute o script:

```bash

python main.py

```

## 📦 Exemplo de resultado

**Antes:**
```bash
/Documentos
├── foto1.png
├── foto2.jpg
└── arquivo.pdf
```

# Depois

 /Documentos 
├── imagens/
│   ├── foto1.png
│   └── foto2.jpg
└── pdfs/
    └── arquivo.pdf