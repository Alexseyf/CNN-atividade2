# 🧠 Reconhecimento de Emoções Humanas usando CNN

Projeto de Classificação de Emoções desenvolvido para a disciplina de Inteligência Artificial do curso de Análise e Desenvolvimento de Sistemas do UniSenac (5º Semestre, 2025). O sistema utiliza Redes Neurais Convolucionais (CNN) para classificar expressões faciais em seis categorias de emoções diferentes: raiva, nojo, medo, felicidade, tristeza e surpresa.

## 🎯 Objetivos

- Implementar uma CNN para classificação de emoções em imagens faciais
- Realizar pré-processamento e normalização das imagens
- Treinar e avaliar o modelo usando métricas de desempenho
- Criar visualizações para análise dos resultados

## 📋 Pré-requisitos

- Python 3.10 ou superior
- Git
- uv (gerenciador de pacotes e ambientes virtuais Python)
- GPU (recomendado para treinamento mais rápido)

## 🚀 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/Alexseyf/CNN-atividade2.git
cd atividade2
```

### 2. Instale o uv (caso ainda não tenha)

```bash
# Usando pip (qualquer sistema operacional)
pip install uv

# Ou usando curl (Linux/macOS)
curl -LsSf https://astral.sh/uv/install.sh | sh

# Ou usando PowerShell (Windows)
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 3. Configure o ambiente virtual

```bash
# Criar e ativar ambiente virtual
uv venv
source .venv/bin/activate  # Linux/macOS
# ou
.venv\Scripts\activate  # Windows
```

### 4. Instale as dependências

```bash
uv sync
```

O projeto utiliza o arquivo `pyproject.toml` para gerenciar suas dependências. O comando `uv sync` instalará automaticamente todas as dependências especificadas neste arquivo.

## 📥 Dataset e Pré-processamento

O dataset usado neste projeto contém imagens faciais classificadas em seis emoções diferentes. As imagens são pré-processadas através das seguintes etapas:

1. Redimensionamento para 64x64 pixels
2. Conversão para escala de cinza
3. Normalização dos valores dos pixels
4. Aumento de dados (data augmentation) para melhor generalização

O dataset completo está disponível para download através do seguinte link:
[Download Dataset](https://drive.google.com/drive/u/0/folders/1_4L4nw7XvlGiV3guMkyPaPVQgNC9_zmR)

**Nota Importante**: Este dataset é mantido apenas para fins acadêmicos. Após o download, o arquivo deve ser extraído na raiz do projeto, criando a pasta `data/` com as subpastas para cada emoção.

### Estrutura esperada após extração:
```
data/
├── angry/
├── disgust/
├── fear/
├── happy/
├── sad/
└── surprise/
```

## 🔬 Estrutura do Projeto

- `main.ipynb`: Notebook principal contendo todo o pipeline do projeto
- `data/`: Diretório contendo as imagens organizadas por emoção
  - `angry/`: Imagens de expressões de raiva
  - `disgust/`: Imagens de expressões de nojo
  - `fear/`: Imagens de expressões de medo
  - `happy/`: Imagens de expressões de felicidade
  - `sad/`: Imagens de expressões de tristeza
  - `surprise/`: Imagens de expressões de surpresa
- `pyproject.toml`: Arquivo de configuração do projeto e suas dependências
- `uv.lock`: Arquivo de lock para garantir versões consistentes das dependências

## 📚 Bibliotecas Principais

- **TensorFlow**: Framework principal para construção e treinamento da CNN
- **OpenCV**: Processamento e manipulação de imagens
- **NumPy**: Operações numéricas e manipulação de arrays
- **Pandas**: Análise e manipulação de dados
- **scikit-learn**: Métricas de avaliação e divisão de dados

## 📊 Métricas de Avaliação

O modelo é avaliado usando as seguintes métricas:
- Acurácia
- Matriz de Confusão
- Relatório de Classificação (Precisão, Recall, F1-Score)

## 👥 Autores

<div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
  <img src="https://avatars.githubusercontent.com/u/79027790?v=4" width="50" style="border-radius: 50%;">
  <a href="https://github.com/Alexseyf">Alexandre Seyffert</a>
</div>

<div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
  <img src="https://avatars.githubusercontent.com/u/140200421?v=4" width="50" style="border-radius: 50%;">
  <a href="https://github.com/JoaoAANgr">João Antônio</a>
</div>

<div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
  <img src="https://avatars.githubusercontent.com/u/173370106?v=4" width="50" style="border-radius: 50%;">
  <a href="https://github.com/OrtizLaura">Laura Ortiz</a>
</div>
<div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
  <img src="" width="50" style="border-radius: 50%;">
  <a href="https://github.com/">Henrique</a>
</div>

## 📄 Licença

Este projeto é para fins acadêmicos e educacionais.
