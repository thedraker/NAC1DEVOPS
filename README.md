# Sistemas para Internet - SecDevOps

***nac:*** Criação de uma aplicação no formato "CRUD" executada em containers com base na linguagem "PHP" e no banco de dados "MySQL";

---

***Importante:***
PROCESS FLOW DEVOPS
NAC02
2TINR
RM78065
LUIZ CARLOS SILVA PIRES

1 - Abra o command line em uma pasta de sua preferência, e execute:

git clone https://github.com/thedraker/NAC1DEVOPS.git

2 - Pelo command line do docker navegue para a pasta NAC1DEVOPS/backend execute o seguinte comando:

$ docker run -d --rm --name backend -e MYSQL_DATABASE=demo -e MYSQL_ALLOW_EMPTY_PASSWORD=yes db:0.0.1

3 - Pelo command line do dockernavegue para a pasta frontend:

$ docker run -d --rm --name frontend -p 80:80 --link backend frontend:0.0.1

4 - Acesse http://ipdodocker/ para acessar a aplicação 
