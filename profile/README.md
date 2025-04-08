## 1. Introdução

Neste projeto, propomos o desenvolvimento de uma plataforma web que conecta desenvolvedores e empresas, com o objetivo de facilitar:

- A publicação de vagas de trabalho
- O gerenciamento de projetos em andamento
- A comunicação entre as partes envolvidas
- O controle de perfil e pagamentos

A plataforma contará com funcionalidades como:

- Feed de vagas
- Acompanhamento de projetos
- Chat integrado
- Exibição e edição de perfis
- Sistema de pagamento via chave PIX
- Navegação por meio de uma barra global presente em todas as telas

---

## 2. Telas a Implementar

Definimos quatro telas principais no sistema:

- Feed de Propostas
- Projetos em Andamento
- Chat de Projetos
- Perfil do Usuário

Além disso, há componentes e subtelas associadas que complementam o funcionamento da aplicação.

### 2.1 Feed de Propostas

Tela principal onde desenvolvedores visualizam propostas de trabalho publicadas por empresas. Cada vaga é representada por um card com:

- Nome do publicador
- Valor da proposta
- Breve descrição
- Imagem (opcional)
- Botão para candidatura

Também contará com uma **barra de pesquisa** para filtrar as vagas por:

- Palavra-chave
- Categoria
- Valor da proposta

### 2.2 Projetos em Andamento

Apresenta os projetos em que o usuário está envolvido, seja como:

- Empresa contratante
- Desenvolvedor

Organização por:

- Data da última visualização
- Status (ativo, finalizado, pendente)

Permite acesso direto ao **chat do projeto**.

### 2.3 Chat de Projetos

Concentra as conversas entre empresas e desenvolvedores. Cada conversa está associada a um projeto.

A interface mostra:

- Nome e imagem do contato
- Título do projeto relacionado
- Envio e recebimento de mensagens em **tempo real**

### 2.4 Perfil do Usuário

Contém:

- Nome
- E-mail
- Telefone
- Redes sociais
- Biografia profissional
- Foto de perfil (com opção de edição)

A edição é feita via **modais acessíveis pela Navbar**.

### 2.5 Componentes e Subtelas

Além das telas principais, a plataforma terá componentes globais e subtelas que melhoram a experiência do usuário e a fluidez da navegação.

### 2.6 Navbar (Componente Global)

Presente em todas as telas da aplicação. Fornece:

- Acesso rápido ao Feed, Projetos e Perfil
- Valor atual da carteira do usuário
- Campo de pesquisa para facilitar a navegação

### 2.7 Subtelas/Modais da Navbar

- **Modal de Login**: Acesso à plataforma com e-mail e senha. Links para cadastro e recuperação de senha.
- **Modal de Esqueci minha Senha**: Envio de link de recuperação de senha via e-mail.
- **Modal de Edição de Perfil**: Alteração de dados pessoais, redes sociais, imagem e biografia.
- **Modal de Edição de Empresa**: Para usuários com empresa vinculada. Permite editar nome, CNPJ, endereço, logo e telefone.
- **Modal de Cadastro de Usuário**: Solicita nome, e-mail, CPF e senha. Possui checkbox para opção de cadastro de empresa.
- **Modal de Cadastro de Empresa**: Segunda etapa para quem optou por cadastrar uma empresa. Solicita dados da empresa.

### 2.8 Modal de Pagamento (Subtela)

Exibida ao final de um projeto, é responsável por formalizar a **transferência de valores** entre empresa e desenvolvedor.

Mostra:

- Dados da transação
- Identificação das partes
- Forma de pagamento (ex: chave PIX)
- Confirmação de que o valor será liberado após a finalização oficial da proposta pela empresa
