<h1>Azure - Machine Learning</h1>
<p align="center">
Exercício de aprendizado de Máquinas utilizando o AI Search para indexação e consulta de dados
</p>

## 📎 Ferramentas Utilizadas
- Azure AI Search
- Azure AI Search resource
- Storage account

## Sobre o Processo
<p>Para utilizarmos o AI Search para filtrar os resultos será necessário utilizarmos 3 ferramentas já citadas acima, o processo consiste em criar um serviço de IA, fazer um link com a automação do processo e direcionar pra um repositório. Para alimentar nosso Storage Account eu optei por utilizar os arquivos já fornecidos na própria documentação.</p>
<p>Após já alimentado o nosso Container é hora de começarmos a utilizar o serviço de busca, nesse processo podemos observar que temos um retono no formado JSON, e que o conceito de busca é baseado em <strong>Palavras Chaves</strong>, por exemplo estamos trabalhando com um modelo de cafeteria tendo vários pontos localizados, durante a configuração da nossa IA deixamos habilitado a opção de buscar por sentimento, na qual podemos buscar um sentimento negativo e teremos retorno de todos comentário, para facilitar a explicação deixarei alguns exemplos de busca e retorno abaixo</p>

## Modelo de Busca
```
{
 "search": "locations:'Chicago'",
 "count": true
}
```

## Saída de Dados
```
"keyphrases": [
        "new drink theme",
        "seasonal baked goods",
        "coffee tastings",
        "local music",
        "Fourth Coffee",
        "rising artists",
        "Review",
        "afternoon",
        "spot",
        "advance",
        "weekdays",
        "slice",
        "pie",
        "Date",
        "August",
        "Location",
        "Chicago",
        "Illinois"
      ],
      "language": "en",
```

<p>Na saída de dados podemos foi retirado apenas um trecho do retorno, porém nossa IA fez uma busca de tudo que está relacionado a palavra chave que no caso foi Chicago, nossa IA consegue trazer informações positivas, negativas, neutras, datas, localizações dentre outras coisas. Processo para otimização de buscas e o mais interessante, todas as informações fornecidas são dentro do portal Azure. Em estudo de caso podemos perceber que quando temos diversos arquivos e precisamos localizar apenas alguma palavre chave essa ferramente consegue nos auxiliar, deixando claro os seguintes pontos:
</p>

- Retorna dados Estruturados
- Busca por interesse e relacionamentos
- Busca por palavras chaves e capacidade de resumo

<p>Como todo recurso de IA antes de começar a utilizar o medelo precisa ser treinado, no portal do Azure já temos alguns modelos de exemplo que podem ser adaptados conforme a necessidade do cliente.</p>