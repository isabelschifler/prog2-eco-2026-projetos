# [Amigo Fiel] – Equipe Isabel, Larissa, Suzana e Nathan

## Integrantes

| Nome | Matrícula | GitHub |
|------|-----------|--------|
| Isabel Schifler | 2024003899 | [@isabelschifler](https://github.com/isabelschifler) |
| Suzana Silveira | 2024002283 | [@SuzanaSilveira](https://github.com/SuzanaSilveira) |
| Larissa Damasceno | 2023009987 | [@lariiferraz](https://github.com/lariiferraz) |
| Nathan | 2023007991| [@Nathan](https://github.com/M1st3r2) |

---

## Descrição do projeto

O Amigo Fiel é uma plataforma web desenvolvida para facilitar e incentivar a adoção responsável de animais. O sistema conecta animais que aguardam por um lar a pessoas interessadas em adotar, promovendo transparência, segurança e eficiência no processo de adoção.

## ✨ Funcionalidades

### 👑 Para o Administrador

- ✅ Cadastrar, editar e gerenciar animais disponíveis para adoção
- ✅ Manter informações completas (nome, espécie, porte, idade, status)
- ✅ Gerenciar solicitações de adoção
- ✅ Entrar em contato com os usuários interessados

### 🐶 Para o Usuário (Adotante)

- ✅ Visualizar todos os animais cadastrados com detalhes
- ✅ Acessar informações completas de cada animal
- ✅ Realizar contato com os responsáveis por meio de mensagens internas
- ✅ Filtrar animais por espécie, porte e disponibilidade


## Modelagem do Sistema

Para representar o funcionamento do projeto Amigo Fiel, foram desenvolvidos diagramas UML que auxiliam na compreensão das funcionalidades e da estrutura do sistema. O diagrama de casos de uso apresenta as principais interações entre os atores e a plataforma. Nele, o ator Administrador possui responsabilidades como cadastrar conta, cadastrar animais, visualizar os animais cadastrados e editar ou excluir anúncios. Já o ator Usuário (adotante) pode definir preferências de busca, navegar entre os animais disponíveis e visualizar detalhes dos animais, além de entrar em contato com o responsável pelo anúncio. Essas funcionalidades representam o fluxo principal do sistema e demonstram como ocorre o processo de adoção dentro da plataforma.

Já o diagrama de classes representa a estrutura interna do sistema e os relacionamentos entre suas entidades principais: Administrador, Usuário, Animal e Contato. A classe Administrador é responsável pelo gerenciamento dos anúncios de adoção, enquanto a classe Usuário permite a navegação pelos animais disponíveis e a solicitação de adoção daqueles de seu interesse. A classe Animal armazena informações como nome, espécie, idade, porte, descrição, status e também poderá armazenar a imagem do animal. Por fim, a classe Contato gerencia a comunicação entre usuários interessados e responsáveis pelos animais. Essa modelagem contribui para uma melhor organização da aplicação e facilita futuras expansões e manutenções do sistema.


## Diagrama de Casos de Uso

![Diagrama de Casos de Uso](./Diagrama%20Caso%20de%20Uso.png)

## Diagrama de Classes

![Diagrama de Classes](./diagramadeclasse.png)

---

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (ES6+)
- Node.js
- Express.js
- SQLite
- Swagger (documentação da API)

As tecnologias escolhidas para o desenvolvimento do Amigo Fiel foram selecionadas por oferecerem praticidade, boa documentação e ampla utilização no desenvolvimento web. O JavaScript (ES6+) foi utilizado para implementar a lógica do sistema tanto no frontend quanto no backend. O HTML5 e o CSS3 foram escolhidos para estruturar e estilizar as páginas da aplicação, possibilitando a criação de uma interface intuitiva e responsiva. O Node.js foi utilizado como ambiente de execução do backend, permitindo o gerenciamento eficiente das requisições do sistema. Já o Express.js foi empregado para facilitar a criação da API REST e a organização das rotas da aplicação. O SQLite, juntamente com comandos SQL, foi definido para armazenar e gerenciar os dados de usuários, animais e contatos de forma segura e organizada. Além disso, o Swagger foi utilizado para documentar e testar os endpoints da API, contribuindo para a manutenção e validação das funcionalidades desenvolvidas.

## Como executar o projeto

```bash
# 1. Clone o repositório
git clone https://github.com/SuzanaSilveira/projeto-progII.git

# 2. Entre na pasta
cd projeto-progII

# 3. Instale as dependências
cd backend
npm install

# 4. Inicie o servidor
npm start

# 5. Acesse no navegador
# http://localhost:3000
---

## Estrutura de pastas

```
projeto-progII/
│
├── backend/
│   ├── package.json            
│   ├── package-lock.json      
│   ├── .env                   
│   │
│   └── src/
│       ├── server.js           
│       │
│       ├── controladores/     
│       │   ├── animalController.js
│       │   └── usuarioController.js
│       │   └── adminController.js
│       │   └── authController.js
│       │   └── solicitacaoController.js
│       │   └── uploadController.js
│       │
│       ├── rotas/              
│       │   ├── Animal.js
│       │   └── Usuario.js
│       │   └── adminRoutes.js
│       │   └── authRoutes.js
│       │   └── solicitacaoRoutes.js
│       │   └── uploadRoutes.js
│       │
│       ├── database/           
│       │   ├── database.js
│       │   └── amigofiel.db
│       │   └── solicitacao.js
│       │
│       ├── middleware/
│       │   ├── adminMiddleware.js
│       │   └── uploadConfig.js
│
├── frontend/
│       ├── css/           
│       │   ├── cadastro-animal.css
│       │   └── cadastro.css
│       │   └── detalhes-animal.css
│       │   └── home.css
│       │   └── index.css
│       │   └── interesses.css
│       │   └── login.css
│       │   └── style.css
│       │   └── tela-admin.css
│       │
│       ├── js/
│       │   ├── cadastro-animal.js
│       │   └── cadastro.js
│       │   └── detalhes-animal.js
│       │   └── home.css
│       │   └── index.js
│       │   └── interesses.js
│       │   └── login.js
│       │   └── tela-admin.js
│       │
│       ├── pages/
│       │   ├── cadastro-animal.html
│       │   └── cadastro.html
│       │   └── detalhes-animal.html
│       │   └── home.html 
│       │   └── index.html
│       │   └── interesses.html
│       │   └── login.html
│       │   └── tela-admin.html
│       │
├── uploads/
|
└── .gitignore                  
```

---

## Histórico de entregas

| Entrega | Descrição | Data | Status |
|---------|-----------|------|--------|
| E1 | Definição do projeto | 06/04/2026 | ✅  |
| E2 | Modelagem | 10/04/2026 | ✅ |
| E3 | Backend + BD | 15/04/2026 |  ✅ |
| E4 | Interface integrada | 15/06/2026 | ✅ |
| E5 | Projeto final | — | ✅ |

> ⏳ Pendente | ✅ Concluído | 🔄 Em andamento
