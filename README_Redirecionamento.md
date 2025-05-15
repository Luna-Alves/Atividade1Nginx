## Tutorial Passo a passo da correção do redirecionamento de páginas em uma aplicação ReactJs provida pelo Nginx.

### Passo 1 -Instalação e configuração do Nginx:
#### O Nginx é um servidor web que possui uma arquitetura orientada a eventos e modelos assíncronos. Por isso, ele é muito útil para o gerenciamento de conexões simultâneas consumindo pouca memória e CPU. Ele atua como servidor HTTP para uma entrega rápida de arquivos estáticos e é utilizado como proxy reverso, intermediando requisições entre clientes e servidores de aplicação. 
#### Nesse tutorial, estou utilizando o WSL2 com Ubuntu rodando no Windows. Por isso, iniciei fazendo a atualização da lista de pacotes com o comando "sudo apt update":
![image](https://github.com/user-attachments/assets/57771ed9-a051-498c-a7b8-5bb4afa066a2)

#### Em seguida, fiz a instalação do Nginx, comando "sudo apt install nginx":
![image](https://github.com/user-attachments/assets/07f83208-cb5a-4cde-bb7d-8cb469cff3c2)

#### Verificação da versão instalada:

![image](https://github.com/user-attachments/assets/0836cf7c-4b0e-4ef5-ba5c-fe06eff09ecc)

#### Inicialização e habilitação do Nginx com verificação de status:
![image](https://github.com/user-attachments/assets/de51a42c-3481-4993-aba9-d988f25844bb)

### Passo 2 - Configuração do bloco de servidor para a minha aplicação React:
#### Abertura do arquivo com o Nano:

![image](https://github.com/user-attachments/assets/d6964563-1607-4678-9888-97819eec6014)

#### Configuração do server:

![image](https://github.com/user-attachments/assets/a7c7d0c1-af90-4f75-b023-21c900612237)

#### Comandos Ctrl+O + Enter para gravar e comando Ctrl+X para voltar ao cmd:

![image](https://github.com/user-attachments/assets/27341374-926f-4f3a-a72f-412d1b4e6450)

#### O próximo passo é a habilitação do host:
![image](https://github.com/user-attachments/assets/4dac11dd-1c8d-41b3-956a-c6bf47bfe436)

#### Um teste de configuração do Nginx foi feito:

![image](https://github.com/user-attachments/assets/ca2e068d-0878-4f47-9861-6700db744856)

#### E em seguida a reinicialização do Nginx é recomendada:
![image](https://github.com/user-attachments/assets/d60f75cf-83ef-4140-bab8-bc45cb929d20)

### Passo 3 - Verificação e depuração na aplicação:
#### Iniciei  utilizando o comando curl -I para visualizar o status retornado na página Localhost e Localhost/index.html, ambas retornando Status 200:

![image](https://github.com/user-attachments/assets/9591116d-2455-4ede-b064-0c943283fad3)

#### O último teste foi o de verificação da aplicação rodando através do browser:

![image](https://github.com/user-attachments/assets/2b6525be-e94f-40ce-a18c-b586086e0aa6)
![image](https://github.com/user-attachments/assets/a3c130a4-24a2-4181-87e8-1edfb81b1682)





