                                    >-------------------------------------------------------------<
                                    # Plugins para serem feitos;                                  #
                                    #1º   WCZumbi                                                 #
                                    #2º   WCRadiação                                              #
                                    #3º   WCNoHitDelay                                            #
                                    #4º   WCAirDrop                                               #
                                    #5º   WCCofre                                                 #
                                    #6º   WCKillRanking                                           #
                                    #7º   WCBan                                                   #
                                    >-------------------------------------------------------------<
1º WCZumbi;

Come funcionara: Bom, para esse plugin ocorrer, terá que ser feito da seguinte forma; haverá um comando chamdo /sethorda, esse comando será usado para setar uma localização onde nascera 20 zumbis de uma vez só, isso ocorrera em tempo (X), por exemplo "/sethorda (1,2,3,4,5) 
o maximo de hordas que terá será somente 5, ao spawnar não averá mensagens no chat, será meio que surpresa pro player, logo os zumbis ao nascer vira com efeitos especiais tipo mais velocidade e tirara mais dano, as vezes pode ate envenenar um jogador.
Como assim?; simples, logo quando o zumbi spawnar (nem todos os zumbis serão o mesmo efeito), quero porcentagem ao nascer, tipo 5%,15%,30% e por fim 50% de chance de esles vir com tal efeito, quero que não so eles e sim todos os zumbis que spawnar no mapa vem com esses efitos porcentual, explicação abaixo.

On spawn and zumbies:
5% lerdesa 3, força 4. (Zumbi equipado com armadura de ferro, apos a morte não dropar armadura e sim carne podre.)
15% somente veneno 1. (Zumbi equipado com peitoral de ouro, apos a morte não dropar armadura e sim carne podre.)
30% velocidade 3, força 2. (Zumbi equipado com peitoral e calça de ferro, botina de diamante e capacete tambem, apos a morte não dropar armadura e sim carne podre.)
50% velocidade 4, regeneração 5. (Zumbi equipado com nehum tipo de armadura, apos a morte dropar carne podre.)
os efeitos temque ser permanentes. 

#Configuração

#Mundo que haverá zumbis modificados.
World: "DayZ"

#Tempo de spawnação de hordas.

Tempo: (a cada 3 horas) "3h"

#Localizações.
Locations:
1: "x=,y=,z="
2: "x=,y=,z="
3: "x=,y=,z="
4: "x=,y=,z="
5: "x=,y=,z="

#Ocorrera sorteio acada 3h, spawnara uma horda em somente uma localização.
#Mensagem que de quando setar a localização da horda ou remover.
mensagem1: "§4[HORDA] §cVocê removeu a localização da horda §6{1,2,3,4,5}§c, no caso não nascera mais hordas nesse local!"
mensagem2: "§4[HORDA] §cVocê setou a horda §6{1,2,3,4,5} §cna localização §6{localização}§c!"
#mensagem de ja setado.
mesagem3: "§4[HORDA] §cErro, esse localização já foi setada, remova ela para setar novamente!"
Comandos; /setarhorda {1,2,3,4,5}, /removerhorda {1,2,3,4,5}, /wchordareload (recarregar o plugin).
#Todos os plugins que nascerem sem ser da horda pelo mapa é para vir com os efeitos memso assim.
Permissão: WCZumbi.*
Obrigado :D
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
2º WCRadiação

Como funciona?; presumo que ja jogou free fire? kk, então é tipo aquilo que mata os jogadores, mas terá certos locais, e meio igual o sethorda, é por localização, /setradicao {1,2,3}, apenas 3
pra não dificultar muito.
Será tipo um campo invisivel que crescera, ele cresce so até 100 blocos, quando chega nos 100 ele fica 2 minutos ativo, caso alguém entre lá ganha dano constantemente até morrer, perdendo meio coração por segundo, caso ele sair da area ele se livra e não morrera
passando esses 2 minutos o campo de radição some, e depois de 2 horas aparecerá novamente ou outra localização, será somente 3, no caso numa delas.
Quando o jogador entrar na area ou a area começar a crescer e chegar aonde o jogador o jogador está, aparecerá a seguinte mensagem, "§4[ATENÇÃO] §cRadiação sendo liberada da terra, corra para um local seguro e salva-se." logo quando aparecer essa mensagem passara 5 segundos e se o jogador estiver dentro da aria ainda ele comesara
a levar danos como eu citei logo acima, logo quando ele sair aparecerá a seguinte mensagem, "§A[ATENÇÃO] &cVocê conseguiu se afastar do campo de radiação, fique tranqulo,já pode parar de correr!" e literalmente o dano desaparecera, mas caso ele entrar novamente dentro da radição surge essa seguinte mensagem;
"§4[ATENÇÃO] &cVocê entrou em uma aréa crescente de radiação, saia imediatamente ou você irá morrer!".

#Configuração 

#Mundo que será esposto a radiaçã.
World: "DayZ"

#Tempo de surigmento da radiação.
Tempo: (a cada 2 horas) "2h"

#Localizações.
Locations:
1: "x=,y=,z="
2: "x=,y=,z="
3: "x=,y=,z="

#Ocorrera sorteio a cada 2h, e a radiação surgirá somente em uma localização a cada 2h, será sorteada a localização ideal.

#Mensagens
#radição alçando o jogador.
mensagem1: "§4[ATENÇÃO] §cRadiação sendo liberada da terra, corra para um local seguro e salva-se."

#jogador entrando na area com radiação por querer e seguir em frente.
mensagem2: "§4[ATENÇÃO] &cVocê entrou em uma aréa crescente de radiação, saia imediatamente ou você irá morrer!".

#jogador saindo da area de radição.
mensagem3: "§A[ATENÇÃO] &cVocê conseguiu se afastar do campo de radiação, fique tranqulo,já pode parar de correr!"

#mensagem de setarradicao ou deletar radiação.
mensagem4: "§4[RADIAÇÃO] §cVocê setou radiação §6{1,2,3}§c na localização §6{localização}§c!"
mensagem5: "§4[RADIAÇÃO] §cVocê removeu a localização da radiação §6{1,2,3}§c, no caso não surgira radição nesse local!"
#mensagem de ja setado.
mesagem6: "§4[RADIAÇÃO] §cErro, esse localização já foi setada, remova ela para setar novamente!"

#Comandos
Comandos: /setradicao {1,2,3}, /removeradiacao {1,2,3}, /wcradicaoreload(recarregar o plugin).
Permissão: WCRadiação.*
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
3º WCNoHitDelay

BOM, esse ja expliquei para você, não haverá configuração, vou te mostrar no servidor do lek ai se vê como faz.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
4º WCAirDrop

Esse ja expliquei mas como sou legal, vou deixar registrado pra você :D
Bom esse é simples, mesmo sistema do de zumbis e mais facil :D, no caso terá /setairdrop {1,2,3,5,6,7,8,9,10} só 10 ta otimo.
Vou montar a configuração ai você entende melhor.

#obs: o airdrop será um sinalizador, apos ter caido em certa localização se o jogador clicar nele abrira um bau pequeno com os itens celecionados abaixo, logo quando ele pegar os itens o airdrop some.
#Configuração

#Mundo que ocorrera o AirDrop.
World: "DayZ"

#Tempo que o AirDrop vai cair.
Tempo: (a cada 4 horas) "4h"

#localização
locations:
1: "x=,y=,z="
2: ""
3: ""
4: ""
5: ""
6: ""
7: ""
8: ""
9: ""
10: ""

#As localização será sorteada, a qual for celecionada que será onde o airdrop vai cair a cada 4h, sempre sorteando a cada 4h.

#Itens que virá dentro do AirDrop.
Itens:
1: "56,1"
2: "277,1"
3: "1,30"
4: ""
5: ""
6: ""
7: ""
8: ""
9: ""
10: ""
11: "" 
12: ""
13: ""
14: ""
15: ""
16: ""
17: ""
18: ""
19: ""
20: ""
#Mensagem de quando setar a localização do AirDrop ou remover.
mensagem1: "§4[AirDrop] §cVocê removeu a localização da horda §6{1,2,3,4,5}§c, no caso não nascera mais hordas nesse local!"
mensagem2: "§4[AirDrop] §cVocê setou a horda §6{1,2,3,4,5} §cna localização §6{localização}§c!"
#Mensagem de ja setado.
mesagem3: "§4[AirDrop] §cErro, esse localização já foi setada, remova ela para setar novamente!"
#Mensagem ao cair o AirDrop.
mensagem4: "§b[AirDrop] &6Caindo um AirDrop na localização {localização}, corra para garantir que seja seu!"
#Comandos
comandos: /setaraidrop {1,2,3,4,5,6,7,8,9,10}, /removerairdrop {1,2,3,4,5,6,7,8,9,10},/wcairdropreload (recarregar o plugin).
Permissão: WCAirDrop.*
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
5º WCCofre
Bom esse e bem simples e facil :D, ele terá não uma localização, e sim será um bloco, esse bloco será o ejetor, o jogador clicara no cofre com uma chave a chave será um item
pode ser o gancho de armadilha, so terá uma forma de pegar esse ganho que será com comando /pegarchave e so admins poderão usar, e também o cofre será pego apenas com comando /pegarcofre.
bom, logo quando pegar o cofre, eu colocarei apenas em um local, quando o cofre recarregar os itens aparecera dentro do bau do cofre, tipo e mesma coisa do airdrop, so que em um local
fixo, o negocio terá um tempo para resetar em media de 2h, ai quando resetar aparecera uma mensagem avisando que ele foi restaurado e tal, o jogaodor que chegar primeiro com a chave e abrir o cofre ganha os itens.
logo o cofre será um ejetor certo?, quando o plyer clicar vai abrir um bau pequeno com varios itens que eu colocar na configuração, logo quando ele pegar os itens e sair do bau, o ejetor vira obsidian
e quando ele recaregar novamente, a obsidian vira o ejetor.
Vamos a configuração.

#Configuração

#Mundo que havera o cofre.
World: "DayZ"

#horario de resetação.
Tempo: "2h" ou "4h"

#item que será o cofre.
cofre: "23" (Nomeado: "§8Cofre")

#item que será o cofre em recarregamento.
cofre2: "49" (Nomeado: "§8Cofre")

Item que será a chave para abrir o cofre.
chave: "131" (Nomeado: "§8Chave §f- §cAbra um cofre!"

#Itens do cofre.
itens:
1: "56,1"
2: "277,1"
3: "1,30"
4: ""
5: ""
6: ""
7: ""
8: ""
9: ""
10: ""
11: "" 
12: ""
13: ""
14: ""
15: ""
16: ""
17: ""
18: ""
19: ""
20: ""

#Mensagens
mensagem1: "§4[COFRE] &cVocê pegou um cofre, coloque em um local!"
mensagem2: "§4[COFRE] &cVocê pegou uma chave, abra um cofre!"
mensagem3: "§4[COFRE] &cDesculpe, mas o cofre está vazio, volte mais tarde."
mensagem4: "§a[COFRE] &6O cofre foi recarregado!!!"
#Comandos
Comandos: /pegarchave,/pegarcofre,/wccofrereload.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
6º WCKillRanking
Então, eu já tenho esse plugin, pois o cara que fez deixou varios bugs e na versão só 1.5.2, queria que você refizesse ele da mesma forma, mas colova como prioridade minha, tipo wckillranking
e resolvesse os bugs.
Obrigado :D, logo pedirei mais plugins, só falta ideia :v.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
7º WCBan
Então, esse é essencial kk, plugin top de ban.
vou montar uma base pra você entender do jeito certo.
  
#Inicio.
Prmeiro comando; /wcban
Mensagem no chat, quando o staff digitar o comando acima sem o argumento, tipo /wcban <rick_games> <hack>.		
1 linha: "&c[WillCraft] &bSistema De Banimentos - Comandos"
2 linha: "&c[WillCraft] &b/wcban list - Lista De Argumentos De Banimentos"
3 linha: "&c[WillCraft] &b/wcban - Ferramenta De Banir Jogador"
4 linha: "&c[WillCraft] &b/wcunban - Ferramenta De Desbanir Jogador"
5 linha: "&c[WillCraft] &b/wcbanip - Ferramenta De Banir o IP do Jogador"
6 linha: "&c[WillCraft] &b/wckick - Ferramenta Usada Para kickar somente um jogador"
7 linha: "&c[WillCraft] &b/wckickall - Ferramenta Usada Para kickal todos os jogadores"
8 linha: "&c[WillCraft] &3Modo De Uso -> /WCBan [Nick] [Motivo]"
9 linha: "&c[WillCraft] &3Lembrete: [Nick] = Nick do Player"
10 linha: "&c[WillCraft] &3Lembrete: [Motivo] = Argumento do /WCBAN List"
11 linha: "&c[WillCraft] &eUse Com Sabedoria!, E Tenha Um Bom Trabalho!"
Segundo comando; /wcban list
Mensagem no chat, quando o staff digitar o comando acima.
Obs: Leia as observações de cada motivo.
1 linha: "&c[WillCraft] &eSistema De Banimentos - Argumentos"
2 linha: "&c[WillCraft] &bMotivos: &6HACK &b= Permanente" Obs: (Quando o staff digitar /wcban <player> <hack>, quero que bani o nick e juntamente o ip do jogador.)
3 linha: "&c[WillCraft] &bMotivos: &6NICK &b= Permanente - Nick Inadequado" Obs: (Esse aqui será banido apenas o nick)
4 linha: "&c[WillCraft] &bMotivos: &6ATJ &b= 12 horas - Anti-jogo"
5 linha: "&c[WillCraft] &bMotivos: &6BUG &b= Permanente - Abuso De Bugs" Obs: (Esse aqui será banido apenas o nick)
6 linha: "&c[WillCraft] &bMotivos: &6DVG &b= Permanente - Divulgaçães de Servidores/Ips/Sites (permitido YT)" Obs: (Esse aqui será banido apenas o nick)
7 linha: "&c[WillCraft] &bMotivos: &6FLD &b= 3 horas e 30 minutos - Flood" 
8 linha: "&c[WillCraft] &bMotivos: &6Negar &b= Permanente - Negar Tela" Obs: (Quando o staff digitar /wcban <player> <negar>, quero que bani o nick e juntamente o ip do jogador.)
9 linha: "&c[WillCraft] &bMotivos: &6OFT &b= Permanente - Ofensa a Staff (ofensa a membros não são considerados)" Obs: (Esse aqui será banido apenas o nick)
10 linha: "&c[WillCraft] &bMotivos: &6Xinga &b= 12 horas - Xingamento ou palavras inadequadas"
11 linha: "&c[WillCraft] &bMotivos: &6OFS &b= Permanente - Ofensa a o SERVIDOR" Obs: (Quando o staff digitar /wcban <player> <ofs>, quero que bani o nick e juntamente o ip do jogador.)
12 linha: "&c[WillCraft] &eUse Com Sabedoria!, E Tenha Um Bom Trabalho!"

#Configuração

MySQL:
  Use: false
  User: henriquegames
  Password: JmrxMfqzZ8fk9Snv
  Port: 3306
  Host: localhost
  Database: henriquegames_fullpvp
  table: wcban_lista
  table-history: wcban_historia

#Mensagens de banimentos,
#Ban uso de hack.
BanHack: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Uso de Hacker(s)/Mod(s)/Cliente Alternativo. &e-> &4Sem volta com VIP &e<-"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso Servidor, &4Por: &c[&a{Staff}&c] &4Motivo: &cUso de Hacker(s)/Mod(s)/Cliente Alternativo."

#Ban nick inadequado.
BanNick: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Nick inadequado, procure utilizar outro tipo de Nick!"
MensagemBroadcast: "&cO Jogador &4{Player} foi banido permanente de nosso Servidor, &4Por: &c[&a{Staff}&c] Motivo:&c Nick inadequado."

#Ban por Anti-Jogo.
BanATJ: "&cVocê foi banido temporariamente do servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Anti-Jogo, restam &4({11}&ch &4{59}&cmin e&4 {60}&cseg&4) para seu ban expirar!"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido por &4(11&ch &459&cmin &ce &460&cseg&4)&c, &4Por: &c[&a{Staff}&c] &4Motivo:&c Anti-Jogo."

#Ban por abusos de bugs.
BanBUG: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Abuso de Bugs! &e-> &aCom volta de VIP &e<-"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso servidor, &4Por: &c[&a{Staff}&c] &4Motivo:&c Abuso de Bugs."

#Ban por divulgação.
BanDVG: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Divulgações de Sites/Servidores/IPS! &e-> &aCom volta de VIP &e<-"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso servidor, &4Por: &c[&a{Staff}&c] &4Motivo:&c Divulgações de Sites/Servidores/IPS."

#Ban por flood.
BanFLD: "&cVocê foi banido temporariamente do servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Flood, restam &4({3}&ch &4{29}&cmin e&4 {60}&cseg&4)&c para seu ban expirar!"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido por &4(3&ch &429&cmin &ce &460&cseg&4)&c, &4Por: &c[&a{Staff}&c] &4Motivo:&c Flood."

#Ban por negar a tela.
BanNegar: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Negar tela, suspeita de Hack! &e-> &4Sem volta com VIP &e<-"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso Servidor, &4Por: &c[&a{Staff}&c] Motivo:&c Negar tela, suspeita de Hack."

#Ban por ofença a staff.
BanOFT: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Ofensa a Staff! &e-> &aCom volta de VIP &e<-"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso Servidor, &4Por: &c[&a{Staff}&c] Motivo:&c Ofensa a Staff."

#Ban por xingamentos ou por palavras inadequadas.
BanXinga: "&cVocê foi banido temporariamente do servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Xingamento ou palavras inadequadas!, restam &4({11}&ch &4{59}&cmin e&4 {60}&cseg&4) para seu ban expirar!"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido por &4(11&ch &459&cmin e &460&cseg&4)&c, &4Por: &c[&a{Staff}&c] &4Motivo:&c Xingamento ou palavras inadequadas."

#Ban por ofensa a o servidor.
BanOFS: "&cVocê foi banido permanente de nosso Servidor! &4Por: &c[&a{Staff}&c] &4Motivo:&c Ofensa ao SERVIDOR!"
MensagemBroadcast: "&cO Jogador &4{Player} &cfoi banido permanente de nosso Servidor, &4Por: &c[&a{Staff}&c] Motivo:&c Onfensa ao SERVIDOR."

#Quando um jogador banido volta pro servidor.
Welcome-ban: "&aVocê foi desbanido(a) pelo nosso sistema, seja bem-vindo(a) de volta :)"

#Kickmensagens
Kick: "&cVocê foi kickado do Servidor!"

#kickbroadcast
kickbroadcast: "&cO jogador {jogador} foi kickado do servidor!"

#Quando o staff digita /kickall, aparecerá no chat para ele.
Kickall: "&cTodos os jogadores foram kickados, menos você!"

#Banip
#Mensgem pro staff, "&cVocê baniu o ip do jogador {jogador}, {Ip}!"

#Unbanip, quero que quando dar /wcunban desbani o nick e o ip do jogador mesmo o ip não estando banido.

#Jogador desbanido
Desban: "&cO jogador {jogador} foi desbanido do servidor!"

#/WCBANRELOAD
#Mensagem, "&aPlugin recarregado."

#Desbanindo jogador, "&cVocê desbaniu o jogador {jogaodor}!".
#Ao banir um jogador, "&cJogador banido com sucesso, bom trabalho!"

#Meia configuração
  Welcome-ban-msg: true
  Broadcast-kick-msg: false
  Broadcast-ban-msg: true
  SalvarIpBanido: true
  SalvarNickBanido: true
  Broadcast-desban-msg: false
version: 1.0
