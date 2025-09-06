# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas linguagens Python, JavaScript, TypeScript e Java, e gera relatórios `HTML` como [este](https://andrehora.github.io/gitevo-examples/python/pandas.html).

Mais exemplos de relatórios podem ser podem ser encontrados em https://github.com/andrehora/gitevo-examples.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

> [!NOTE]
> Antes de instalar a ferramenta, é recomendado criar e ativar um [ambiente virtual Python](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-and-use-virtual-environments).

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
$ pip install gitevo
```

Execute a ferramenta no repositório selecionado utilizando o comando abaixo (ajuste conforme a linguagem do repositório).
Substitua `<git_url>` pela URL do repositório que será analisado:

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r javascript <git_url>

# TypeScript
$ gitevo -r typescript <git_url>

# Java
$ gitevo -r java <git_url>
```

Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

> [!NOTE]
> Essa etapa pode demorar alguns minutos pois o projeto será clonado e analisado localmente.

# Passo 3: Explorar o relatório de evolução de código

Após executar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), é gerado um relatório `HTML` contendo diversos gráficos sobre a evolução do código.

Abra o relatório `HTML` e observe com atenção os gráficos.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo
- Detalhar se as curvas estão de acordo com boas práticas
- Explicar grandes alterações nas curvas
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- etc.

Seja criativo!

# Instruções para o exercício

1. Crie um `fork` deste repositório (mais informações sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Adicione o relatório `HTML` no seu fork.
3. No Moodle, submeta apenas a URL do seu `fork`.

Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork:

1. Repositório selecionado: https://github.com/TheAlgorithms/Java
2. Gráfico selecionado: <img width="975" height="487" alt="download (1)" src="https://github.com/user-attachments/assets/6f7de7e8-8672-4174-819b-18cb782c2d41" />
3. Explicação: O gráfico mostra a evolução da quantidade de arquivos de implementação e de testes ao longo do tempo, mais precisamente entre 2020 e 2025. A quantidade de arquivos com código de algoritmos em 2020 já é quase 200 e continua crescendo até 2025, o que mostra que o repositório cresceu ao longo do tempo. No entanto, a quantidade de arquivos de testes é 0 até 2022 e somente a partir deste ano testes começaram a ser criados, chegando à quase a mesma quantidade dos arquivos de implementação dos algoritmos. Por conta da natureza do repositório, que não é um sistema completo mas sim um lugar onde é possível encontrar algoritmos úteis com implementações em diferentes linguagens, talvez incialmente não havia a preocupação em realizar testes nos códigos. Porém, é possível ver que a mentalidade mudou a partir de 2022 e a quantidade de testes cresceu abruptamente. Idealmente, por mais simples que o código seja, é uma boa prática ter testes que permitam verificar se o código se comporta da maneira esperada. Dessa forma, essa mudança é importante e permite que seja mais fácil encontrar erros, verificar se mudanças feitas causaram problemas, entre outras coisas. Inicialmente o repositório não tinha testes, mas em 2025 há um alinhamento maior com as boas práticas no que diz respeito aos testes de software.



