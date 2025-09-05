# Como instalar e executar o projeto

- As respostas das perguntas do item 2 e 3 do documento de especificação do desafio estão dentro do Jupyter Notebook na seção "Respostas da análise exploratória", assim como a previsão da nota do filme selecionado no item 4.

## Pré-requisitos

- [Python 3.8 ou superior](https://www.python.org/downloads/)
- pip (gerenciador de pacotes Python)
- [Git](https://www.python.org/downloads/) (opcional, para clonar o repositório)

## Instalação e Configuração

### 1. Clonar o repositório
```bash
git clone https://github.com/arthwho/IMDB-EDA
cd IMDB-EDA
```

### 2. É recomendável que um ambiente virtual seja criado ao lidar com projetos Python (apenas os pacotes necessários são instalados apenas naquele ambiente virtual. Isso evita a geração de conflitos de versões de forma global no seu computador). Para criar um ambiente virtual:
```bash
# Windows
python -m venv imdb_env

# Linux/Mac
python3 -m venv imdb_env
```

### 3. Ative o ambiente virtual:
```bash
# Windows
imdb_env\Scripts\activate

# Linux/Mac
source imdb_env/bin/activate
```

### 4. Instalar as dependências através do arquivo de dependências (para gerar um arquivo de dependências faça 'pip freeze > requirementes.txt'). Faça isso dentro do ambiente virtual.
```bash
pip install -r requirements.txt
```

## Executando o Projeto

### Opção 1: Jupyter Notebook no Navegador

#### 1. Ative o ambiente virtual (se não estiver ativo)
```bash
# Windows
imdb_env\Scripts\activate

# Linux/Mac
source imdb_env/bin/activate
```

#### 2. Inicie o Jupyter Notebook
```bash
jupyter notebook
```

#### 3. Abra o arquivo `pproductions.ipynb`
- Navegue até o arquivo no navegador
- Clique em `pproductions.ipynb`
- Execute as células na ordem

### Opção 2: VS Code (Como estou fazendo)

#### 1. [Instale o VS Code](https://code.visualstudio.com/)
- Instale as extensões Python e Jupyter

#### 2. Abra o projeto no VS Code (Clique com o botão direito no espaço vazio do diretório do projeto > clique em 'abrir no terminal'). No terminal digie:
```bash
code .
```

#### 3. Configure o interpretador Python
- Ative o ambiente virtual (se já não estiver ativo)
- Pressione `Ctrl + Shift + P`
- Digite "Python: Select Interpreter"
- Selecione o interpretador do seu ambiente virtual (`imdb_env`)

#### 4. Abra o notebook
- Clique em `pproductions.ipynb` no explorador de arquivos
- O VS Code abrirá o notebook com suporte completo ao Jupyter

#### 5. Execute as células
- Use `Shift + Enter` para executar uma célula
- Use `Ctrl + Enter` para executar sem mover para a próxima
- Use `Ctrl + Shift + Enter` para executar todas as células

## Dependências Principais

- **pandas**: Manipulação e análise de dados
- **numpy**: Computação numérica
- **matplotlib**: Visualizações e gráficos
- **seaborn**: Visualizações estatísticas avançadas
- **scikit-learn**: Machine learning
- **jupyter**: Ambiente de desenvolvimento interativo

## Solução de Problemas

### Erro de importação de matplotlib
```bash
pip install --upgrade matplotlib
```

### Erro de versão do numpy
```bash
pip install "numpy<2.1"
```

### Erro de permissão no Windows
Execute o PowerShell como Administrador

### Problemas no VS Code
- Verifique se o interpretador Python está correto
- Reinstale as extensões Python e Jupyter
- Reinicie o VS Code após instalar dependências

## Notas Importantes

- O arquivo `desafio_indicium_imdb.csv` deve estar na pasta `datasets/`
- Certifique-se de que o ambiente virtual está ativo antes de executar
- Algumas células podem demorar para executar dependendo do tamanho dos dados
- **VS Code**: Recomendado para desenvolvimento profissional e debugging
- **Jupyter no Navegador**: Ideal para apresentações e demonstrações

**Desenvolvido para o Desafio Indicium - Análise de Dados de Filmes IMDB**