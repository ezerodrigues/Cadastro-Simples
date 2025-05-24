# Cadastro Simples de Clientes

[![Python Version](https://img.shields.io/badge/python-3.12+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-^1.39.0-orange.svg)](https://streamlit.io/)
[![Pandas](https://img.shields.io/badge/Pandas-^2.2.3-yellowgreen.svg)](https://pandas.pydata.org/)
[![Poetry](https://img.shields.io/badge/Poetry-Managed-blueviolet.svg)](https://python-poetry.org/)

## Visão Geral

Bem-vindo ao **Cadastro Simples de Clientes**! Este projeto demonstra a criação de uma aplicação web interativa e funcional para o registro básico de informações de clientes, utilizando a simplicidade e o poder do Streamlit em conjunto com Pandas para manipulação de dados. Embora seja um sistema de cadastro elementar, ele serve como um excelente ponto de partida para entender os fundamentos do desenvolvimento web com Python e Streamlit, além de ser facilmente adaptável para necessidades mais complexas.

A aplicação oferece uma interface de usuário limpa e intuitiva, permitindo que os usuários insiram o nome, a data de nascimento e o tipo de cliente (Pessoa Física ou Jurídica). Os dados são então persistidos de forma organizada em um arquivo CSV (`clientes.csv`), ilustrando um fluxo básico de entrada e armazenamento de dados.

## ✨ Funcionalidades Principais

*   **Interface Intuitiva:** Formulário claro e direto para entrada de dados do cliente.
*   **Campos de Entrada:** Campos específicos para Nome, Data de Nascimento (com seletor de data) e Tipo de Cliente (com caixa de seleção).
*   **Validação Simples:** Verificação básica para garantir que os dados essenciais (nome e data) sejam fornecidos antes do cadastro.
*   **Persistência de Dados:** Salvamento automático das informações dos clientes em um arquivo `clientes.csv`, facilitando a consulta e o gerenciamento posterior.
*   **Feedback ao Usuário:** Mensagens de sucesso ou erro são exibidas após a tentativa de cadastro, informando o status da operação.
*   **Tecnologia Moderna:** Construído com Streamlit, permitindo a criação rápida de aplicações web de dados com Python puro.

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

*   **Python:** Versão 3.12 ou superior.
*   **Streamlit:** Framework principal para a criação da interface web interativa.
*   **Pandas:** Biblioteca utilizada para manipulação e armazenamento de dados, embora neste projeto seu uso seja implícito na forma como os dados poderiam ser lidos ou processados (o código atual usa escrita direta em CSV).
*   **Poetry:** Ferramenta para gerenciamento de dependências e ambientes virtuais, garantindo uma configuração de projeto organizada e reprodutível.

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter instalado em seu sistema:

*   [Python](https://www.python.org/downloads/) (versão 3.12 ou superior)
*   [Poetry](https://python-poetry.org/docs/#installation) (gerenciador de pacotes e dependências)

## 🚀 Instalação e Configuração

Siga os passos abaixo para configurar e executar o projeto em seu ambiente local:

1.  **Clone o Repositório:**
    ```bash
    git clone https://github.com/ezerodrigues/Cadastro-Simples.git
    ```

2.  **Navegue até o Diretório do Projeto:**
    ```bash
    cd Cadastro-Simples
    ```

3.  **Instale as Dependências:**
    Utilize o Poetry para instalar todas as dependências listadas no arquivo `pyproject.toml`.
    ```bash
    poetry install
    ```

4.  **Ative o Ambiente Virtual:**
    Para garantir que você está utilizando as dependências corretas, ative o ambiente virtual gerenciado pelo Poetry.
    ```bash
    poetry env activate
    ```
    *Observação: O comando pode variar ligeiramente dependendo do seu sistema operacional e shell. Consulte a documentação do Poetry se necessário.*

## ▶️ Executando a Aplicação

Com o ambiente virtual ativado e as dependências instaladas, você pode iniciar a aplicação Streamlit com o seguinte comando:

```bash
streamlit run app.py
```

A aplicação será aberta automaticamente no seu navegador padrão. Você verá a interface de cadastro pronta para uso.

## 📁 Estrutura de Arquivos

O projeto possui uma estrutura simples:

```
Cadastro-Simples/
│
├── .gitignore         # Arquivos e diretórios ignorados pelo Git
├── README.md          # Este arquivo que você está lendo
├── app.py             # Código principal da aplicação Streamlit
├── clientes.csv       # Arquivo onde os dados dos clientes são armazenados
├── poetry.lock        # Arquivo de lock do Poetry, garante instalações consistentes
└── pyproject.toml     # Arquivo de configuração do projeto e dependências (Poetry)
```

*   `app.py`: Contém toda a lógica da aplicação, incluindo a definição da interface do usuário com Streamlit e a função para salvar os dados.
*   `clientes.csv`: Armazena os dados dos clientes cadastrados. Cada linha representa um cliente com nome, data de nascimento e tipo.
*   `pyproject.toml`: Define as metadados do projeto e suas dependências para o Poetry.

## 📝 Como Usar

1.  Após iniciar a aplicação (`streamlit run app.py`), a interface de cadastro será exibida.
2.  Preencha o campo "Digite o nome do Cliente".
3.  Selecione a "Data de nascimento" utilizando o calendário interativo.
4.  Escolha o "Tipo do Cliente" entre "Pessoa Física" e "Pessoa Jurídica" na caixa de seleção.
5.  Clique no botão "Cadastrar".
6.  Uma mensagem de sucesso ("Cliente Cadastrado com Sucesso!") ou erro ("Houve algum problema no cadastro") será exibida abaixo do botão.
7.  Os dados do cliente cadastrado com sucesso serão adicionados ao final do arquivo `clientes.csv`.

## 🤝 Contribuições

Contribuições são bem-vindas! Se você tiver sugestões de melhorias, novas funcionalidades ou correções de bugs, sinta-se à vontade para abrir uma *Issue* ou enviar um *Pull Request*.

## 👨‍💻 Autor

**Eliézer Rodrigues**

- GitHub: [ezerodrigues](https://github.com/ezerodrigues)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

---

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!
