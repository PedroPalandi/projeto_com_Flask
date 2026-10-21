# Projeto Flask com uv

## Guia rápido para configurar a aplicação usando o uv.

## Pré-requisitos

* Python: 3.10 ou superior
* uv: Gerenciador de pacotes Python


1. Instalar o uv (Windows)

*powershell -executionpolicy bypass -c "irm https://astral.sh/uv/install.ps1 | iex"*


## Comandos Úteis

- **Verificar versão do uv:** `uv --version`
- **Verificar versão do Python:** `python --version`


2. Inicializar o projeto

*uv init*
(Cria a estrutura inicial do projeto e o arquivo pyproject.toml)

3. Criar o ambiente virtual

*uv venv*


4. Instalar Dependências e Sincronizar
Na pasta do projeto, use:

*uv sync*
(Instala as dependências listadas no pyproject.toml e atualiza a .venv)

5. Template (templates/ola.html)

- Se nome for fornecido na URL: Exibe Olá, {nome}!.
- Se nome não for informado: Exibe Olá, Flask!.

6. Executar a aplicação

*uv run flask run*
(Inicia o servidor de desenvolvimento do Flask usando o ambiente virtual gerenciado pelo uv)