[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# RaidBrowser
Trazendo LFR para Wotlk (3.3.5a).

Este Addon substitui a aba LFR não utilizada (em 3.3.5a) no menu social por um localizador de raid funcional. O RaidBrowser funciona de forma semelhante ao localizador de grupos do Live WoW, exceto que os líderes de raid não precisam interagir com o Addon para listar seu grupo. O RaidBrowser procura mensagens LFR enviadas em canais do chat e /y e lista quaisquer raids encontradas na aba "Navegar" do navegador de raid.

Ao procurar por um raid para participar no Global, pode haver grandes quantidades de texto (e spam sem sentido) para ler a fim de encontrar qualquer coisa. Este complemento faz todo o trabalho de processamento de texto e lista todos os raids em um formato coerente. Cada entrada no navegador de raid é formatada da seguinte forma para incluir o nome do líder do raid, nome do raid, requisitos de gearscore e a lista de funções necessárias (tank/healer/dps).

![alt text](https://i.imgur.com/6aqE1TD.png)

Você não vai mais entrar em uma raid e passar vergonha ao perceber que já possui cooldown naquela raid feita na semana. O RaidBrowser destaca claramente as raids bloqueadas em vermelho (exemplo. ![alt text](https://i.imgur.com/hvTL7s8.png) ). Qualquer raid para o qual você não está em cooldown é marcado em verde brilhante (exemplo. ![alt text](https://i.imgur.com/5SkqcwA.png) ). Assim, você saberá de antemão se deve ignorar essa raid ou não.

# Como Baixar

Para baixar a versão estável mais recente, clique em "releases" que está na aba de estatísticas do repositório sob a descrição do addon (exemplo: https://github.com/Ostoic/RaidBrowser/releases/latest). O arquivo .zip 
é a pasta do addon, então certifique-se de descompactar essa pasta para uma chamada "RaidBrowser", então siga as instruções abaixo.

# Instalação e modo de usar
Assim como qualquer outro addon, copie a pasta RaidBrowser para o seu diretório /Interface/AddOns dentro da pasta do WoW.
Quando estiver no jogo, digite /rb para ativar a IU do navegador de raid. Como alternativa, a interface pode ser acessada da seguinte forma:
1. Abra o menu social (Pressione O),
2. Selecione a aba "Raid",
3. Clique em "Open Raid Browser"

É importante entrar no canal global para que o addon encontre raids. Se você não quiser que sua janela de bate-papo fique cheia de bate-papo global,
você pode simplesmente ocultar o canal global da sua janela de bate-papo padrão.

1. Clique com o botão direito na aba "General"
2. Clique em configurações (under Filters)
3. Selecione a aba "Global Channels"
4. Certifique-se de que "global" esteja desmarcado na lista de canais.

Agora o RaidBrowser poderá encontrar raids sem que o global seja despejado na janela de bate-papo geral.

See the common issues section for further help.

# Examples 
![alt text](https://i.imgur.com/dR7MIUf.png)
![alt text](https://i.imgur.com/qkVS07w.png)
![alt text](https://i.imgur.com/GvEgQSJ.gif)

# Common Issues
**Improper Addon Placement**

A fairly common issue when unzipping the addon is that your zip program puts the addon at RaidBrowser/RaidBrowser. Make sure that when you open the folder in the Addons directory (in %WoW Folder%/Interface/AddOns), you see all the .lua files (core.lua, RaidBrowser.toc, etc). Make sure you can see RaidBrowser.toc by going to %WoW Folder%/Interface/AddOns/RaidBrowser/RaidBrowser.toc.

# Todo
- Further improve pattern matching for better detection of LFM messages.
- Raid host tab where "Inv x gs [achieve]" messages are parsed similarly to how LFM messages are parsed. Can select raid to host, GS min req, achievement requirement, etc which will be formatted into an auto-barked message sent to the specified channel.
- If you run into any bugs, such as incorrect information being reported by the addon, send me a screenshot/copy of the original message and the incorrect information the addon displayed.
- Suggestions?? Open up an issue or send me a message ingame/in discord.

# Remark

Be aware that since it is difficult to consider every possible LFM message that someone could think of, this addon may consider false 
positives, or may omit valid LFM messages. As an example, some guild recruitment messages may be listed in the raid browser, since a lot of the language used in these messages is similar to LFM messages. On the other hand, a raid host may use unexpected words or grammar in their LFM message.

# Acknowledgements
Thanks to the following people for feature ideas and bug reports:
- Adidi
- Swenson
- Imbued
