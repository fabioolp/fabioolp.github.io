# Fábio Oliveira — Site Pessoal

Site pessoal construído com [Jupyter Book](https://jupyterbook.org/).

## Estrutura

```text
myst.yml              Configuração do projeto e sumário (TOC)
style.css             CSS customizado
pages/                Páginas do site (index, about, research)
notebooks/            Notebooks Jupyter
.github/workflows/    Publicação automática
```

## Desenvolvimento

Instalar o Jupyter Book:

```bash
pip install "jupyter-book>=2"
```

Iniciar o servidor local de desenvolvimento:

```bash
jupyter book start
```

O site fica disponível em `http://localhost:3000`, com atualização automática ao salvar os arquivos.

## Build

```bash
jupyter book build --html
```

O resultado do build fica em `_build/html`.

## Publicação

O site é publicado automaticamente no GitHub Pages via GitHub Actions
(`.github/workflows/deploy.yml`), a cada push na branch `main`.

No GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

Site: <https://fabioolp.github.io/>
