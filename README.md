Notebooks de Machine Learning, 3ª edição
=========================================

Este projeto tem como objetivo ensinar os fundamentos de Machine Learning em
Python. Ele contém os códigos de exemplo e as soluções dos exercícios da terceira edição do livro [Hands-on Machine Learning with Scikit-Learn, Keras and TensorFlow](https://homl.info/er3), de Aurélien Géron:

<a href="https://homl.info/er3"><img src="https://learning.oreilly.com/library/cover/9781098125967/300w/" title="livro" width="150" border="0" /></a>

**Observação**: se você procura os notebooks da segunda edição, acesse [ageron/handson-ml2](https://github.com/ageron/handson-ml2). Para a primeira edição, consulte [ageron/handson-ml](https://github.com/ageron/handson-ml).

## Estrutura do repositório

Os notebooks e suas imagens estão em [`notebooks/`](notebooks/), a documentação complementar está em [`docs/`](docs/) e a configuração do Docker permanece em [`docker/`](docker/). Comece por [`notebooks/index.ipynb`](notebooks/index.ipynb).

## Início rápido

### Quer experimentar os notebooks online sem instalar nada?

* <a href="https://colab.research.google.com/github/andreluizpedroso/handson-ml3/blob/main/notebooks/index.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Abrir no Colab"/></a> (recomendado)

⚠ _O Colab oferece um ambiente temporário: tudo o que você fizer será apagado após algum tempo. Baixe os dados que deseja preservar._

<details>

Outros serviços também podem funcionar, embora não tenham sido totalmente testados:

* <a href="https://homl.info/kaggle3/"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Abrir no Kaggle" /></a>

* <a href="https://mybinder.org/v2/gh/andreluizpedroso/handson-ml3/HEAD?filepath=%2Fnotebooks%2Findex.ipynb"><img src="https://mybinder.org/badge_logo.svg" alt="Abrir no Binder" /></a>

* <a href="https://homl.info/deepnote3/"><img src="https://deepnote.com/buttons/launch-in-deepnote-small.svg" alt="Abrir no Deepnote" /></a>

</details>

### Quer apenas visualizar os notebooks sem executar o código?

* <a href="https://nbviewer.jupyter.org/github/andreluizpedroso/handson-ml3/blob/main/notebooks/index.ipynb"><img src="https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg" alt="Visualizar no nbviewer" /></a>

* O [visualizador de notebooks do GitHub](https://github.com/andreluizpedroso/handson-ml3/blob/main/notebooks/index.ipynb) também funciona, mas não é a opção ideal: ele é mais lento, nem sempre exibe corretamente as equações matemáticas e costuma falhar ao abrir notebooks grandes.

### Quer executar o projeto usando uma imagem Docker?

Leia as [instruções do Docker](docker/README.md).

### Quer instalar o projeto em sua máquina?

Comece instalando o [Anaconda](https://www.anaconda.com/products/distribution/) (ou o [Miniconda](https://docs.conda.io/en/latest/miniconda.html)), o [Git](https://git-scm.com/downloads) e, caso tenha uma GPU compatível com o TensorFlow, instale o [driver da GPU](https://www.nvidia.com/Download/index.aspx), além das versões apropriadas do CUDA e do cuDNN. Consulte a documentação do TensorFlow para mais detalhes.

Em seguida, clone este projeto abrindo um terminal e executando os comandos abaixo. Não digite os primeiros sinais de `$`; eles apenas representam o prompt do terminal:

    $ git clone https://github.com/andreluizpedroso/handson-ml3.git
    $ cd handson-ml3

Depois, execute:

    $ conda env create -f environment.yml
    $ conda activate homl3
    $ python -m ipykernel install --user --name=python3

Por fim, inicie o Jupyter:

    $ jupyter notebook notebooks/index.ipynb

Se precisar de mais orientações, leia as [instruções detalhadas de instalação](docs/INSTALL.md).

# Perguntas frequentes

**Qual versão do Python devo usar?**

Recomenda-se o Python 3.10. Seguindo as instruções de instalação acima, essa será a versão utilizada. Qualquer versão igual ou superior à 3.7 também deve funcionar.

**Estou recebendo um erro ao chamar `load_housing_data()`**

Se o erro for relacionado a HTTP, confirme que está executando exatamente o mesmo código do notebook — copie e cole o trecho, se necessário. Caso o problema persista, verifique sua conexão de rede. Se for um erro de SSL, consulte a próxima pergunta.

**Estou recebendo um erro de SSL no macOS**

Provavelmente é necessário instalar os certificados SSL. Consulte esta [pergunta no Stack Overflow](https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error). Se você baixou o Python pelo site oficial, execute `/Applications/Python\ 3.10/Install\ Certificates.command` no terminal, substituindo `3.10` pela versão instalada. Caso tenha usado o MacPorts, execute `sudo port install curl-ca-bundle`.

**Como atualizo este projeto para a versão mais recente?**

Consulte [docs/INSTALL.md](docs/INSTALL.md).

**Como atualizo as bibliotecas Python para as versões mais recentes usando o Anaconda?**

Consulte [docs/INSTALL.md](docs/INSTALL.md).

## Colaboradores

Agradecemos a todas as pessoas que [contribuíram com o projeto original](https://github.com/ageron/handson-ml3/graphs/contributors), seja enviando feedback, abrindo issues ou submetendo Pull Requests. Um agradecimento especial a Haesun Park e Ian Beauregard, que revisaram todos os notebooks e enviaram diversos PRs, incluindo melhorias nas soluções dos exercícios. Agradecemos também a Steven Bunkley e Ziembla, responsáveis pelo diretório `docker`; ao usuário SuperYorio, pelas contribuições em algumas soluções; e a Victor Khaustov, pelas muitas correções enviadas. Por fim, agradecemos à equipe Google ML Developer Programs pelo apoio com créditos do Google Cloud.
