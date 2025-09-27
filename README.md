# Índice

* [Instalação](#-instalação)
* [Descrição](#descrição)
* [Funcionalidades](#funcionalidades)
* [Tecnologias Utilizadas](#-tecnologias-utilizadas)
* [Autor](#autor)
# MVP-Sistemas-Inteligentes

# 🎲 Instalação
Recomendado iniciar ambiente virtual antes da instalação das dependência/bibliotecas.

Para iniciar ambiente virtual no padrão do python utilizar:
```
python -m venv env
```
```
.\env\Scripts\activate
```
Após clonar o repositório, é necessário ir ao diretório API, pelo terminal e executar:
```
pip install -r requirements.txt
```
Este comando instala as dependências/bibliotecas, descritas no arquivo requirements.txt.

Para executar a API acessar o diretório "API" e executar:
```
flask run --host 0.0.0.0 --port 5000
```
Em modo de desenvolvimento é recomendado executar utilizando o parâmetro reload, que reiniciará o servidor automaticamente após uma mudança no código fonte.
```
flask run --host 0.0.0.0 --port 5000 --reload
```
Abra o http://localhost:5000/#/ no navegador para acessar a homepage da aplicação. 
Abra o http://localhost:5000/docs/ no navegador para verificar a documentação da API em execução

# Descrição
Aplicação desenvolvida como MVP para a Sprint: Sistemas Inteligentes.
Esta aplicação tem o objetivo de aplicar modelos de Machine Learning para determinar a personalidade de uma pessoa (podendo ser Introvertida ou Extrovertida) através de algumas perguntas, sendo elas:
- Horas passadas sozinho diariamente (0–11).
- Presença de medo de palco (Sim/Não).
- Frequência de participação em eventos sociais (0–10).
- Frequência com que sai de casa (0–7).
- Sensação de exaustão após socializar (Sim/Não).
- Número de amigos próximos (0–15).
- Frequência de postagens nas redes sociais (0–10).
- Variável alvo (Extrovertido/Introvertido).

Foram testados 4 modelos de ML sendo eles: 
- KNN
- Decision Tree
- Nayve Bayes
- Random Forest

E para avaliação foi utilizado o parâmetro de Acurácia, aonde o Random Forest (RF) se mostrou melhor, com 93,92% de acurácia.
O dataset utilizado foi retirado do site [Kagle](https://www.kagle.com/datasets/rakeshkapilavai/extrovert-vs-introvert-behavior-data)

# Funcionalidades
- [x] Cadastro de Usuário
- [x] Predição da personalidade (Introvertido/Extrovertido)

Após a Execução da API é possível acessar a documentação via Swagger e verificar/testar todas as funcionalidades da aplicação.
Abaixo segue todas as rotas da API
![rotas api](https://github.com/user-attachments/assets/f75eccdd-10c3-4d5f-991d-3cb3e9841f29)

E um exemplo de respostas possíveis
![respostas](https://github.com/user-attachments/assets/83de11f8-8158-467d-9c76-7dd9c1a2fea7)

Abaixo segue a homepage da aplicação
![homepage](https://github.com/user-attachments/assets/b6313fbc-93f1-420c-9ab4-0596b0607b5f)

Abaixo segue a tela para cadastro de usuário na aplicação
![modal](https://github.com/user-attachments/assets/473bde29-8952-4676-830b-91d0c8a5889f)


# 🛠 Tecnologias utilizadas
- [Python](https://www.python.org/)
- [Flask](https://flask.palletsprojects.com/en/stable/)
- [Pydantic](https://docs.pydantic.dev/latest/)
- [OpenAPI3](https://swagger.io/solutions/getting-started-with-oas/)

# Autor
---

<a href="https://github.com/MatheusPiaia">
 <img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/185968337?s=400&u=b4f54f3c5ea4b83b959d508547adf7077fd2caf8&v=4" width="100px;" alt=""/>
 <br/></a> 

 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/MatheusPiaia)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-Matheus-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/matheus-piaia-231647144)
