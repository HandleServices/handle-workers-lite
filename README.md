# Handle Web Workers

![Handle-Workers](./docs/images/Handle_Banner1.png)

A Handle é um aplicativo destinado a auxiliar novos universitários que ingressam em universidades fora de sua região e carecem de uma rede de apoio local. O propósito é que por meio dessa plataforma, os estudantes possam acessar e contratar uma variedade de serviços locais, como montagem de móveis, serviços elétricos, encanamento, entre outros. O aplicativo permitirá que os usuários analisem disponibilidade, preços e avaliações prévias dos profissionais, proporcionando segurança, confiabilidade e conforto a esses estudantes que enfrentam essa nova realidade.

Ademais, objetiva-se por proporcionar aos prestadores de serviço em questão, além de um aumento na prospecção de clientes, um suporte da plataforma ao gerenciamento efetivo e organizado da sua prestação de serviços. Assim, será possível gerar novas oportunidade de renda aos prestadores e incentivar a economia local.

---

## 📝 [Documentação](./docs)

Aqui, você encontrará documentos essenciais que fornecem informações sobre a visão, escopo e requisitos do nosso projeto.

[Documentação Requisitos, Visão e Escopo](./docs/Documentação%20Requisitos,%20Visão%20e%20Escopo.docx.pdf)

---

## 📂 Estrutura do Projeto

```bash
.
├── back-app
│   └── repo
│       ├── handle-api
│       └── handle-auth-service
├── docs
│   └── images
└── web-app
    └── repo
        └── handle-workers
```

O projeto é dividido em duas partes: `back-app` e `web-app`. A primeira é responsável por toda a parte de backend da aplicação, enquanto a segunda é responsável por toda a parte de frontend.

- Back-app: Contém os repositórios dos serviços `handle-api` e `handle-auth-service`.
- Web-app: Contém o repositório das aplicações web `handle-workers`.

## 📦 Submódulos

Este repositório incorpora a funcionalidade de submódulos do GitHub para gerenciar dependências externas de forma organizada e eficiente.

Para clonar este repositório juntamente com todos os seus submódulos, utilize o seguinte comando:

```bash
git clone --recursive git@github.com:HandleServices/handle-workers-lite.git
```

Se preferir clonar apenas o repositório principal e posteriormente inicializar seus submódulos, empregue o seguinte comando:

```bash
git clone git@github.com:HandleServices/handle-workers-lite.git
```

Após realizar a clonagem do repositório, a inicialização de todos os submódulos pode ser realizada por meio do seguinte comando:

```bash
git submodule update --init --recursive
```

Caso deseje iniciar somente um submódulo específico, utilize o comando a seguir, especificando o caminho para o repositório desejado:

```bash
git submodule update --init path/to/repository
```

Para atualizar o repositório principal juntamente com seus submódulos, empregue o comando abaixo:

```bash
git pull --recurse-submodule
```

Estas orientações fornecem uma abordagem estruturada para gerenciar os submódulos neste projeto, otimizando a integração de dependências externas.

## 🚀 Tecnologias

### Front-end

[![react](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactjs.org/)
[![typescript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![nextjs](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)](https://nextjs.org/)
[![axios](https://img.shields.io/badge/-Axios-56A7F7?style=flat-square&logo=axios&logoColor=white)](https://axios-http.com/)
[![react-query](https://img.shields.io/badge/-React_Query-000000?style=flat-square&logo=react-query&logoColor=white)](https://react-query.tanstack.com/)
[![tailwindcss](https://img.shields.io/badge/-Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

### Back-end

[![python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org/)
[![fastapi](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![pydantic](https://img.shields.io/badge/-Pydantic-333?style=flat-square&logo=python&logoColor=white)](https://docs.pydantic.dev/latest/)
[![sqlalchemy](https://img.shields.io/badge/-SQLAlchemy-333?style=flat-square&logo=sqlalchemy&logoColor=white)](https://www.sqlalchemy.org/)
[![gloe](https://img.shields.io/badge/Gloe-gray?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAP8AAADOAgMAAACMQDxRAAAACVBMVEUAAAAA18cA2MXxw+UeAAAAA3RSTlMA/4Md4+s2AAAGsklEQVR4nO2bPXIjNxCF16pyYOY+wgarU/AICkSWrIjlSNYpZGc+AHMnqrJ5Svd7/YuZoagBVOaWSwhW0gD4ptHobnSD3C9LbXN8fFnseG973e0eRubf7Ha7/YgI3wSwOwwAjgAMrAErkDVcEfATAbt+LX79IED/NnATPgDQv48y+XEEgF28EymGAAdR5H0v4AcBbMUWui0JdvQyDBAxxgCiiOsBfjTA7roAmOP1Ab0BQQHiDJ+AT8B3APgunGk0oAyHtE/ABwC6T2cC5GwcA8j51p1g/I8Ad2snno77vypgbaL5D9LDAMg/KwG3kWATIGneOsCN5rcVsF0FYJmkb3XAqphqAvQDrEjh1hHw80qAVJotYOWxoGVWC1gVDnwF3QBfQSoxAd/m9nDzuvt7eQUJyHhynDsVjJZWP1nB6cvJDemPcMbNfC18X4PVOs+lagELBkGja6p72XRzpDlADeL2VIar0VXV8EksCoDfIxxI3wFC5/hNblhdUwhAwJ8+gxUY1pGasMK2KIE6zDc0APQdKGKs2dym6JZI6eceBEC9mQCK6G/wPZ8A5M+NLQMAsSyloe9AEV3ksNrcBsgk3R6EGgD6UIW+BXABZRgHGSDhWwJcZNNh0RoBgnNVA+CuoH0Z7gy5bwCQCcMrwF/IGyXTuwFoM1RNBUB2PHRfcF9in+k9DWPP52FJmBhxIACqMw5sAPq6GSDceAJgH8r5mKCWhUdhim5mLHkDoMO5LBxzcSGhC4VQFwAqMPwUHdjJcwDVyhmAwKkxnBOqVj55DyAM8R4PcNjqxs4BoY8FgI6TB+gkwGZWgJvBBJAXOlj2JQAX3ADSEBlO2FnkxQ+3A4w/B1D4VzM93yoZDYCbcph1A0hD3BKAGQUQYhcXOAd4aQAm72WALlCtGwBoA50m72WA9moflAgAoiSeyE+M8RSI1voGgP82AA0+EdLUtKYA7dUY4wBA8boVABmuAF4LFQAc0OYvAyyCah98wQHmujGpC1Ac8CzA7JzOSHeeA2o8yQB6DrAtAHldOCCa/D4HmJFoIENIawFNVJ/YbdM7B+jiLwNsjwPA0J6AOO43khfNALbVCRdH4uESAB4UHPAqtAD4uZDZRIafFuCHIf48JMBFXwLsGwBGcg5zpxkgLfkMgLUBdYjFzQB+2peALRMk76M3AsAUgyNYHIYdmPIKwO0lAbRhZtYLAFs7j9IZ4NdCRwvrf0hfMEAKGEYti/tlAoidLwCbWACu7QTYSe95LY9cB5RUaQrIj308RTNfbgC+9gLAopYBmcrfNemBR6sCgIJt5U7PzFw27hCm729OAOcVgBcGGY2YyrtrGkAHJ4BjCcVvlmg/LQHszQXARRHAF1teUaoVPSxM1T5R1RRJswI81zUdenGk5x190yc2ANVYyCLa0PIwahONIOx8sj4ehA7IDNfqNL1jyHAKEV12lIIcrXrGmNw8Y51sD+NE0JMvq06O1tcW8+EhHDl+AzAbtK1RgOt58qlhVBk1b/fjpQG4t8h+1k8NGzGngCoe8mK2J78UyRQwmx0JnqbUTqS0Uq5Io8bgxGkIXJs7WDmBXLzfAIBeck2IQzQE8wGZyxIvLT33iLUiARyjDZGQgSiYFLEottRhDLaYkQCtlvRw0/aov9IWYXqZGIja8ANSaJ2p+mOJ9hI3HHLZpgt+1luIkgbIMMzDSOYCpm0K80yFPpyOj+JF1vmsTNsPFPRPFIThKQDuGU2dWc0mHp6OUnib5HZ6N/5brKe16uZywwbLssyGJO4UC/Sx1Wza6xXrkSw5/TABMbZadXvBYwAsixriXsWKc2xRQnMXVL81QMNh77xWL2uYXBBphz68fd1r4Fu4bsg1eHBuANN7KxM472hSqukXRUo4ffvLCHYPNBUg4nLb7AsZzWO1wtk3VfIcaRqNon2Z3ObNtsAB86u7G/Ea8Z2mbU67U3shGICly+SFsYutpCZ9LfPPzhb5Z2+L/LOzlQSzr3G/RwAluepqJbXpa8uesKKp1w0Amhu7jlbzma5WAmJfG/4alYW+6wE8VHcDoEOmOL0A6JApzgCAKU43ALnVCIA55yiAuVUvgHOvCmDlMAi4HwJILq0X7r0AXvcMAg5DAB5qAwC9ohkEbEcBmmxfC6DX1gOArMKvCcj7xE/AwC74ner1APppRFdTU24+nf6PARpQ9OOMAUB8TtB5tjYfOqxtuHrBjcQIgK273vBidhgwlKR9BKC/6LM8c6Dom38zZGUbrlfOlP4rGtYwvZFY1aTsHPq/M3JJcJrdSLyv/Qv8VEqXgVcthAAAAABJRU5ErkJggg==&style=flat-square
)](https://gloe.ideos.com.br/)

[![nodejs](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)](https://nodejs.org/)
[![nestjs](https://img.shields.io/badge/-NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)](https://nestjs.com/)
[![jwt](https://img.shields.io/badge/-JWT-000000?style=flat-square&logo=json-web-tokens&logoColor=white)](https://jwt.io)

[![postgresql](https://img.shields.io/badge/-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)](https://postgresql.org)
[![docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://docker.com)
[![docker-compose](https://img.shields.io/badge/-Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white)](https://docs.docker.com/compose/)

## 👥 Integrantes

- Elpidio Cabral - [@ElpidioCabral](https://github.com/elpidiocabral)
- Gabriel Al-Samir - [@GuimaraesSl](https://github.com/GuimaraesSl)
- José Souza - [@JoseEdSouza](http://github.com/JoseEdSouza)
- Mariana Hofer - [@Hofeerr](http://github.com/hofeerr)
- Luigy Gabriel - [@Dev-Luigy](http://github.com/Dev-Luigy)
