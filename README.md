

# *Chamadas Thunder* 


POST /projetos/adicionar
URL: http://localhost:8080/projetos/adicionar
Method: POST
Body:
json
{
    "descricao": "Novo Projeto",
    "dataInicio": "2023-01-01",
    "dataFim": "2023-12-31",
    "funcionariosIds": [1, 2]
}

GET /projetos/{id}
URL: http://localhost:8080/projetos/1
Method: GET

POST /projetos/{idProjeto}/vincular/{idFuncionario}
URL: http://localhost:8080/projetos/1/vincular/2
Method: POST

FuncionarioController
POST /funcionarios/adicionar
URL: http://localhost:8080/funcionarios/adicionar
Method: POST
Body:
json
{
    "nome": "Novo Funcionario"
}

GET /funcionarios/{idFuncionario}/projetos
URL: http://localhost:8080/funcionarios/1/projetos
Method: GET

SetorController
POST /setores/adicionar
URL: http://localhost:8080/setores/adicionar
Method: POST
Body:
json
{
    "nome": "Novo Setor"
}

GET /setores/{idSetor}
URL: http://localhost:8080/setores/1
Method: GET
