# Projeto: Company Assets

## Descrição

Este projeto, chamado **Company Assets**, foi desenvolvido para otimizar o gerenciamento de ativos da empresa, utilizando diversas tecnologias modernas para garantir uma aplicação robusta, performática e de fácil manutenção.

## Ferramentas e Tecnologias Utilizadas

### 1. **AWS**
O deploy da aplicação foi feito utilizando o **AWS Amplify**, que facilita a implementação contínua e integrações com serviços AWS, além de automatizar o processo de CI/CD (Integração e Entrega Contínuas), garantindo uma pipeline de deploy confiável e eficiente.

A aplicação está disponível neste link: [Acessar aplicação](https://main.d2lkjvhvc510nq.amplifyapp.com/).

### 2. **Axios para Requests à API**
Utilizei o **Axios** para realizar as requisições à API. Ele proporciona uma interface mais simples para gerenciar requisições HTTP assíncronas, incluindo interceptação de respostas para tratamento de erros e configuração global de headers.

### 3. **Sass para Estilização**
A estilização do projeto foi feita com **Sass**, que facilita a modularização e manutenção dos estilos. Alguns dos benefícios incluem:

- **Mixins**: Reutilizo blocos de código CSS através de mixins, o que proporciona consistência e evita repetição de código.
- **Variáveis**: Garantem uma uniformidade visual em toda a aplicação, especialmente para cores e espaçamentos.

### 4. **Redux para Gerenciamento de Estado**
Implementei **Redux** para gerenciar o estado global da aplicação de maneira eficiente. Utilizei **Redux Thunk** para lidar com ações assíncronas, permitindo uma maior flexibilidade e abstração na lógica de interação com a API.

### 5. **Hook Personalizado de Debounce**
Criei um **hook personalizado de debounce** para otimizar as requisições à API, evitando chamadas excessivas enquanto o usuário digita. Isso melhora a performance e a experiência do usuário ao reduzir a carga de requisições desnecessárias.

### 6. **Conventional Commits**
Adotei o padrão de **Conventional Commits** para manter o histórico de commits claro e semântico. Isso facilita a rastreabilidade de mudanças e auxilia na geração automatizada de changelogs.

### 7. **Error Boundary**
Implementei uma classe **ErrorBoundary** para capturar erros que não são tratados por blocos `try/catch`, garantindo que a aplicação continue funcionando mesmo em cenários de erro inesperado.

### 8. **useMemo e useCallback para Melhorar a Performance**
Utilizei os hooks **useMemo** e **useCallback** para otimizar a renderização de componentes, evitando cálculos e recriações desnecessárias de funções em cada renderização. Isso melhora a performance, especialmente em componentes que realizam operações pesadas ou dependem de callbacks constantes.

### 9. **Husky com Commitlint e Lint-Staged**
Implementei o **Husky** para automatizar hooks do Git, como `pre-commit`, garantindo a execução de scripts de linting antes de cada commit. Além disso:

- **Commitlint**: Assegura que as mensagens de commit sigam o padrão **Conventional Commits**, garantindo consistência no histórico de commits.
- **Lint-Staged**: Faz o linting apenas dos arquivos modificados, melhorando a eficiência nas verificações de código.

### 10. **Paginação Customizada para Melhorar a Performance**
Implementei um sistema de paginação customizada para melhorar a performance nas requisições e na renderização de grandes volumes de dados. A paginação divide as requisições em blocos menores, permitindo que a API envie apenas as informações necessárias para cada página. Dessa forma, reduzo o tempo de carregamento e evito sobrecarregar a interface com dados desnecessários, otimizando a experiência do usuário.

### 11. **Yup com React Hook Form para Validação de Formulários**
Para garantir uma validação eficaz e simples dos formulários, utilizei o **Yup** em conjunto com o **React Hook Form**. Essa combinação permite:

- **Validação declarativa**: O Yup facilita a criação de esquemas de validação declarativos, o que torna o código mais legível e fácil de manter.
- **Melhoria na experiência do usuário**: O React Hook Form otimiza a performance de formulários ao evitar renderizações desnecessárias, garantindo uma experiência suave.
- **Feedback imediato ao usuário**: Com a integração do Yup, é possível fornecer mensagens de erro em tempo real, à medida que o usuário preenche os campos do formulário.

#### Credenciais de Acesso
Utilize as seguintes credenciais para acessar o sistema:

- **Email**: `tractian@admin.com`
- **Senha**: `admin`

## Instalação e Configuração
1. Clone o repositório: `git clone https://github.com/Sandross/company-assets.git`
2. Instale as dependências: `npm install`
3. Execute a aplicação: `npm run dev`

## Melhorias Futuras

### 1. **Testes Unitários com Jest**
Com mais tempo, eu adicionaria testes unitários utilizando **Jest** para garantir a qualidade do código e prevenir regressões. Isso ajudaria a identificar rapidamente possíveis falhas em funcionalidades críticas.

### 2. **Melhor Componentização**
Melhoraria a componentização do projeto, dividindo componentes grandes em unidades menores e mais reutilizáveis. Isso facilitaria a manutenção e o entendimento do código, além de melhorar a legibilidade e a escalabilidade da aplicação.

### 3. **Configurar um DNS Permanente**
Implementaria um **DNS permanente** para a aplicação, garantindo que o endereço seja mais amigável e fácil de memorizar. Isso também melhoraria a confiabilidade do acesso à aplicação, evitando possíveis problemas com links temporários.

### 4. **Aprimorar o Layout Mobile**
O layout mobile poderia ser refinado, garantindo uma melhor experiência do usuário em dispositivos móveis. Isso incluiria otimizações para diferentes tamanhos de tela e ajustes de design responsivo para garantir uma navegação mais fluida.

### 5. **Implementação do React Window para Renderização de Grandes Listas**
Para melhorar ainda mais a performance ao lidar com grandes volumes de dados, planejo implementar o React Window. Essa biblioteca permitirá a renderização apenas dos itens visíveis na tela, otimizando o uso de memória e reduzindo o tempo de carregamento, garantindo uma rolagem suave e uma experiência de usuário mais rápida e responsiva, mesmo com listas extensas.
