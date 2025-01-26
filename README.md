# Projeto DsList 
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/wescaetano/dslist/blob/main/LICENSE) 
### Sobre o projeto:
 DsList é basicamente uma lista de jogos feita durante a semana do intensivão Java spring ministrada pelo Prof. Nelio Alves contendo informações dos jogos como: nome, avaliação, data de lançamento, categoria, resumo curto e longo.
 Nessa lista contendo vários jogos o usuário terá a opção de clicar em um jogo da lista para que assim informações mais completas desse jogo sejam mostradas.
 Uma funcionalidade interessante é que o usuário poderá clicar em um jogo que por exemplo esteja na primeira posição da lista e arrastalo para qualquer outra posição da mesma.

### Modelo Estrutural:
![Modelo Estrutural](https://github.com/wescaetano/dslist/blob/main/src/main/java/com/devsuperior/dslist/assets/dslist-model.png)

### Backend:
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- PostgreSQL

## Pré requisitos:
- Java 21
  
## Como usar:


1 - GET: /games/2 - Retorna um jogo específico no caso o jogo '2'
``` bash
{
    "id": 2,
    "title": "Red Dead Redemption 2",
    "year": 2018,
    "genre": "Role-playing (RPG), Adventure",
    "platforms": null,
    "score": 4.7,
    "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/2.png",
    "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!",
    "longDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa."
}
```

2 - GET: /lists - Retorna todas as listas por categoria
``` bash
{
        "id": 1,
        "name": "Aventura e RPG"
    },
    {
        "id": 2,
        "name": "Jogos de plataforma"
    }
```

3 - GET: /lists/2/games - Retorna todos os jogos no caso da lista '2'
``` bash
 {
        "id": 6,
        "title": "Super Mario World",
        "year": 1990,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/6.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 7,
        "title": "Hollow Knight",
        "year": 2017,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/7.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 8,
        "title": "Ori and the Blind Forest",
        "year": 2015,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/8.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 9,
        "title": "Cuphead",
        "year": 2017,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/9.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 10,
        "title": "Sonic CD",
        "year": 1993,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/10.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    }
```


4 - GET: /games - Retorna todos os jogos de todas as listas
``` bash
{
        "id": 1,
        "title": "Mass Effect Trilogy",
        "year": 2012,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/1.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 2,
        "title": "Red Dead Redemption 2",
        "year": 2018,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/2.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 3,
        "title": "The Witcher 3: Wild Hunt",
        "year": 2014,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/3.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 4,
        "title": "Sekiro: Shadows Die Twice",
        "year": 2019,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/4.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 5,
        "title": "Ghost of Tsushima",
        "year": 2012,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/5.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
    {
        "id": 6,
        "title": "Super Mario World",
        "year": 1990,
        "imgUrl": "https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/6.png",
        "shortDescription": "Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!"
    },
```
