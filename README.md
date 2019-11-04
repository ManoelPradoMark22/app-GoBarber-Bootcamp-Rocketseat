# API GoBarber
## API da aplicação GoBarber, desenvolvida durante o Bootcamp da Rocketseat. Tem como função agendamento de horário para corte de cabelo.
Para a aplicação funcionar, siga os passos:
<ul>
<li>Caso não tenha instalado, instale o <a href="https://docs.docker.com/docker-for-windows/install/">Docker</a> na sua máquina e o inicie;</li>
<li>Crie os containers executando, na raíz do projeto, cada comando a seguir:
<br />
docker run --name gobarber -e POSTGRES_PASSWORD=sua_senha_aqui -p 5432:5432 -d postgres
<br />
docker run --name mongobarber -p 27017:27017 -d -t mongo
<br />
docker run --name redisbarber -p 6379:6379 -d -t redis:alpine
</li>
<li>Para ver se os conteiners estão rodando execute:
<br />
docker ps
<br />
Este comando mostra todos os containers em execução ("docker ps -a" mostra todos, até os que não estão em execução no momento).
</li>
<li>Caso você tenha parado a execução de algum container, basta executar o comando:
<br />
docker start nome_do_container
<br />
Isso irá iniciar o container em questão.
</li>
<li>Agora em um terminal, na raíz do projeto, execute:
<br />
yarn queue
</li>
<li>Em outro terminal, na raíz do projeto, execute:
<br />
yarn dev
</li>
<li>E, por fim, em outro terminal, também na raíz do projeto, execute:
<br />
yarn start
</li>
</ul>
