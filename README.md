# Calor vs Humor 

A base de dados trata de uma pesquisa com o tema *"Calor vs Humor"*, que analisa como a percepção do calor pode influenciar o humor das pessoas.

## Preparando o ambiente de execução

```markdown
📁 Projeto Ciência de Dados
├── 📁 src
│   └── 📁 dataset
├── 📄 computacao_aplicada.ipynb
├── 📄 README.md
└── 📄 requirements.txt
```
Como visto no esquema acima, o dataset, em formato *scv*, pode ser encontrado em [./src/dataset](./src/dataset). A execução do arquivo jupyter notebook depende desse arquivo, o que o torna importante na execução. Além deste, pode-se encontrar o arquivo requirements.txt necessário para a instalação de todas as bibliotecas utilizada no projeto.

### Configurando o ambiente de execução

Para configurar o ambiente de execução do código deste repositório, é necessário ter o python na versão igual ou superior a 3.13, além de ter o gerenciador de pacotes do python instalado (pip).

Logo em seguida, utilize o comando `python -m venv venv` para criar um ambiente de execução específico para esta aplicação. Para executar este ambiente, utilize o comando `.\venv\Scripts\activate` pelo próprio terminal ou powershel do windows. Em qualquer momento você pode desativar esse ambiente utilizando o comando `.\venv\Scripts\deactivate`.

> **Lembrando que o usuário deve estar na pasta raiz.**

Com o ambiente de execução devidamente configurado, o próximo passo é instalar as bibliotecas utilizadas no projeto e para isso basta usar o comando `pip intall -r requirements.txt` na raiz deste repositório. Todas as bibliotecas, como numpy, matplotlib, seaborn e outros, serão instalada.
