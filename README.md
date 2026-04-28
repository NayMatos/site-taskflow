TaskFlow - Gerenciador de Tarefas Colaborativo 📝

🌐 Demonstração Online
https://site-taskflow.web.app/

🚀 Sobre o Projeto

O TaskFlow é uma aplicação web para gerenciamento de tarefas no estilo Kanban, desenvolvida para ser totalmente colaborativa e em tempo real. A aplicação utiliza o Firebase Firestore como banco de dados, permitindo que qualquer alteração feita por um usuário seja refletida instantaneamente na tela de todos os outros.

Com uma interface moderna e focada no modo escuro, é a ferramenta ideal para organizar projetos pessoais ou gerenciar as atividades de pequenas equipes.

✨ Principais Funcionalidades

Quadro Kanban Interativo: Organize tarefas visualmente nas colunas "A Fazer", "Em Andamento" e "Concluído".

Sincronização em Tempo Real: Graças ao Firebase, as tarefas são atualizadas para todos os usuários sem a necessidade de recarregar a página.

Funcionalidade de Arrastar e Soltar (Drag and Drop): Mova as tarefas entre as colunas de forma fluida e intuitiva para atualizar seu status.

Interface em Modo Escuro: Design elegante e confortável para os olhos, focado em uma experiência de uso agradável.

Design Responsivo: A experiência de uso é otimizada para desktops, tablets e celulares.

CRUD Completo de Tarefas: Crie, leia, edite e exclua tarefas através de um modal simples e elegante.

🛠️ Tecnologias Utilizadas

Frontend:

HTML5

Tailwind CSS

JavaScript (ES6+)

Backend & Infraestrutura:

Firebase Firestore (Banco de Dados NoSQL em tempo real)

Firebase Authentication (Login anônimo)

Firebase Hosting (Hospedagem e Deploy)

📦 Como Executar

Para executar este projeto, você precisará configurar seu próprio ambiente no Firebase.

Clone o repositório:

git clone [https://github.com/NayMatos/site-taskflow.git](https://github.com/NayMatos/site-taskflow.git)

Crie um projeto no Firebase:

Acesse o Console do Firebase e crie um novo projeto.

Adicione um aplicativo da Web e copie o objeto de configuração firebaseConfig.

Configure o index.html:

Abra o arquivo index.html e substitua o objeto firebaseConfig de exemplo pelo que você copiou do seu projeto.

Habilite os serviços do Firebase:

Em Authentication, na aba "Sign-in method", habilite o provedor "Anônimo".

Em Firestore Database, crie um novo banco de dados no modo de teste.

Abra o arquivo index.html no seu navegador para usar a aplicação localmente.

🚀 Deploy com Firebase Hosting

O projeto está pronto para ser publicado na web.

Instale o Firebase CLI:

npm install -g firebase-tools

Faça o login e inicialize o projeto:

firebase login
firebase init

Durante a inicialização, escolha a opção "Hosting" e vincule ao projeto que você criou no Firebase.

Publique o site:

Mova o arquivo index.html para a pasta public criada pelo Firebase.

Execute o comando de deploy:

firebase deploy

👤 Autor e Licença

Atenção: Este projeto possui Todos os Direitos Reservados. A utilização, cópia ou modificação deste código por terceiros para fins comerciais ou criação de sites ativos não é permitida sem autorização expressa da autora.

Este projeto foi gerenciado, desenhado e desenvolvido por Nayara Matos.

➡ Acesse o portfólio ao vivo: https://naymatos.github.io/portfolio-nayara-matos/

📬 Contato
 * LinkedIn: linkedin.com/in/nayarasilvamatos
 * E-mail: nayarasmatos@gmail.com