[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# RaidBrowser
Trazendo LFR para Wotlk (3.3.5a).

Este Addon substitui a aba LFR não utilizada (em 3.3.5a) no menu social por um localizador de raid funcional. O RaidBrowser funciona de forma semelhante ao localizador de grupos do Live WoW, exceto que os líderes de raid não precisam interagir com o Addon para listar seu grupo. O RaidBrowser procura mensagens LFR enviadas em canais do chat e /y e lista quaisquer raids encontradas na aba "Navegar" do navegador de raid.

Ao procurar por um raid para participar no Global, pode haver grandes quantidades de texto (e spam sem sentido) para ler a fim de encontrar qualquer coisa. Este complemento faz todo o trabalho de processamento de texto e lista todos os raids em um formato coerente. Cada entrada no navegador de raid é formatada da seguinte forma para incluir o nome do líder do raid, nome do raid, requisitos de gearscore e a lista de funções necessárias (tank/healer/dps).

![alt text](https://i.imgur.com/6aqE1TD.png)

Você não vai mais entrar em uma raid e passar vergonha ao perceber que já possui cooldown naquela raid feita na semana. O RaidBrowser destaca claramente as raids bloqueadas em vermelho (exemplo. ![alt text](https://i.imgur.com/hvTL7s8.png) ). Qualquer raid para o qual você não está em cooldown é marcado em verde brilhante (exemplo. ![alt text](https://i.imgur.com/5SkqcwA.png) ). Assim, você saberá de antemão se deve ignorar essa raid ou não.

# Como Baixar

Para baixar a versão estável mais recente, clique em "releases" que está na aba de estatísticas do repositório sob a descrição do addon (exemplo: https://github.com/valberlimabr/RaidBrowser/releases). 
O arquivo "RaidBrowser-release.zip" é a pasta do addon, então após baixar-lo clique com o botão direito no arquivo e selecione "extrair aqui" agora você terá uma pasta chamada "RaidBrowser", 
agora siga as instruções abaixo.

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

Consulte a seção de problemas comuns para obter mais ajuda.

# Lembrete

Esteja ciente de que, como é difícil considerar todas as mensagens LFM possíveis que alguém poderia pensar, este complemento pode considerar falsos positivos ou pode omitir mensagens LFM válidas. 
Como exemplo, algumas mensagens de recrutamento de guilda podem ser listadas no navegador de raid, já que muito da linguagem usada nessas mensagens é semelhante às mensagens LFM. Por outro lado, um host de raid pode usar palavras ou gramática inesperadas em sua mensagem LFM.

# Problemas comuns
**Colocação inadequada do addon**

Um problema bastante comum ao descompactar o addon é que seu programa de descompactação pode colocar o addon em RaidBrowser/RaidBrowser. 
Certifique-se de que quando você abrir a pasta no diretório Addons (em %WoW Folder%/Interface/AddOns), você veja todos os arquivos .lua (core.lua, RaidBrowser.toc, etc). Certifique-se de que você pode ver RaidBrowser.toc indo para %WoW Folder%/Interface/AddOns/RaidBrowser/RaidBrowser.toc.

- Se você encontrar algum bug, como informações incorretas sendo relatadas pelo addon, envie-me uma captura de tela/cópia da mensagem original e as informações incorretas que o addon exibiu.
- Sugestões?? Abra um problema ou envie-me uma mensagem no jogo/no discord.

# Examples 
![alt text](https://i.imgur.com/dR7MIUf.png)
![alt text](https://i.imgur.com/qkVS07w.png)
![alt text](https://i.imgur.com/GvEgQSJ.gif)

# Todo
- Melhorar ainda mais a correspondência de padrões para melhor detecção de mensagens LFM.
- Aba de host de raid onde as mensagens "Inv x gs [Achievement]" são analisadas de forma semelhante a como as mensagens LFM são analisadas.

# Acknowledgements
Thanks to the following people for feature ideas and bug reports:
- Adidi
- Swenson
- Imbued
