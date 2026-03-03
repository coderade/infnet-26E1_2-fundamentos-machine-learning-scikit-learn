# infnet-26E1_2-fundamentos-machine-learning-scikit-learn

## Pré-requisitos

1. **Python 3.11+** instalado no sistema
2. **uv** (gerenciador de pacotes) — [instalação](https://docs.astral.sh/uv/getting-started/installation/)

## Configuração do Ambiente

### Usando uv (recomendado)

```bash
# Criar ambiente virtual
uv venv .venv

# Ativar ambiente virtual
# No macOS/Linux:
source .venv/bin/activate
# No Windows:
.venv\Scripts\activate

# Instalar dependências
uv pip install -r requirements.txt
```

### Registrar kernel no Jupyter

```bash
.venv/bin/python -m ipykernel install --user --name=ml-heart-disease --display-name="Python (ML Heart Disease)"
```

## Dataset

O dataset é carregado automaticamente pelo notebook via URL do UCI Machine Learning Repository — não é necessário baixar nada manualmente.

## Execução

1. **Iniciar Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Abrir o arquivo:** `projeto_ml_heart_disease.ipynb`

3. **Selecionar o kernel:** `Kernel → Change Kernel → Python (ML Heart Disease)`

4. **Executar todas as células:** `Cell → Run All`

## Estrutura dos Arquivos

```
projeto/
├── projeto_ml_heart_disease.ipynb  # Notebook principal
├── requirements.txt                # Dependências
├── actividade.md                   # Descrição da atividade
├── avaliacao.md                    # Critérios de avaliação
└── README.md                       # Este arquivo
```

## Troubleshooting

- **Erro de importação:** Verifique se o ambiente virtual está ativo e as dependências instaladas
- **Kernel não aparece:** Reinicie o Jupyter após registrar o kernel
- **NameError entre células:** Execute todas as células em ordem (`Kernel → Restart & Run All`)
- **Erro de conexão no dataset:** Verifique sua conexão com a internet (o CSV é baixado da UCI)
