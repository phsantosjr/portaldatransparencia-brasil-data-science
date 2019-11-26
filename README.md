## Portal da Transparência - Brasil - Estudo ##

Esse projeto é para estudo das bibliotecas de Data Science do Python

### Fazer download das bases ? ###

#### Bolsa Família ####

Acessar o Portal da Transparência (http://www.portaltransparencia.gov.br/download-de-dados), ir ao item 
Benefícios ao Cidadão --> Bolsa Família Pagamentos.

Fazer o download do arquivo do mês que deseja analisar, salvá-lo na pasta bases.

O nome do arquivo deve ser alterado para carga:

```
df = pd.read_csv("bases/201910_BolsaFamilia_Pagamentos.csv", encoding ='latin1', engine='python', 
                 quotechar='"', delimiter=";", decimal=",", nrows=10000)
```

O parâmetro nrows da carga é para limitar o volume de informaçoẽs a subir pro DataFrame.


#### Militares remuneração ####

Acessar o Portal da Transparência (http://www.portaltransparencia.gov.br/download-de-dados), ir ao item
Servidores --> Servidores civis e militares do Executivo Federal

Fazer o download do arquivo do mês que deseja analisar, salvá-lo na pasta bases.

O nome do arquivo deve ser alterado para carga:

```
df = pd.read_csv('bases/201901_RemuneracaoMilitares.csv', encoding ='latin1', 
                 engine='python', quotechar='"', delimiter=";", decimal=',')
```

### Criar virtualenv ###

* Ambiente Linux

```
mkvirtualenv --python=/usr/bin/python3.6 data-science
```


### Executar Jupyter ###

Abra um terminal, ative o virtualenv e execute o comando.
```
jupyter notebook
```

Aguarde o browser abrir o Jupyter.


### Autor ###

PH

### Referências ###

* [VirtualEnv Wrapper](https://virtualenvwrapper.readthedocs.io/en/latest/)


### Outros projetos interessantes ###

https://github.com/fmasanori/CursoPyLadiesSP