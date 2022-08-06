# Automação de tarefas no envio de mensagens

**Seminário de Orientação de Projeto Integrador**

**Alunos:**
- Alan Alves
- [Amanda Rodrigues](https://github.com/amanda-rosa)
- [Hetrisley Gomes](https://github.com/HetrisleyGomes)

***Sumário:***
- [Cronograma](#cronograma-do-projeto);
- [Diagramas](#diagramas);
- [Imagens](#imagens-das-telas);
- [Conclusões Finais (*vazio por enquanto*)](#fim);

---

## Cronograma do projeto

### Descrição:
Com esse projeto, pretendemos mostrar nosso avanço e conhecimento nas áreas de Desenvolvimento para dispositivos móveis e Testes de Software.

### Lista sequencial das atividades:

- Pesquisa e Documentação
- Desenvolvimento inicial
- Teste de implementação
- Documentação do projeto

### Cronograma:

```mermaid
gantt
title Cronograma do projeto
dateFormat DD-MM-YYYY
section Pesquisa e Documentação
 Definição do cronograma     		:a1, 24-05-2022, 7d
 Primeira pesquisa        		:a2, after a1, 10d
 Documentação Inicial     		:a3, after a2, 55d
 Criação de telas para modelo 		:a4, after a2, 3d
 Levantamento dos requisito e dados	:3d
 Diagramas uml (caso de uso, classe, componentes) :3d

section Desenvolvimento Inicial
  Preparação do ambiente de trabalho      :2d
  Começo do desenvolvimento do prototipo  :18d

section Testes de Implementação
  Teste de layout     :3d
  Testes unitários    :4d
  Testes de serviço   :4d
  Correção de erros   :5d
  Nova etapa de testes :10d
  
section Documentação do projeto
  Refinamento da Documentação      :after a3, 5d
  Envio para revisão do orientador :2d
  Revisão da documentação          :5d
  Preparação dos slides		   :3d

```
### Descrição dos grupos das atividades e das atividades:
#### **Pesquisa e Documentação:**
- Aqui é onde iniciaremos a pesquisa e definição das etapas do processo, sera uma etapa com bastante pesquisa.
- Inicia-se também a documentação do projeto, que continuará até o final da etapa de Testes de Implementação.

#### **Desenvolvimento inicial:**
- Com as pesquisas e diagramas prontos, iniciaremos a contrução de um protótipo.

#### **Teste de implementação:**
- Com o prototipo já em mãos, iniciaremos uma etapa de testes, para encontrar e corrigir possíveis erros.

#### **Documentação do projeto**
- Após todo esse período, finalizariamos a documentação do relatório.
- Preparariamos também os slides e a contrução da defesa do projeto.

[Voltar ao início](#automação-de-tarefas-no-envio-de-mensagens)

---

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


[Voltar ao início](#automação-de-tarefas-no-envio-de-mensagens)

---

## Imagens das telas

### Descrição:
Demonstraçao das telas da aplicação de Automação de tarefas no envio de mensagens.

### Telas iniciais
<img src="/imagens/Telas01.PNG" alt="telas iniciais" style="height: 300px; width:auto;"/>

A primeira tela é uma demonstração da tela de carregamento inicial, a segunda tela mostra o leyout do app ainda vazio, A partir dessa tela podemos ver:

<img src="/imagens/Telas01_2.PNG" alt="telas iniciais" style="height: 300px; width:auto;"/>

As janelas de visualização de chatbots salvos e os agendados por data; O menu extensivo, que revela as opçoes de configurações, permiçoes e politicas privacidade; E por fim um ícone onde nos possibilitarar a criação de novos chatbots.

### Telas de gerenciamento

#### Tela de gerenciamento 1:
Aqui são as telas de criação de chatbots, começando na primeira que seria a opção mais genérica de chatbot, logo de começo damos um nome a esse chat para ajudar na sua organização, abaixo tem o espaço para salvar as respostas por pergunta, como por exemplo informar ao app o que dizer se outra pessoa enviar um "oi", ainda nessa parte tem uma opção que pode ser marcada, chamada 'Mensagem guia', que caso outra pessoa envie uma mensagem que não possui resposta, o chatbot informaria as opções disponíveis.

Na parte mais abaixo temos a opção de informar quem esse chat responderá, podendo ser um grupo de contatos selecionados, todos os contatos, e qualquer número. Por fim vem a opção de qual(is) aplicativos o chat irá funcionar, neste exemplo, marcamos o whatsapp, telegram e sms.

#### Tela de gerenciamento 2:
A segunda tela não é tão diferente da primeira, porém essa tela mostra os chatbots agendados por data. Logo de começo a opção de por um nome neste chat, em baixo a mensagem a ser enviada, desta vez a mensagem não precisa que o seu contato envie uma mensagem como gatilho, ao invés disso esse gatilho será por data, logo a cima tem a opção de confirmação de envio, se essa opção for selecionada, antes do app enviar a mensagem ele pedirá uma confirmação para enviar.

Abaixo tem a opção de quem será enviada a mensagem, podendo adicionar de um em um ou todos os contatos de uma vez, nessa parte o ussuário vai escolher entre usar uma data para cada contato, ou selecionar a opção data por conjunto, onde é informado uma data onde será enviado a todos que estiverem marcados. Essa opção só será disponibilizada primeiramente ao aplicativo whatsapp.

<img src="/imagens/Telas02.PNG" alt="telas de gerenciamento" style="height: 300px; width:auto;"/>

Aqui estão as telas iniciais com chatbots salvos:

<img src="/imagens/Telas02_2.PNG" alt="telas iniciais" style="height: 300px; width:auto;"/>


### Telas contatos

Na primeira tela inicia-se com a página principal de adicionar um novo contato para o chatbot. Nessa tela de Novo contato, novos usuários poderão ser cadastrados no chatbot, serão adicionados os dados deles, sendo o nome, telefone e o e-mail. Nessa tela terá a opção de salvar o contato e uma opção de voltar. Esse botão de voltar será utilizado assim que o novo contato for adicionado na lista, com isso será redirecionado para a tela de visualizar a lista de contatos.

Na segunda tela temos uma lista com todos os usuários que foram cadastrados no chatbot. Essa lista especifica o nome do usuário e a foto, a foto é optativa, podendo ou não colocar a foto.
Na listagem, tem a opção de adicionar um novo contato também, para cadastrar mais usuários, clicando nesse botão, será redirecionado automaticamente para a primeira tela, a de novos contatos.
Voltando para a listagem dos contatos, lá temos a opção de pesquisar o contato, a partir do nome do usuário.
Por fim, ao clicar no nome do usuário, será redirecionado para uma nova conversa.

<img src="/imagens/Telas03.PNG" alt="telas contatos" style="height: 300px; width:auto;"/>

### Telas configurações

Na parte inicial apresenta a foto do usuário, visualização de cadastro e apagar conta.

Na visualização de cadastro, o usuário consegue ver seus dados vinculados a aplicação, dando a opção de fazer alterar foto, edições do nome, telefone e email, sendo que estes devem seguir o padrão de preenchimento, ao finalizar a visualização/edição, tem a opção de salvar ou voltar, para caso não deseje realizar a alteração e ao clicar em salvar, as informações devem imediatamente ser apresentada ao usuário na mesma tela que faz a edição.

Na opção de apagar conta, faz a pergunta se realmente deseje apagar a conta, se confirmar, o aplicativo deve direcionar o usuário a tela de cadastro, caso clicar em não, deve retornar a tela de configuração.

<img src="/imagens/Telas04.PNG" alt="telas configurações" style="height: 300px; width:auto;"/>

[Voltar ao início](#automação-de-tarefas-no-envio-de-mensagens)

---

## fim
