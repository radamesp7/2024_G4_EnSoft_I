<body>
  <h1>Levantamento de Requisitos para um Sistema de Controle de Estacionamento</h1>
  <p>Base: Estacionamento do Shopping Patio Chapecó</p>

  <h2>Equipe</h2>
  <p>Andre Gabrielli da Silva, Arthur Couto Mulling e Gustavo Henrique Telo.</p>

  <h1>Descrição do Sistema</h1>
  <p>O estacionamento controla o momento de entrada e saída dos veículos utilizando um cartão que é emitido antes da entrada, abrindo a catraca para dar passagem e recolhido antes da saída. Após a retirada do cartão e entrada do veículo, o sistema contabiliza o tempo em que o veículo permaneceu dentro do estacionamento e cobra uma taxa fixa após 15 (quinze) minutos da entrada.</p>
  <p>As vagas dentro do estacionamento possuem um sensor para monitoramento das vagas ocupadas, mostrando uma luz verde em caso de vaga livre e uma luz vermelha em caso de vaga ocupada. Para a saída do veículo, será necessário pagar a taxa registrada por tempo no cartão, permitindo a devolução do cartão no momento da saída do veículo somente se a taxa for paga, assim abrindo a catraca. Caso contrário, o cartão será recusado.</p>
<p>O pagamento da taxa poderá ser feito dentro do shopping em algumas maquinas/computadores cujo permitem efetuar o pagamento da taxa do cartão por meio delas. O pagamento também pode ser feito com a atendente a qual fica na entrada, ou saida, do shopping em frente ao estacionamento no segunda andar.</p>

  <section>
    <h2>Perguntas Feitas em Entrevistas/Respostas</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <thead>
        <tr>
          <th style="width: 25%;">Pergunta</th>
          <th>Resposta</th>
        </tr>
      </thead>
      <tr>
        <td><h3>O que você acha do estacionamento?</h3></td>
        <td>Todos os entrevistados avaliaram o estacionamento como um bom estacionamento sem muitos comentários sobre ele, exceto sobre seu valor, que poderia ser mais barato.</td>
      </tr>
      <tr>
        <td><h3>Você acha que o estacionamento poderia melhorar em algo?</h3></td>
        <td>Dentre os entrevistados, a grande maioria não apontou nenhuma melhoria, pois achavam o estacionamento bom o suficiente da forma que estava. No entanto, alguns sugeriram que fosse adicionada alguma forma de organização para que os carros possam trafegar pelo estacionamento de forma mais fluida, já que frequentemente há situações de bloqueios devido ao grande fluxo de carros.</td>
      </tr>
      <tr>
        <td><h3>Acha que o estacionamento é seguro? Se não, quais motivos e como pode melhorar?</h3></td>
        <td>Nesta parte da entrevista, tivemos um resultado de respostas unânime. Todos os entrevistados concordam que o sistema de segurança do estacionamento é muito bom e não acham que precisa de alguma melhoria.</td>
      </tr>
    </table>
  </section>

  <section>
    <h2>Pontos Críticos</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <thead>
        <tr>
          <th>Ponto Crítico</th>
        </tr>
      </thead>
      <tr>
        <td>Em caso de algum problema ou perda do cartão causará problemas para efetuar o pagamento e consequentemente para a saída do veículo.</td>
      </tr>
      <tr>
        <td>Possível falha no sistema de detecção de vagas disponíveis poderá ocasionar um “falso positivo” onde o sistema identifica uma vaga vazia como ocupada, causando uma possível confusão e atrapalhando a localização de vagas.</td>
      </tr>
    </table>
  </section>

  <section>
    <h2>Áreas para Melhorias</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <thead>
        <tr>
          <th>Área para Melhoria</th>
        </tr>
      </thead>
      <tr>
        <td>Uma melhoria no sistema de identificação da entrada e saída de veículos, podendo evitar erros com o cartão.</td>
      </tr>
      <tr>
        <td>Organização na procura de vagas dentro do estacionamento a fim de evitar transtornos durante a procura de uma vaga.</td>
      </tr>
    </table>
  </section>

  <section>
    <h2>Funcionalidades Adicionais</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <thead>
        <tr>
          <th>Funcionalidade</th>
        </tr>
      </thead>
      <tr>
        <td>Aplicação de um app para mapeamento de vagas disponíveis, mostrando a localização exata da vaga e guiando o motorista para a mesma, assim agilizando e facilitando o uso do estacionamento. Desta forma também criaria uma maior fluidez no tráfego de veículos.</td>
      </tr>
      <tr>
        <td>Criação de um sistema para cadastro e criação de uma conta para o estacionamento, permitindo ao motorista utilizar um sistema de recarga de créditos para pagamento do estacionamento, permitindo que o mesmo não precise parar para pagar o estacionamento e assim somente descontado do crédito da conta. Este sistema funcionaria através de um leitor de placas que identificaria o carro cadastrado na conta do usuário.
  O aplicativo também contaria com um sistema de alerta para avisar o usuário de quanto tempo ele pode ficar estacionado antes que se esgote o crédito do cartão. Em caso de esgotamento, o aplicativo permitirá que o pagamento do tempo adicional seja feito dentro do mesmo, visando praticidade para o usuário. Também podendo contar com descontos para quem possuir cadastro.</td>
      </tr>
      </tr>
      <tr>
        <td>Sistema de feedback para o estacionamento, permitindo críticas e sugestões de melhorias para o estacionamento, assim possibilitando novas melhorias e um maior conforto do cliente.</td>
      </tr>
    </table>
  </section>

  <section>
    <h2>Requisitos Funcionais</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <tr>
        <th style="width: 25%;">Título</th>
        <th>Descrição</th>
      </tr>
      <tr>
        <td>Controle de acesso de veículos</td>
        <td>O sistema deve registrar a entrada e saída de veículos, monitorando o fluxo no estacionamento.</td>
      </tr>
      <tr>
        <td>Monitoramento da ocupação das vagas</td>
        <td>O sistema deve acompanhar em tempo real o status das vagas, indicando quais estão livres ou ocupadas.</td>
      </tr>
      <tr>
        <td>Processamento de pagamento conforme tempo de permanência</td>
        <td>O sistema deve calcular automaticamente o valor do pagamento, aplicando uma tarifa fixa após 15 minutos e uma cobrança adicional a cada hora.</td>
      </tr>
      
      <tr>
        <td>Relatório de incidentes de segurança</td>
        <td>A Equipe de Segurança deve registrar e enviar relatórios de incidentes, como batidas de veículos ou brigas, diretamente pelo sistema.</td>
      </tr>
      <tr>
        <td>Relatório de manutenção</td>
        <td>A Equipe de Manutenção deve registrar e enviar relatórios sempre que houver necessidade de reparos ou ajustes no estacionamento.</td>
      </tr>
    </table>
  </section>

  <section>
    <h2>Requisitos Não Funcionais</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <tr>
        <th style="width: 25%;">Título</th>
        <th>Descrição</th>
      </tr>
      <tr>
        <td>Desempenho</td>
        <td>O sistema deve processar e atualizar as informações em tempo real, com respostas imediatas (menos de 1 segundo) para monitoramento e transações.</td>
      </tr>
      <tr>
        <td>Segurança</td>
        <td>Todos os dados, incluindo informações de pagamento e relatórios de incidentes, devem ser criptografados para garantir a privacidade e segurança.</td>
      </tr>
      <tr>
        <td>Escalabilidade</td>
        <td>O software deve ser capaz de gerenciar um número crescente de veículos, transações e relatórios sem perda de desempenho.</td>
      </tr>
      <tr>
        <td>Portabilidade</td>
        <td>O sistema deve ser acessível em dispositivos móveis para permitir que administradores e equipes monitorem e registrem atividades remotamente.</td>
      </tr>
      <tr>
        <td>Usabilidade</td>
        <td>A interface do sistema deve ser fácil de usar, permitindo que os administradores e equipes operem sem a necessidade de treinamento especializado.</td>
      </tr>
      <tr>
        <td>Manutenção</td>
        <td>O sistema deve ser modular, facilitando a implementação de atualizações e manutenções sem interrupção do serviço.</td>
      </tr>
      <tr>
        <td>Auditoria</td>
        <td>O sistema deve manter logs detalhados de todas as operações e transações financeiras, armazenados por um período mínimo de 12 meses.</td>
      </tr>
    </table>
  </section>
</body>

<tbody style="width: 25%; border: 2px solid black; text-align: center;">
    <tr>
        <td>
            <img
                src="https://github.com/radamesp7/2024_G4_EnSoft_I/blob/main/Diagrama%20do%20Estacionamento.png"
                style="width: 500px; height: 450px; margin: 0 auto;"
            />
        </td>
    </tr>
    <tr>
    </tr>
</tbody>
