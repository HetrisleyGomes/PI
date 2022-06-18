# Automação de tarefas no envio de mensagens

**Seminário de Orientação de Projeto Integrador**

**Alunos:**
- Alan Alves
- Amanda Rodrigues
- Hetrisley Gomes


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

Na parte inicial apresenta a foto do usuário, com as opções de alterar foto, visualização de cadastro, central de ajuda e apagar conta.

Na visualização de cadastro, o usuário consegue ver seus dados vinculados a aplicação, dando a opção de fazer edições do nome, telefone e email, sendo que estes devem seguir o padrão de preenchimento, ao finalizar a visualização/edição, tem a opção de salvar ou voltar, para caso não deseje realizar a alteração e ao clicar em salvar, as informações devem imediatamente ser apresentada ao usuário na mesma tela que faz a edição.

Na opção de alterar foto, torna-se um campo optativo de inserir ou não a foto, ao clicar em escolher, deve ser direcionado ao diretório do dispositivo para buscar a foto desejada, caso não deseje fazer a alteração é só clicar em voltar, que retornará a tela de configuração.

<img src="/imagens/Telas04.PNG" alt="telas configurações" style="height: 300px; width:auto;"/>

Na opção de apagar conta, faz a pergunta se realmente deseje apagar a conta, se confirmar, o aplicativo deve direcionar o usuário a tela de cadastro, caso clicar em não, deve retornar a tela de configuração.

A opção de central de ajuda, traz informações acerca do aplicativo, em relação ao conceito e uso.

<img src="/imagens/Telas05.PNG" alt="telas configurações" style="height: 300px; width:auto;"/>

