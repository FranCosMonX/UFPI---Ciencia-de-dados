# Calor vs Humor 

A base de dados trata de uma pesquisa com o tema *"Calor vs Humor"*, que analisa como a percepção do calor pode influenciar o humor das pessoas.

## Preparando o ambiente de execução

```markdown
📁 Projeto Ciência de Dados
├── 📁 src
│   └── 📁 dataset
|   └── 📁 graficos
|   └── 📁 tabelas
├── 📄 computacao_aplicada.ipynb
├── 📄 README.md
└── 📄 requirements.txt
```
Como visto no esquema acima, o dataset, em formato *"csv"*, pode ser encontrado em [./src/dataset](./src/dataset). Os gráficos vistos neste README são carregados automaticamente após executar o arquivo *"computacao_Aplicada.ipynb"* e estes podem ser encontrados em [./src/graficos](./src/graficos/). A pasta *"tabelas"* não é atualizada após a execução do arquivo. A execução do arquivo jupyter notebook depende desse arquivo, o que o torna importante na execução. Além deste, pode-se encontrar o arquivo *"requirements.txt"* necessário para a instalação de todas as bibliotecas utilizada no projeto.

### Configurando o ambiente de execução

Para configurar o ambiente de execução do código deste repositório, é necessário ter o python na versão igual ou superior a 3.13, além de ter o gerenciador de pacotes do python instalado (pip).

Logo em seguida, utilize o comando `python -m venv venv` para criar um ambiente de execução específico para esta aplicação. Para executar este ambiente, utilize o comando `.\venv\Scripts\activate` pelo próprio terminal ou powershel do windows. Em qualquer momento você pode desativar esse ambiente utilizando o comando `.\venv\Scripts\deactivate`.

> **Lembrando que o usuário deve estar na pasta raiz.**

Com o ambiente de execução devidamente configurado, o próximo passo é instalar as bibliotecas utilizadas no projeto e para isso basta usar o comando `pip intall -r requirements.txt` na raiz deste repositório. Todas as bibliotecas, como numpy, matplotlib, seaborn e outros, serão instalada.

# Metodologias Utilizadas

1. [Pré-processamento de dados (datageeks)](https://www.datageeks.com.br/pre-processamento-de-dados/): limpando dados ausentes.
<div align="center"> 
<img src="./src/tabelas/preprocessamentoDados.png" alt="tabela que mostra que o dataset não tem dados faltantes ou nulos."/>
<p>Figura 1: Resultado do pré processamento de dados</p>
</div>

> Vale ressaltar que o dataset não prevê dados duplicados, uma vez que não está sendo coletado dados sensíveis comumentes usados para identificar unicamente uma pessoa.

<div align="center"> 
<img src="./src/tabelas/tipoColunas.png" alt="tabela que mostra o tipo de cada coluna do dataset"/>
<p>Figura 2: Tipo das colunas</p>
</div>

    Como visto na figura 2, o dataset é cheio de dados categóricos para facilitar na tomada de decisão sem haver complexidade adicional.

2. [Análise exploratória de dados (IBM)](https://www.ibm.com/br-pt/think/topics/exploratory-data-analysis)

# Efetuando análises

Antes de começar a analisar as respostas, vale a pena analisar a frequencia com que as pessoas responderam o formulario.

<div align="center"> 
<img src="./src/graficos/numero_de_resposta_por_dia.png" alt="grafico que mostra a quantidade de respostas coletadas por dia."/>
<p>Figura 3: Quantidade de respostas coletadas por dia.</p>
</div>

## Sobre o Formulário

O formulario (Google Forms) tinha 10 questões objetivas. Este foi amplamente divulgado em grupos de alunos, eventos vinculados à UFPI e, também, em redes de contatos pessoais dos participantes. Como resultado, foi gerado um dataset de 132 respostas com 11 colunas (a data em que a pessoa respondeu o questionário e as questões). Posteriormente foi acrescentado as colunas de Temperatura Minima e Máxima em °C. Tais perguntas são:
1. Como você se sentiu hoje?
2. Você saiu de casa hoje?
3. Se sim, em qual período?
4. O calor influenciou sua decisão de sair ou ficar em casa?
5. O que você fez para se refrescar hoje?(Marque todas as que se aplicam)
6. O calor influenciou sua alimentação hoje?
7. Quantos copos de água (aproximadamente) você tomou hoje?
8. Como você avaliaria sua produtividade hoje?
9. Você acha que o calor afetou seu humor hoje?
10. De 0 a 10, qual nota você daria para o "calor de hoje"?

## Análise exploratória com foco em motivação

Esse estudo é importante para descobrir se a temperatura afeta negativamente o cotidiano das pessoas. Sendo assim, é avaliado o bem estar da pessoa juntamente com a ação de sair para fazer algo do cotidiano.

<div align="center"> 
<img src="./src/graficos/distribuicao_resposta_1.png" alt="grafico que mostra como a pessoa está se sentindo: multo bem/mal, mal/bem ou neutro"/>
<p>Figura 4: Bem estar pessoal.</p>
</div>

<div align="center"> 
<img src="./src/graficos/distribuicao_resposta_2.png" alt="grafico que mostra a relação de pessoas que sairam ou não de suas casas no dia em que responderam o formulário"/>
<p>Figura 5: Relação entre as pessoas que sairam e que não sairam de casa</p>
</div>

<div align="center"> 
<img src="./src/graficos/relacaoDeSentirVsInfluenciaDoCalor.png" alt="grafico que mostra a influência do calor sob o humor das pessoas"/>
<p>Figura 6: Influência do calor sob o humor</p>
</div>

Com as 3 imagens dá para notar que as pessoas não deixam de fazer suas atividades cotidianas devido ao calor, mesmo ele influênciando seu humor.