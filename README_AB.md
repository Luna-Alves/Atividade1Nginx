## Tutorial detalhando a configuração do Apache Bench e execução de um teste de carga no Home de uma aplicação em React.

### Passo 1 - Instalação do Apache Bench
#### O Apache Bench serve para medir o desempenho de um servidor web através da submissão de um volume determinado de requisições ao HTTP. Com ele, podemos determinar a quantidade de requisições que devem ser feitas e quantas devem ser executadas em paralelo, a fim de simular um cenário. Essa simulação nos retorna um relatório com métricas de tempo médio de resposta, percentuais de latência e taxa de transferência de dados, por exemplo.

#### Sabendo disso, a primeira coisa a ser feita para as minhas simulações foi utilizar um comando para a instalação do Apache Bench, aqui, sendo utilizado o WSL2 com Ubuntu rodando no Windows:
![image](https://github.com/user-attachments/assets/7cf345d0-8cae-457c-9f85-30dc77321a36)

### Passo 2 - Acesso ao diretório e início dos testes:
#### Dentro do diretório do projeto criado para essa simulação:
![image](https://github.com/user-attachments/assets/909fc907-4852-4f21-8b5a-667c6d96e75b)

#### A execução do Apache foi feita através de linha de comando. A seguir, executei o teste disparando 1000 requisições com 50 delas acontecendo de forma paralela:

![image](https://github.com/user-attachments/assets/588449b4-01aa-48d4-83be-dedbdcd3bf57)

#### Execução do teste disparando 10000 requisições com 100 delas acontecendo de forma paralela:

![image](https://github.com/user-attachments/assets/6f607efc-6864-4cdd-b759-8d629b355aae)

#### Execução do teste disparando 100000 requisições com 1000 delas acontecendo de forma paralela:
![image](https://github.com/user-attachments/assets/32fcfe5f-16f5-4b49-8c91-c295c35697b7)
