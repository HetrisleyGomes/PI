# Descreva no seu relatório Markdown um capítulo sobre a prototipação
## Prototipação do Projeto

### Diagramas

**Diagrama de Componentes:** Nesse diagrama de componentes, usamos as três disciplinas para montá-lo, Por parte da IoT vamos usar os serviços do twilio para para conectar pela internet para analisar e responder os clientes. Em conexão a internet teremos a aplicação, que será construída no Delphi, e está diretamente integrada aos testes de cobertura do software através de ferramentas como o Code Coverage.

<img src="/imagens/Diagrama_comp.jpeg" alt="Diagrama de Componentes" style="height: 300px; width:auto;"/>


**Diagrama de Banco de dados e Diagrama de Caso de uso:**

<img src="/imagens/Diagrama_BancoDados.jpg" alt="Diagrama de Componentes" style="height: 360px; width:auto;"/>

<img src="/imagens/Diagrama_CasodeUso.jpg" alt="Diagrama de Componentes" style="height: 600px; width:auto;"/>

para mais informações sobre esses diagramas clique [aqui](https://github.com/HetrisleyGomes/PI/blob/main/03-Diagramas.md)



### Prototipação do projeto :

- Solução em Mobile;
- Solução em IoT; 
- Estratégia de testes adotadas; 


#### Mobile

Com a IDE delphi, planejaremos desenvolver um aplicativo mobile para poder gerenciar e controlar o tráfego de mensagens por outros aplicativos, como o whatsapp e o telegram

#### Internet das Coisas

Integração com Twilio no ambiente de desenvolvimento delphi, será acessado por meio de serviços em nuvem, que será o meio de comunicação com entre dois ou mais dispositivos, nela os usuários poderão enviar e receber mensagens de forma automática e programada, bem como possibilitará comunicação via sms e Whatsapp.
O Twilio faz parte da CPaas (Plataforma de Comunicação em Serviço), que é 100% nas nuvens, possibilitando fazer ligações, sms, e-mails, push e whatsapp.

_( Ver mais sobre o Twilio e o envio de mensagens: <a href="https://www.twilio.com/docs/sms/send-messages" target="_blank">Envio de mensagens</a> , <a href="https://www.twilio.com/pt-br/docs/conversations" target="_blank">Conversas</a> , <a href="https://www.twilio.com/docs/sms/tutorials/how-to-send-sms-messages-delphi" target="_blank">Como enviar mensagens pelo delphi</a> )_



#### Testes

O Delphi disponibiliza de uma ferramenta de cobertura de códigos, o Code Coverage, iremos utilizá-la para verificar erros na programação do projeto.

