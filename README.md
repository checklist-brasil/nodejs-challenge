# Desafio Node JS

## Criar uma API de Pokemons com autenticação e rotas protegidas

 - Criar uma API com suporte a criação, edição, exclusão e leitura, usando a seguinte
[API de referencia](https://pokeapi.co/)
 - A autenticação deve ser [JWT](https://jwt.io/)
 - Deve-se utilizar Docker para virtualização
 - Criar automatização de CI/CD (Sugestão: Usar o GitActions para subir uma nova imagem no docker registry (sugerimos o DockerHub, mas sinta-se avontade para usar outros gateways), sempre que um commit for empurrado para a branch MAIN na origin. A implantação deve apenas acontecer mediante a aprovação de PR's que serão abertos a partir da branch de desenvolvimento.)  
 - Testes unitários não são obrigatórios mas serão tratados como um diferencial (E que diferencial!)
 
## O que será avaliado:

- Arquitetura escolhida para desenvolvimento do teste.
- Qualidade e objetividade do código.
- Funcionamento do produto entregue.
- Seguir o padrão RESTful.
- Boas praticas de desenvolvimento de software (baixo acoplamento, reutilização de codigo, modelagem de dados, aplicação dos princípios SOLID e testes, caso haja)

### Rotas
##### Usuários

- Endpoint de login (JWT)
- Endpoint de cadastro
- Endpoint de remoção lógica
- Endpoint de editar perfil
- Endpoint de listar usuarios

##### Pokemons

- Endpoint para listagem
- Endpoint para criação
- Endpoint para edição
- Endpoint para exclusão
- Endpoint para detalhamento

### A solução DEVE conter

- Manual do setup no readme.md
- Dockerfile com as definições da imagem que será gerenciada pelo GitActions
- Garanta que sua aplicação tenha alta disponibilidade (Utilize o PM2 para clusterizar e gerenciar a disponibilidade, ou crie o mesmo comportamento via docker)
- O token da aplicação deverá expirar a cada 5 minutos, impedindo o usuario de comunicar com os endpoints utilizando o token expirado, a chave de critpografia utilizada na geração dos tokens, também deverá mudar concomitantemente.
- Isole os dados sensiveis em um arquivo de variavel de ambiente, e consuma na aplicação.
- Garanta que sua aplicação seja segura, se debruçando em recursos e pacotes disponíveis. 

### **Ganha + pontos se conter**

- Cobertura com [Jest](https://jestjs.io/) (ou qualquer outra ferramenta)
- Documentação com [ApiDoc](https://apidocjs.com/) (ou qualquer outra ferramenta)
- Setup do projeto com docker
- Variáveis de environment setadas por ambiente (não hard coded)
- CI/CD com GitActions, ou qualquer outra ferramenta de automatização (Não precisa estar integrado a nenhum cloud provider, basta apenas publicar a imagem docker no registry como uma prova de conceito)


### Processo de submissão

- Faça um fork deste projeto em sua conta no [Github](https://github.com/join) (crie um repositório privado).
- Em seguida, desenvolva o projeto em seu repositório privado.
- Por fim, adicione como membro o usuario (@dmourainatel) ao seu repositório, quando fizer isto, avise-nos por e-mail diego.moura@checktudo.com.br, avaliaremos o mais rápido possível e te daremos o feedback.

_Boa sorte!_



