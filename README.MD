
<body>
  <h1>Levantamento de Requisitos para um Sistema de Controle de Estacionamento</h1>
  <p>Base: Estacionamento do Shopping Patio Chapecó</p>

  <h2>Equipe</h2>
  <p>Andre Gabrielli da Silva, Arthur Couto Mulling e Gustavo Henrique Telo.</p>

  <h1>Descrição do Sistema</h1>
  <p>O estacionamento controla o momento de entrada e saída dos veículos utilizando um cartão que é emitido antes da entrada e recolhido antes da saída. Após a retirada do cartão e entrada do veículo, o sistema contabiliza o tempo em que o veículo permaneceu dentro do estacionamento e cobra uma taxa fixa após 15 (quinze) minutos da entrada.</p>
  <p>Durante a entrada do veículo, as vagas possuem um sensor para monitoramento das vagas ocupadas, mostrando uma luz verde em caso de vaga livre e uma luz vermelha em caso de vaga ocupada. Para a saída do veículo, será necessário pagar a taxa registrada por tempo no cartão, permitindo a devolução do cartão no momento da saída do veículo. Caso contrário, o cartão será recusado na tentativa de saída sem pagamento.</p>

  <section>
    <h2>Perguntas Feitas em Entrevistas/Respostas</h2>
    <table border="1" cellpadding="8" cellspacing="0">
      <thead>
        <tr>
          <th style="width: 25%;">Pergunta</th>
          <th>Resposta</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>
            <h3>O que você acha do estacionamento?</h3>
          </td>
          <td>
            <p>Todos os entrevistados avaliaram o estacionamento como um bom estacionamento sem muitos comentários sobre ele, exceto sobre seu valor, que poderia ser mais barato.</p>
          </td>
        </tr>
        <tr>
          <td>
            <h3>Você acha que o estacionamento poderia melhorar em algo?</h3>
          </td>
          <td>
            <p>Dentre os entrevistados, a grande maioria não apontou nenhuma melhoria, pois achavam o estacionamento bom o suficiente da forma que estava. No entanto, alguns sugeriram que fosse adicionada alguma forma de organização para que os carros possam trafegar pelo estacionamento de forma mais fluida, já que frequentemente há situações de bloqueios devido ao grande fluxo de carros.</p>
          </td>
        </tr>
        <tr>
          <td>
            <h3>Acha que o estacionamento é seguro? Se não, quais motivos e como pode melhorar?</h3>
          </td>
          <td>
            <p>Nesta parte da entrevista, tivemos um resultado de respostas unânime. Todos os entrevistados concordam que o sistema de segurança do estacionamento é muito bom e não acham que precisa de alguma melhoria.</p>
          </td>
        </tr>
    </table>
  </section>

<section>
    <h2>Pontos Críticos</h2>
    <ul>
      <li>Em caso de algum problema ou perda do cartão causará problemas para efetuar o pagamento e consequentemente para a saída do veículo.</li>
      <li>Possível falha no sistema de detecção de vagas disponíveis poderá ocasionar um “falso positivo” onde o sistema identifica uma vaga vazia como ocupada, causando uma possível confusão e atrapalhando a localização de vagas.</li>
    </ul>
  </section>

  <section>
    <h2>Áreas para Melhorias</h2>
    <ul>
      <li>Uma melhoria no sistema de identificação da entrada e saída de veículos, podendo evitar erros com o cartão.</li>
      <li>Organização na procura de vagas dentro do estacionamento a fim de evitar transtornos durante a procura de uma vaga.</li>
    </ul>
  </section>

  <section>
    <h2>Funcionalidades Adicionais</h2>
    <ul>
      <li>Aplicação de um app para mapeamento de vagas disponíveis, mostrando a localização exata da vaga e guiando o motorista para a mesma, assim agilizando e facilitando o uso do estacionamento. Desta forma também criaria uma maior fluidez no tráfego de veículos.</li>
      <li>Criação de um sistema para cadastro e criação de uma conta para o estacionamento, permitindo ao motorista utilizar um sistema de recarga de créditos para pagamento do estacionamento, permitindo que o mesmo não precise parar para pagar o estacionamento e assim somente descontado do crédito da conta. Este sistema funcionaria através de um leitor de placas que identificaria o carro cadastrado na conta do usuário.</li>
      <li>O aplicativo também contaria com um sistema de alerta para avisar o usuário de quanto tempo ele pode ficar estacionado antes que se esgote o crédito do cartão. Em caso de esgotamento, o aplicativo permitirá que o pagamento do tempo adicional seja feito dentro do mesmo, visando praticidade para o usuário. Também podendo contar com descontos para quem possuir cadastro.</li>
      <li>Sistema de feedback para o estacionamento, permitindo críticas e sugestões de melhorias para o estacionamento, assim possibilitando novas melhorias e um maior conforto do cliente.</li>
    </ul>
  </section>

  <section>
    <h2>Requisitos Funcionais</h2>
    <ul>
      <li>Controle de acesso de veículos: O sistema deve registrar a entrada e saída de veículos, monitorando o fluxo no estacionamento.</li>
      <li>Monitoramento da ocupação das vagas: O sistema deve acompanhar em tempo real o status das vagas, indicando quais estão livres ou ocupadas.</li>
      <li>Processamento de pagamento conforme tempo de permanência: O sistema deve calcular automaticamente o valor do pagamento, aplicando uma tarifa fixa após 15 minutos e uma cobrança adicional a cada hora.</li>
      <li>Indicação de rotas dentro do estacionamento: O software deve guiar os motoristas com setas e sinais visuais, levando-os até as vagas disponíveis.</li>
      <li>Relatório de incidentes de segurança: A Equipe de Segurança deve registrar e enviar relatórios de incidentes, como batidas de veículos ou brigas, diretamente pelo sistema.</li>
      <li>Relatório de manutenção: A Equipe de Manutenção deve registrar e enviar relatórios sempre que houver necessidade de reparos ou ajustes no estacionamento.</li>
    </ul>
  </section>

  <section>
    <h2>Requisitos Não Funcionais</h2>
    <ul>
      <li>Desempenho: O sistema deve processar e atualizar as informações em tempo real, com respostas imediatas (menos de 1 segundo) para monitoramento e transações.</li>
      <li>Segurança: Todos os dados, incluindo informações de pagamento e relatórios de incidentes, devem ser criptografados para garantir a privacidade e segurança.</li>
      <li>Escalabilidade: O software deve ser capaz de gerenciar um número crescente de veículos, transações e relatórios sem perda de desempenho.</li>
      <li>Portabilidade: O sistema deve ser acessível em dispositivos móveis para permitir que administradores e equipes monitorem e registrem atividades remotamente.</li>
      <li>Usabilidade: A interface do sistema deve ser fácil de usar, permitindo que os administradores e equipes operem sem a necessidade de treinamento especializado.</li>
      <li>Manutenção: O sistema deve ser modular, facilitando a implementação de atualizações e manutenções sem interrupção do serviço.</li>
      <li>Auditoria: O sistema deve manter logs detalhados de todas as operações e transações financeiras, armazenados por um período mínimo de 12 meses.</li>
    </ul>
  </section>


</body>

