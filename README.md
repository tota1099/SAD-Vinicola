# SAD-Vinicola
Construção de um sistema de apoio a decisão. Transformando um banco de dados relacional para um banco de dados dimensional.

# Informações importantes

## PGADMIN (http://localhost:5050/browser/)

* **User:** admin
* **Password:** admin
  
## Postgres

* **Host:** postgres
* **User:** postgres
* **Password:** postgres
* **Database main:** curso
  
## Databases
    
* **relacional_vinhos:** Banco de dados relacional do sistema. É díficil exportar/análisar dados nesse banco, tempo de utilizar muitos joins e processando para tirar informaçes úteis.
* **dwvinhos:** Banco de dados dimensional. Sua estrutura foi definida anteriormente, com o objetivo de ser mais fácil a análise de dados importantes.
    
## Spoon (http://localhost:8181/spoon/spoon)

Existem 2 jobs principais no spoon:
  
 * **Job Gerar Carga:** Gera os dados do banco de dados relacional. O job possui várias transformações, e cada uma trabalha com uma dimensão (tempo, vinho, geografia, loja).
 * **Avaliação 3 Job:** Job relacionado a avaliação. Lê os dados do excel legado, adapta os dados para cada dimensão. Além disso, gera um excel com uma estatística (questão 4 da atividade).
