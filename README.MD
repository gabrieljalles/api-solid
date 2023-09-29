# GymPass Style app.

### RFs (Requisitos funcionais) - O que é possível fazer na aplicação.

 [ ] Deve ser possível se cadastrar;<br>
 [ ] Deve ser possível se autenticar;<br>
 [ ] Deve ser possível obter o perfil de um usuário logado;<br>
 [ ] Deve ser possível obter o número de check-ins realizados pelo usuário logado;<br>
 [ ] Deve ser possível o usuário obter seu histórico de check-ins;<br>
 [ ] Deve ser possível o usuário buscar academias próximas;<br>
 [ ] Deve ser possível o usuário buscar academias pelo nome;<br>
 [ ] Deve ser possível o usuário realizar check-in em uma academia;<br>
 [ ] Deve ser possível validar o check-in de um usuário;<br>
 [ ] Deve ser possível cadastrar uma academia;<br>
 
### RNs (Regras de negócios) - As regras devem ser associadas ao requisitos funcionais! 

 [ ] O usuário não deve poder se cadastrar com um e-mail duplicado;<br>
 [ ] O usuário não pode fazer 2 check-ins no mesmo dia;<br>
 [ ] O usuário não pode fazer check-in se não estiver perto (100m) da academia;<br>
 [ ] O check-in só pode ser validado até 20 minutos após criado;<br>
 [ ] O check-in só pode ser validado por administradores;<br>
 [ ] A academia só pode ser cadastrada por administradores;<br>

### RFNs (Requisitos não funcionais) - Somente o programador compreende;

 [ ] A senha do usuário precisa estar criptografada;<br>
 [ ] Os dados da aplicação precisam estar persistidos em um banco POSTGRESQL<br>
 [ ] Todas as listas de dados precisam estar paginadas com 20 itens por página;<br>
 [ ] O usuário deve ser identificado por um JWT (JSON WEB TOKEN);<br>


 ______________________________________________________________

 ### Códigos usados para programar!

1. npm init -y : Cria o package.json;<br>
2. Criar uma pasta chamada src e dentro dela, server.ts;<br>
3. npm i typescript @types/node -D : Baixa  o typescript para node;<br>
4. npm i tsx -D : usado para interpretar o código typescript para javascript e roda-lo no node;<br>
5. npm i tsup -D : usado para criar a versão de build da aplicação;<br>
6. npx tsc --init : iniciar cria o arquivo tsconfig.json;<br>
7. Mudar o dentro do tscondig o target para es2020;<br>
8. npm i fastify : criar
9. criar .gitignore e colocar o node_modules e build para ignorar<br>
10. Criar os scripts:<br> 
        "dev": "tsx watch src/server.ts", inicia servidor desenvolvimento<br>
        "build":"tsup src --out-dir build", converte e cria para a pasta build - produção<br>
        "start": "node build/server.js", inicia o servidor para  produção.<br>
12. Criar arquivo .npmrc com o dado save-exact=true : para fixar a versão do package.json<br>
13. <br>



