# Trilha Elixir

Elixir é uma linguagem compilada, compila para Erlang e roda na VM do Erlang. 

## Comandos

- Setup

  ```bash
  wget https://packages.erlang-solutions.com/erlang-solutions_2.0_all.deb && sudo dpkg -i erlang-solutions_2.0_all.deb
  sudo apt-get update
  sudo apt-get install esl-erlang
  sudo apt-get install elixir

  # Install Phoenix
  mix archive.install hex phx_new 1.5.7
  # Create project template "rocketpay"
  mix phx.new rocketpay --no-webpack --no-html
  ```

- Developing

  ```bash
  # Baixa todas as dependências da nossa aplicação
  mix deps.get

  # Verifica conexão com o banco de dados 
  mix ecto.setup

  # Setup Credo (analisador sintático de código)
  mix credogen.config

  # Run project
  mix phx.server
  ```
