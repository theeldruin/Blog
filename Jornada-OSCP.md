Olá queridos leitores, dia 13/07/2022 consegui receber a certificação OSCP (Offensive Security Certified Professional) e sugeriram fazer uma postagem para explicar minha jornada e rotina de estudos para conseguir ela. Vamos lá

# #Background
Inicialmente eu não comecei meus estudos em cyber segurança totalmente do zero. Na época eu já era graduado em Ciência da Computação fazia alguns anos (por mais que estivesse meio enferrujado), portanto já tinha conhecimento em protocolos de rede, programação, sistema operacional, etc..... E já havia feito um curso de inglês (TopWay), portanto já tinha uma ótima compreensão do idioma (intermediário-avançado)

Alguns desses conhecimentos não são “obrigatórios” para iniciar na área, porém é interessante ter eles para facilitar o aprendizado e a retenção de conhecimento. Sabendo protocolos de rede por exemplos acaba facilitando a compreensão de ferramentas como “netcat” e "telnet". Porém o INGLÊS é essencial que você domine o máximo possível, pois a maior parte das plataformas de estudos e as certificações mais conhecidas são neste idioma.

Após minha graduação fiquei aprox 10 anos sem atuar na área de TI, porém na época da pandemia me deparei com um vídeo "Você tapa a sua webcam" do Gabriel Pato (https://www.youtube.com/watch?v=2bpAg2QI-HM).

Depois de ver o vídeo acabei ganhando uma injeção de ânimo e comecei meus estudos em cyber segurança.

# #Inicio dos estudos
Para começar eu estava interessado em uma visão geral da área, então resolvi recorrer a Udemy para localizar um curso sobre hacking. Fi uma boa pesquisa para localizar o curso com o melhor custo/beneficio, pois muitos deles eram cursos pequenos (1h até 5h) e quase todos com o mesmo preço. Mas então eu localizei o curso [“Fundamentos de Ethical Hacking: curso prático”](https://www.udemy.com/share/101WyS3@_b1oQZML7nT4ox4pReKHvOak0HHzBnxjF7TgyAwASUe58d3c0cnzzpnVRRqczUd8/) do prof. Marcos Flávio Araújo Assunção. 

Para qualquer pessoa que esteja iniciando na área considero este o curso mais indicado, pois ele vai te dar uma visão geral da área, ferramentas, como montar um laboratório de testes, vulnerabilidades já encontradas e juntando tudo isso você começa a montar seu mindset. Faça anotações de TUDO, eu recomendo utilizar a ferramenta CherryTree para organizar suas anotações (ajuda MUITO)

# #Continuação dos estudos
Após concluir o curso do prof. Marcos Flávio busquei um material mais robusto, aproveitando uma promoção adquiri o curso ["Novo Pentest Profissional"](https://desecsecurity.com/cursos) da DESEC Security. Caso tenha dúvidas este é sim um curso com custo mais elevado, porém considerando que você recebe videoaulas + laboratório prático, o custo beneficio é absurdamente satisfatório.

A vantagem do curso da DESEC é que ele te explica em detalhes desde o básico (protocolos por exemplo), até o avançado (desenvolvimento de ferramentas e exploração de vulnerabilidades).

# #OSCP e Primeira tentativa
Após um tempo fazendo o curso da DESEC, continuei tentando me envolver com noticias e canais sobre pentest/hacking, com isso conheci o “Ultimate Hacking Championship” e comecei a acompanhar as transmissões deles. Depois de algum tempo participei de um sorteio e acabei ganhando um voucher para o curso [OSCP](https://www.offensive-security.com/pwk-oscp/) da Offensive Security.

> ⚠️AVISO⚠️  
> Não cometa meu erro. Após iniciar o curso da OSCP eu foquei nos estudo e deixei a prática nos laboratórios de lado. 
Se você já tiver conhecimento recomendo partir direto para a prática, porque o tempo de acesso aos laboratórios é limitado. Porém o material de estudo você recebe, portanto pode ver quando quiser.
Se não tiver conhecimento na área busque outros cursos antes deste, afim de acelerar a prática e aproveitar ao máximo as máquinas do laboratório.

Voltando... após concluir os estudos parti para a parte prática, conseguindo comprometer aprox. 13 máquinas (na época não documentei nada, não cometam esse erro kkkk)
Depois disso agendei minha primeira vez o exame e devo ter conseguido aprox. 40 pontos ☹️

# #Segunda tentativa
Depois de tomar esse banho de água fria resolvi praticar mais em CTFs. Buscando por máquinas para OSCP encontrei esse arquivo aqui [“NetSecFocus Trophy Room”](https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit#gid=1839402159)
Como rotina foquei em fazer as máquinas no VulnHub → HackTheBox

Após concluir as máquinas recomendadas parti para a segunda tentativa, devo ter feito aprox. 60 pontos.🤦‍♂️

# #Terceira tentativa (Com AD)
Por mais que tenha falhado uma segunda vez, o meu progresso em comparação as duas tentativas acabou me dando um estimulo para continuar os estudos.
Para a terceira tentativa refiz o caminho anterior mas adicionei mais máquinas
VulnHub → HackTheBox → Proving Grounds Play

Porém aqui eu lembrei que o exame OSCP havia mudado e seria inserido um ambiente AD. Como é complicado de encontrar ambientes de teste com essa estrutura resolvi fazer a máquina [WREATH](https://tryhackme.com/room/wreath) do TryHackMe.  
 
> Obs.: um pouco antes da minha prova o TryHackMe começou a liberar máquinas com ambientes AD. Não cheguei a fazer elas, mas recomendo que façam para se acostumar com a estrutura e formas de exploração.  

Para impedir uma Quarta Tentativa adquiri o [Proving Grounds Practice](https://www.offensive-security.com/labs/individual/), pois nela existem varias máquinas Windows e Linux desenvolvidas pela própria Offensive Security.  
Novamente eu segui a listagem do arquivo, mas fiz algumas outras máquinas. Que por mais que não sejam semelhantes as do teste acabam auxiliando pois temos contato com outras técnicas de exploração e tecnologias. 

# #Exame
Para fazer o exame eu foquei inicialmente no Ambiente AD, pois sem ele eu não teria chances de ser aprovado. 
Fiz todo o scan nas máquinas, identifiquei qual(is) seriam Domain Controllers e comecei a exploração a partir das informações que obtive.
Após aprox. 7h eu havia conseguido comprometer todas as 3 máquinas do AD

Depois disso partir para as outras 3 máquinas.
Fiz o scan nas 3 máquinas e comecei a enumeração.
Depois de algum tempo em cada uma dela foi possível identificar uma vulnerabilidade crítica, o que me deu acesso as máquinas
Depois de uma vasta pós-exploração foi possível identificar pontos para elevação de privilégios.

🏆Resultado Final: Todas as máquinas comprometidas - 100 Pontos

# #🥇DICAS DE OURO🥇
 - Durante seus estudos talvez você precise ler o writeup/walkthrough da máquina esta tentando explorar. Não tenha vergonha disso. Porém depois de um tempo volte e tente fazer máquina novamente mas sem ajuda.
    - Sugestão: Faça todas as máquinas sugeridas de uma plataforma (exemplo: HackTheBox), depois que terminar volte e tente fazer tudo novamente
 - A OSCP não é TÃO difícil quanto a fama dela. Faça os exercícios sugeridos, revise as informações e tenha calma durante a prova
 - Anote TUDO durante seus estudos. Recomendo colocar o máximo de informações possível em um único arquivo para ir consultando durante o exame.
   - Eu particularmente tenho um arquivo no CherryTree com comandos, rotinas de exploração, opções de ferramentas com exemplos. Enfim, faça do seu jeito e certifique-se de que você se localiza no arquivo
 - Durante a prova anote todos os comandos utilizados e registre todas as saídas dos comandos com prints. Isso facilitará na hora de fazer o relatório
 - No meu terceiro exame não caiu BufferOverflow, mas recomendo estas máquinas para praticar (https://tryhackme.com/room/bufferoverflowprep e https://tryhackme.com/room/gatekeeper)
