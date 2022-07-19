# Semanas 11, 12 e 13: Construa o diagrama de casos de uso e modelagem do banco de dados.
## Diagramas

### Descrição:
Apresentação dos diagramas de banco de dados e de caso de uso.

### Diagrama de Banco de dados:

Esse diagrama uml mostra a relação de banco de dados, no nosso app todas as informações são salvas de maneira interna, o que quer dizer que não teremos um banco de dados externo para gerenciar as informações dos usuários, teremos apenas um com as configurações individuais. Segue o diagrama:

<img src="/imagens/Diagrama_BancoDados.jpg" alt="diagrama banco de dados" style="height: 400px; width:auto;"/>

1. **Mensagens:**
Apresenta o Identificador do tipo inteiro e faz a interação entre mensagens resposta e mensagens programadas, o ID irá alterar conforme as mensagens trocadas entre os usuários.

2. **Mens_Chatbot:**
Contém o identificador do tipo inteiro, que varia conforme as mensagens armazenadas, que fará a relação de muito para muito entre as listas de respostas e contatos armazenados na aplicação.

3. **Lista_mensagens:**
Contém um identificador do tipo inteiro que fará ligação com a lista de mensagens e respostas. Possui um campo input, que será a mensagem recebida, e um campo resposta, onde terá a resposta enviada. Ambos input e resposta são do tipo string.

4. **Contatos:**
Terá atributos públicos, do tipo inteiro, o que se relaciona a cada contato armazenado na aplicação, com seus nomes e números do tipo strings. 

5. **Mens_Programadas:**
Possui o ID do tipo inteiro, mensagem do tipo String, fazendo uma relação de muitos para muitos com o campo Mensagem e o campo Contato_data da aplicação.  

6. **Contato_data:**
Contém um identificador do tipo inteiro que fará ligação à lista de contatos de mensagens programadas, um identificador do tipo inteiro que fará conexão com a tabela de contatos, e a data a qual a mensagem será enviada.



### Diagrama de Caso de uso:

Esse diagrama mostra as relações que o usuário terá com a aplicação. Segue o diagrama:

<img src="/imagens/Diagrama_CasodeUso.jpg" alt="diagrama caso de uso" style="height: 700px; width:auto;"/>

**Cliente:**

Ao acessar o aplicativo, o cliente terá opção de Criar um chat, verificar data e verificar os input das mensagens recebidas.


Em criar um chat, aparecerá as opções de criar um chat de mensagens, e criar um chat programado.

Ao criar um chat por mensagens, irá observar as mensagens já prontas, como ao clicar no (+), o cliente poderá digitar mensagens imediatas e possivelmente irá fazer as opções de adicionar um ou mais contatos ou enviar para qualquer número e opções de compartilhamento, que pode ser por whatsapp, telegram ou sms.


Em criar um chat cronogramático, levará para a tela de Adicionar respostas, que será onde o usuário irá fazer o escopo da mensagem  e opções para quem e quando será respondido, como também terá a opção de adicionar todos os contatos ou novo contato.


Ao clicar no campo Por data na aplicação (Verificar data), levará o usuário enviar mensagens já programadas como chatbots_01 e mensagens do trabalho, que este possibilita ver as mensagens recebidas (Verificar input das mensagens recebidas) e responder essas mensagens (Responder mensagens).


O cliente após o acesso a aplicação, terá a opção de ir em configurações, que irá poder visualizar a sua foto e as alternativas de Visualizar Cadastro e Apagar Conta. Em visualizar cadastro, será apresentado o nome, fone e email, estes poderão ser alterados e após isso deve clicar obrigatoriamente em Salvar, ou caso contrário, deve clicar em voltar, para retornar à tela inicial da configuração. Em apagar conta, apresentará a mensagem “Deseja realmente apagar a conta” e as opções de sim e não, ao clicar no sim, a aplicação deve levar o indivíduo para fora da aplicação e ao clicar em não, deve retornar para tela inicial do sistema.


**Contatos:**

Os contatos, podem enviar e também receber mensagens. Ao receber as mensagens, ele pode enviar mensagens programadas ao usuário ou responder com mensagens não definidas. Dessa forma, possibilitará ao usuário verificar o input das mensagens recebidas e respondê-las. 
