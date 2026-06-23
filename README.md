# Hands-on Machine Learning — 3ª edição

Notebooks de estudo e exercícios do livro *Hands-on Machine Learning with Scikit-Learn, Keras & TensorFlow* (3ª edição), de Aurélien Géron.

Este repositório é uma reorganização do projeto original [ageron/handson-ml3](https://github.com/ageron/handson-ml3). O conteúdo didático e os créditos permanecem com seus autores e colaboradores originais.

## Comece por aqui

- [Índice dos notebooks](notebooks/index.ipynb)
- [Instruções detalhadas de instalação](docs/INSTALL.md)
- [Checklist de projetos de Machine Learning](docs/ml-project-checklist.md)
- [Equações do livro](docs/book_equations.pdf)
- [Execução com Docker](docker/README.md)

## Estrutura do repositório

```text
.
├── notebooks/          # capítulos, tutoriais, extras e imagens
│   ├── index.ipynb     # ponto de entrada para os estudos
│   └── images/         # imagens usadas e geradas pelos notebooks
├── docs/               # instalação e material de referência
├── docker/             # ambiente conteinerizado (CPU e GPU)
├── environment.yml     # ambiente Conda recomendado
├── requirements.txt    # alternativa de instalação com pip
└── apt.txt             # dependências de sistema
```

Os datasets baixados durante a execução ficam em `notebooks/datasets/` e não são versionados.

## Instalação rápida

```bash
git clone https://github.com/andreluizpedroso/handson-ml3.git
cd handson-ml3
conda env create -f environment.yml
conda activate homl3
python -m ipykernel install --user --name=python3
jupyter notebook notebooks/index.ipynb
```

Como alternativa ao Conda:

```bash
python -m venv .venv
# Linux/macOS: source .venv/bin/activate
# Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
jupyter notebook notebooks/index.ipynb
```

## Organização dos notebooks

- `01_...` a `19_...`: capítulos do livro, em ordem.
- `tools_...`: introduções a NumPy, pandas e Matplotlib.
- `math_...`: fundamentos matemáticos.
- `extra_...`: materiais complementares.
- `index.ipynb`: índice navegável de todo o conteúdo.

## Licença e créditos

Consulte [LICENSE](LICENSE). Para o histórico completo de colaboradores e o projeto canônico, visite [ageron/handson-ml3](https://github.com/ageron/handson-ml3).
