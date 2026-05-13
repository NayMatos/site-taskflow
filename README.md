# TaskFlow - Gerenciador de Tarefas Colaborativo 📝

🌐 **Demonstração Online** [https://site-taskflow.web.app/](https://site-taskflow.web.app/)

## 🚀 Sobre o Projeto
O TaskFlow é uma aplicação web para gerenciamento de tarefas no estilo Kanban, desenvolvida para ser totalmente colaborativa e em tempo real. A aplicação utiliza o Firebase Firestore como banco de dados, permitindo que qualquer alteração feita por um usuário seja refletida instantaneamente na tela de todos os outros.

Com uma interface moderna e focada no modo escuro, é a ferramenta ideal para organizar projetos pessoais ou gerenciar as atividades de pequenas equipes.

## ✨ Principais Funcionalidades
* **Quadro Kanban Interativo:** Organize tarefas visualmente nas colunas "A Fazer", "Em Andamento" e "Concluído".
* **Sincronização em Tempo Real:** Graças ao Firebase, as tarefas são atualizadas para todos os usuários sem a necessidade de recarregar a página.
* **Funcionalidade de Arrastar e Soltar (Drag and Drop):** Mova as tarefas entre as colunas de forma fluida e intuitiva para atualizar seu status.
* **Interface em Modo Escuro:** Design elegante e confortável para os olhos, focado em uma experiência de uso agradável.
* **Design Responsivo:** A experiência de uso é otimizada para desktops, tablets e celulares.
* **CRUD Completo de Tarefas:** Crie, leia, edite e exclua tarefas através de um modal simples e elegante.

## 🛠️ Tecnologias Utilizadas
**Frontend:**
* HTML5
* Tailwind CSS
* JavaScript (ES6+)
* Polyfill (DragDropTouch) para compatibilidade nativa de arrastar e soltar em telas touch (celulares)

**Backend & Infraestrutura:**
* Firebase Firestore (Banco de Dados NoSQL em tempo real)
* Firebase Authentication (Login anônimo)
* Firebase Hosting (Hospedagem e Deploy)

## 📦 Como Executar
Para executar este projeto, você precisará configurar seu próprio ambiente no Firebase.

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/NayMatos/site-taskflow.git](https://github.com/NayMatos/site-taskflow.git)
   

2. **Crie um projeto no Firebase:**
   * Acesse o Console do Firebase e crie um novo projeto.
   * Adicione um aplicativo da Web e copie o objeto de configuração `firebaseConfig`.

3. **Configure o index.html:**
   * Abra o arquivo `index.html` e substitua o objeto `firebaseConfig` de exemplo pelo que você copiou do seu projeto.

4. **Habilite os serviços do Firebase:**
   * Em **Authentication**, na aba "Sign-in method", habilite o provedor "Anônimo".
   * Em **Firestore Database**, crie um novo banco de dados no **modo de produção** (recomendado usar a região `southamerica-east1` para menor latência). Em seguida, acesse a aba "Regras" e permita a leitura e gravação para a coleção de tarefas substituindo o código por:

   ```javascript
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       match /tasks/{taskId} {
         allow read, write: if true;
       }
     }
   }

5. **Execute localmente:**
   * Abra o arquivo `index.html` no seu navegador para usar a aplicação.

## 🚀 Deploy com Firebase Hosting
O projeto está pronto para ser publicado na web.

1. **Instale o Firebase CLI:**
   ```bash
   npm install -g firebase-tools
   

2. **Faça o login e inicialize o projeto:**
   ```bash
   firebase login
   firebase init
   
   *Durante a inicialização, escolha a opção "Hosting" e vincule ao projeto que você criou no Firebase.*

3. **Publique o site:**
   * Mova o arquivo `index.html` para a pasta `public` criada pelo Firebase.
   * Execute o comando de deploy:
   ```bash
   firebase deploy
   

## 👤 Autor e Licença
**Atenção:** Este projeto possui Todos os Direitos Reservados. A utilização, cópia ou modificação deste código por terceiros para fins comerciais ou criação de sites ativos não é permitida sem autorização expressa da autora.

Este projeto foi gerenciado, desenhado e desenvolvido por Nayara Matos, demonstrando precisão técnica e governança no ciclo de vida da aplicação.

➡ **Acesse o portfólio ao vivo:** [https://naymatos.github.io/portfolio-nayara-matos/](https://naymatos.github.io/portfolio-nayara-matos/)

## 📬 Contato
* **LinkedIn:** [linkedin.com/in/nayarasilvamatos](https://linkedin.com/in/nayarasilvamatos)
* **E-mail:** nayarasmatos@gmail.com