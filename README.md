# Projeto Angular com Estrutura Modular

## Descrição do Projeto

Este projeto utiliza Angular para a construção de uma aplicação front-end com uma arquitetura modular e organizada. Ele também conta com um backend (definido no diretório `backend`) e um frontend que segue boas práticas de desenvolvimento com Angular, incluindo a separação de componentes, serviços e diretivas.

## Estrutura do Projeto

A estrutura principal do projeto é organizada da seguinte forma:

### Diretório `backend`
- **`package.json`**: Arquivo de configuração para o backend. Contém informações sobre dependências e scripts necessários para executar o backend.

### Diretório `frontend`
#### **`public`**
- Diretório para armazenar recursos estáticos, como imagens, fontes, ou outros arquivos acessíveis diretamente.

#### **`src`**
##### **`app`**
- **`app.component.html`**: Arquivo HTML principal do componente raiz da aplicação.
- **`app.component.ts`**: Arquivo TypeScript do componente raiz que gerencia a lógica principal da aplicação.
- **`app.config.server.ts`**: Configurações específicas para o ambiente do servidor.
- **`app.config.ts`**: Configurações gerais da aplicação.
- **`app.routes.server.ts`**: Definições de rotas específicas para o servidor.
- **`app.routes.ts`**: Arquivo com a definição das rotas da aplicação.

##### **`components`**
Contém os componentes organizados por funcionalidade:
- **`product`**: Gerenciamento de produtos.
  - **`product-create`**: Componente para criação de produtos.
  - **`product-delete`**: Componente para exclusão de produtos.
  - **`product-read`**: Componente para leitura/listagem de produtos.
  - **`product-update`**: Componente para atualização de produtos.
  - **`product.model.ts`**: Modelo para representar os dados dos produtos.
  - **`product.service.ts`**: Serviço para gerenciar a lógica e comunicação com APIs relacionadas a produtos.

##### **`directives`**
- **`red.directive.ts`**: Diretiva personalizada que aplica estilos ou comportamentos a elementos HTML.

##### **`views`**
Páginas principais da aplicação:
- **`home`**: Página inicial da aplicação.
- **`product-crud`**: Página para operações CRUD (Create, Read, Update, Delete) de produtos.

##### **`assets`**
- **`logo.png`**: Logotipo da aplicação.

## Tecnologias Utilizadas

- **Frontend**: Angular
  - Componentes, Diretivas, Rotas, e Serviços.
- **Backend**: Configurado no diretório `backend`, com dependências listadas no `package.json`.

## Instalação e Configuração

### Pré-requisitos
- Node.js e npm instalados na máquina.
- Angular CLI instalado globalmente.

### Passos
1. Clone o repositório:
   ```bash
   git clone https://github.com/VanderleiAlamino/rep-angular.git
   cd rep-angular
   ```

2. Instale as dependências do backend:
   ```bash
   cd backend
   npm install
   ```

3. Instale as dependências do frontend:
   ```bash
   cd frontend
   npm install
   ```

4. Execute o servidor de desenvolvimento:
   ```bash
   ng serve
   ```

5. Acesse a aplicação em:
   ```
   http://localhost:4200
   ```

## Funcionalidades

- **Home**: Página inicial da aplicação.
- **CRUD de Produtos**: Gerenciamento completo de produtos:
  - Criar, editar, excluir e listar produtos.
- **Estilização**: Diretivas personalizadas para aplicar estilos.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para enviar PRs (Pull Requests) ou abrir issues para relatar problemas ou sugerir melhorias.
