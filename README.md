
# OCR Text Extractor

Aplicativo desktop em Python para extrair texto de arquivos PDF e imagens escaneadas, com exportação para TXT, DOCX e PDF.

## Requisitos

- Python 3.7+
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) instalado e configurado no PATH
- [Poppler](https://poppler.freedesktop.org/) para conversão de PDF em imagem  
  - Windows: [poppler-windows](https://github.com/oschwartz10612/poppler-windows/releases/)
- Bibliotecas Python (instale com pip):

```bash
pip install pytesseract pdf2image pillow python-docx fpdf tkinterdnd2

````markdown
# OCR Text Extractor

Aplicativo desktop em Python para extrair texto de arquivos PDF e imagens escaneadas, com exportação para TXT, DOCX e PDF.

## Requisitos

- Python 3.7+
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) instalado e configurado no PATH
- [Poppler](https://poppler.freedesktop.org/) para conversão de PDF em imagem  
  - Windows: [poppler-windows](https://github.com/oschwartz10612/poppler-windows/releases/)
- Bibliotecas Python (instale com pip):

```bash
pip install pytesseract pdf2image pillow python-docx fpdf tkinterdnd2
````

## Como usar

1. Ajuste o caminho do executável do Tesseract no arquivo `ocr_avancado.py` (linha 7).
2. Execute o script:

```bash
python ocr_avancado.py
```

3. Arraste um arquivo PDF ou imagem para a janela do programa.
4. Visualize o texto extraído e exporte para TXT, DOCX ou PDF.

## Como rodar e testar no Windows

### 1. Instale o Python 3.7+ (se ainda não tiver)

* Baixe em: [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)
* Durante a instalação, **marque a opção “Add Python to PATH”**.

### 2. Instale o Tesseract OCR

* Baixe o instalador Windows:
  [https://github.com/tesseract-ocr/tesseract/releases/latest](https://github.com/tesseract-ocr/tesseract/releases/latest)
* Instale normalmente.
* Ajuste o caminho do executável no `ocr_avancado.py` se necessário (linha 7):

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

### 3. Instale o Poppler para Windows (para PDFs)

* Baixe aqui: [https://github.com/oschwartz10612/poppler-windows/releases/](https://github.com/oschwartz10612/poppler-windows/releases/)
* Descompacte em uma pasta, por exemplo `C:\poppler`.
* Adicione `C:\poppler\bin` ao PATH do Windows (variáveis de ambiente).

### 4. Instale as bibliotecas Python

Abra o prompt e rode:

```bash
pip install pytesseract pdf2image pillow python-docx fpdf tkinterdnd2
```

### 5. Crie a pasta de saída

Na pasta do projeto, crie:

```bash
mkdir documentos
```

### 6. Execute o programa

```bash
python ocr_avancado.py
```

### 7. Usando o programa

* Arraste arquivos PDF ou imagens para a janela.
* Veja o texto extraído na tela.
* Salve em TXT, DOCX ou PDF na pasta `documentos`.

### 8. Dicas finais

* Teste primeiro com arquivos simples.
* PDFs grandes demoram mais para processar.
* Ajuste o idioma no código alterando `IDIOMA` (`'por'` para português, `'eng'` para inglês).
* Verifique o caminho do Tesseract se der erro no OCR.

---

### Estrutura

* `ocr_avancado.py`: Código principal
* `documentos/`: Pasta onde os arquivos exportados serão salvos

---

### Licença

MIT License.


