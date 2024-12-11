# Javalirica

## Descrição

Este projeto visa desenvolver um sistema de gerenciamento de biblioteca física utilizando a metodologia ágil e práticas de DevOps integradas ao GitHub. A arquitetura do software seguirá o padrão Model-View-Controller (MVC) e incorporará o(s) padrõe(s) de projeto Factory para garantir uma base de código robusta e escalável. O desenvolvimento será feito na linguagem Java.

## Índice

1. [Objetivos do Projeto](#objetivo)
2. [Definições, Acrônimos e Abreviações](#definição)
3. [Requisitos](#requisitos)
   1. [Requisitos Funcionais](#rf)
   2. [Requisitos Não Funcionais](#rnf)
4. [Diagramas UML](#uml)
   1. [Diagrama de Casos de Uso](#uc)
   2. [Diagrama de Classe](#classe)
5. [Estrutura do Projeto](#estrutura)
6. [Contribuição](#contribuição)
7. [Licença](#licença)
8. [Contato](#contato)

## Definições, Acrônimos e Abreviações.
HTML (HyperText Markup Language) - Linguagem de marcação utilizada para estruturar e apresentar o conteúdo na web.

CSS (Cascading Style Sheets) - Linguagem de estilo utilizada para definir a aparência e o layout dos elementos HTML.

JS (JavaScript) - Linguagem de programação que permite implementar funcionalidades interativas em páginas web.

CRUD (Create, Read, Update, Delete) - Operações fundamentais para manipulação de dados, permitindo criação, leitura, atualização e exclusão de registros.

UI (User Interface) - Interface do Usuário, ou o conjunto de elementos visuais com os quais o usuário interage.

UX (User Experience) - Experiência do Usuário, o aspecto geral de como o usuário se sente ao interagir com o sistema.

ID de Livro - Identificador único atribuído a cada livro no sistema para facilitar seu rastreamento.

Aluguel de Livro - Ação de emprestar temporariamente um livro para um usuário registrado, com condições de devolução definidas.

Biblioteca Digital - Repositório digital onde os livros são armazenados e organizados para consulta e aluguel online.

Controle de Aluguel - Função que registra e monitora o status de cada livro alugado, incluindo informações de locação e devolução.

## Requisitos ou História de Usuário

   ### Requisitos Funcionais

1 - Listar Livro

2 - Cadastrar Livro

3 - Buscar por nome

4 - Atualizar Estoque

5 - Realizar locação

6 - Listar Locações

7 - Buscar por CPF do Leitor

8 - Registrar Devolução

9 - Listar Usuários

10 - Buscar por Nome

11 - Criar Novo Usuário

12 - Alterar Senha

13 - Listar Leitores

14 - Cadastrar Leitor

15 - Bloquear Leitor

16 - Desbloquear Leitor

   ### Requisitos Não Funcionais
1 - Usabilidade: O sistema deve ser intuitivo e fácil de usar, com interfaces claras e acessíveis para o bibliotecário e os clientes.

2 - Desempenho: O sistema deve ser capaz de realizar operações de busca e cadastro rapidamente, mesmo com um grande volume de livros e clientes cadastrados.

3 - Segurança: O sistema deve garantir que as informações pessoais dos clientes (como nome, endereço, telefone e e-mail) estejam protegidas com criptografia e com acesso restrito.

4 - Backup: O sistema deve ser capaz de realizar backups regulares dos dados para evitar a perda de informações importantes.

5 - Escalabilidade: O sistema deve ser projetado de forma a permitir sua expansão no futuro, como aumento de número de livros, clientes e funcionalidades.

6 - Compatibilidade: O sistema deve ser compatível com diferentes sistemas operacionais, como Windows, Linux e macOS.

7 - Disponibilidade: O sistema deve estar disponível 24 horas por dia, 7 dias por semana, com baixa possibilidade de falhas ou interrupções.

8 - Manutenibilidade: O código-fonte do sistema deve ser bem estruturado e documentado, facilitando a manutenção e a adição de novas funcionalidades.

9 - Atualizações: O sistema deve permitir atualizações periódicas e seguras para melhorar funcionalidades e corrigir problemas de segurança

10 - Consistência de dados: O sistema deve garantir que as informações no banco de dados sejam consistentes, especialmente ao realizar operações como empréstimos e devoluções.

11 - Responsividade: A interface do sistema deve ser responsiva, se adaptando adequadamente a diferentes tamanhos de tela (por exemplo, desktop e dispositivos móveis).

12 - Internacionalização: O sistema deve ser desenvolvido de forma a permitir fácil tradução para outros idiomas no futuro.

13 - Logs de auditoria: O sistema deve manter logs de auditoria detalhados, registrando todas as operações feitas pelo bibliotecário, como cadastro, edição e exclusão de livros, empréstimos e devoluções.

## Diagramas UML   
   
   ### Diagrama de Casos de Uso
Atores:

A) Bibliotecário: Responsável pelo gerenciamento dos livros, estoques e locações.

B) Leitor: Usuário do sistema que poderá consultar informações sobre livros e seu próprio histórico de empréstimos.

C) Administrador do Sistema: Responsável pelo controle de acesso e segurança do sistema.

Casos de Uso:

1 - Adicionar Livro – Bibliotecário adiciona um novo livro ao sistema.

2 - Remover Livro – Bibliotecário remove um livro do sistema.

3 - Listar Livro – Bibliotecário ou Leitor pode visualizar a lista de livros disponíveis.

4 - Locar Livro – Bibliotecário ou Leitor realiza a locação de um livro.

5 - Pesquisar Livro – Bibliotecário ou Leitor pesquisa um livro específico.

6 - Consultar Disponibilidade – Leitor consulta a disponibilidade de um livro.

7 - Verificar Livros em Empréstimos – Bibliotecário consulta os livros atualmente emprestados.

8 - Verificar Leitores Ativos – Bibliotecário verifica quais leitores estão com livros emprestados.

9 - Cadastrar Leitores – Bibliotecário registra novos leitores no sistema.

10 - Excluir Leitores – Bibliotecário remove leitores do sistema.

11 - Controlar Acesso de Usuário – Administrador gerencia os acessos dos usuários ao sistema

![Diagrama de caso de uso](https://github.com/user-attachments/assets/abbfc86f-bfdd-47e4-b805-02c8cecd1155)


   
   ### Diagrama de Classe
   
   ![ERD de hóquei1](https://github.com/user-attachments/assets/4dcc2ab7-c3ec-4cff-9bfe-9a7522b7f0db)



## Estrutura do Projeto 
<Comentario: faça a adaptação necessária para o seu projeto
- `src/`: Código-fonte do projeto.
- `docs/`: Documentação adicional.

## Tecnologias Utilizadas
- JAVA
- Maven
- Spring - security
- Spring - dataJpa
- Spring - Email
- Spring - Validation
- jjwt
- H2
- HTML
- CSS
- JS

## Instruções de Instalação
1. Clone o repositório:
   ```sh
   git clone https://github.com/Javalirica/back-end.git

   além do clone no github o servidor se encontra rodando em um serviço ec2 na aws no caminho http://3.141.87.82:8080

2. Clone do repositório Font-End
   ```sh
   https://github.com/Javalirica/front-end
   
## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo <LICENSE> para mais detalhes.
## Contato
![Marco Thulio Martins - marcothulio120799@mail.com](https://github.com/user-attachments/assets/1169905f-00b1-44de-bd49-eab2a20774c2) 
Marco Thulio Martins - marcothulio120799@mail.com

![Leonardo Gabriel Silva - Leonardogabrielsilva1@outlook.com ](https://github.com/user-attachments/assets/45223d9f-4c4a-4214-8ee0-1238e606c73a) 
Leonardo Gabriel Silva - Leonardogabrielsilva1@outlook.com

![Guilherme Procópio - guilhermeviniciusgv42@gmail.com ](https://github.com/user-attachments/assets/383ade1c-e589-48be-909f-1dbcce80a0db) 
Guilherme Procópio - guilhermeviniciusgv42@gmail.com

![Breno Jesus Andrade - ](https://github.com/user-attachments/assets/ee06874f-c54a-4fe9-9ec3-302688b38d69)
Breno Jesus - Breno.jesus33@hotmail.com

![Pedro Rodrigues - pedrodejesus2001@gmail.com](https://github.com/user-attachments/assets/cf8bde2f-edef-4c9b-9612-aa9a4aa848ec)
Pedro Rodrigues - pedrodejesus2001@gmail.com

