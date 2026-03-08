# Atividade 1 — Filtro Sobel
**Tópicos para Computação 1 — 2026.1**  
Escola Superior de Tecnologia — UEA  
Profa. Dra. Elloá B. Guedes

---

## Sobre o projeto

Aplicação do filtro Sobel em imagens utilizando PyTorch, com o objetivo de ilustrar o processo de extração manual de características por meio de convolução. O notebook cobre:

- Abertura e visualização de imagens em escala de cinza
- Conversão para tensor PyTorch
- Implementação manual de convolução 2D com NumPy
- Cálculo da magnitude e orientação do gradiente
- Visualização comparativa dos resultados
- Construção de um vetor de características global

---

## Requisitos

- Python 3.13+
- [uv](https://docs.astral.sh/uv/) (gerenciador de projetos)

---

## Como executar com uv

### 1. Instale o uv (caso ainda não tenha)

**Linux/macOS:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows (PowerShell):**
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 2. Clone o repositório e entre na pasta

```bash
git clone <url-do-repositorio>
cd <nome-da-pasta>
```

### 3. Instale as dependências

```bash
uv sync
```

Isso lê o arquivo `pyproject.toml` e instala todas as bibliotecas necessárias automaticamente em um ambiente virtual isolado.

### 4. Execute o notebook

```bash
uv run jupyter notebook Topicos1-2026_1-Tarefa1.ipynb
```

---

## Como executar sem uv (pip)

Caso prefira não usar o uv, siga os passos abaixo com pip e venv.

### 1. Crie e ative um ambiente virtual

**Linux/macOS:**
```bash
python -m venv .venv
source .venv/bin/activate
```

**Windows:**
```bash
python -m venv .venv
.venv\Scripts\activate
```

### 2. Instale as dependências manualmente

```bash
pip install opencv-python matplotlib numpy torch jupyter
```

### 3. Execute o notebook

```bash
jupyter notebook Topicos1-2026_1-Tarefa1.ipynb
```

---

## Bibliotecas utilizadas

| Biblioteca | Uso |
|---|---|
| `opencv-python` | Leitura de imagens |
| `matplotlib` | Visualização |
| `numpy` | Operações matriciais |
| `torch` | Convolução com GPU/CPU via PyTorch |
| `jupyter` | Execução do notebook |

---

## Estrutura do projeto

```
.
├── Topicos1-2026_1-Tarefa1.ipynb   # Notebook principal
├── severance_group.jpg              # Imagem de exemplo
├── pyproject.toml                   # Configuração do projeto (uv)
└── README.md
```