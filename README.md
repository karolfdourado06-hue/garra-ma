# GARRA Marília

Sistema web de apoio à gestão de animais, doações e adoções da ONG GARRA Marília, desenvolvido como parte do Projeto Integrador Extensionista de Análise e Desenvolvimento de Sistemas.

## Objetivo

A proposta é centralizar informações que atualmente podem ficar distribuídas em planilhas e registros manuais, facilitando a consulta dos dados dos animais, o acompanhamento das doações e a organização dos processos de adoção.

## Tecnologias

- Vite+ (comando `vp`)
- JavaScript, HTML e CSS (modelo Vanilla)
- Node.js
- Express
- dotenv
- Git e GitHub

## Requisitos

- Git
- Vite+ instalado e disponível pelo comando `vp`

## Como executar o projeto

1. Clone o repositório e entre na pasta:

   ```bash
   git clone https://github.com/SEU-USUARIO/garra-marilia.git
   cd garra-marilia
   ```

2. Instale as dependências:

   ```bash
   vp install
   ```

3. Copie `.env.example` para `.env` e confira a variável `PORT=3000`.

4. No primeiro terminal, inicie a API:

   ```bash
   vp run api
   ```

5. No segundo terminal, inicie o frontend:

   ```bash
   vp dev
   ```

6. Abra no navegador o endereço local informado pelo Vite+ (normalmente `http://localhost:5173`).

A página inicial consulta `GET /api/health` e apresenta o status retornado pela API.

## Rota da API

`GET /api/health`

Exemplo de resposta:

```json
{
  "status": "ok",
  "app": "GARRA Marília",
  "hora": "data e hora geradas pelo servidor"
}
```

## Estrutura inicial

```text
garra-marilia/
├── public/
├── server/
│   └── index.js
├── src/
│   ├── main.js
│   └── style.css
├── .env
├── .env.example
├── .gitignore
├── index.html
├── package.json
├── vite.config.ts
└── README.md
```

## Próximas etapas previstas

O esqueleto inicial será ampliado nas próximas etapas do projeto, incluindo cadastro e consulta de animais, registros de doações, cadastro de adotantes e acompanhamento das adoções, conforme o MVP definido para a ONG.
