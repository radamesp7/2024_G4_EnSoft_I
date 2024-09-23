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
        <td>Criação de um sistema para cadastro e criação de uma conta para o estacionamento, permitindo ao motorista utilizar um sistema de recarga de créditos para pagamento do estacionamento, permitindo que o mesmo não precise parar para pagar o estacionamento e assim somente descontado do crédito da conta. Este sistema funcionaria através de um leitor de placas que identificaria o carro cadastrado na conta do usuário.</td>
      </tr>
      <tr>
        <td>O aplicativo também contaria com um sistema de alerta para avisar o usuário de quanto tempo ele pode ficar estacionado antes que se esgote o crédito do cartão. Em caso de esgotamento, o aplicativo permitirá que o pagamento do tempo adicional seja feito dentro do mesmo, visando praticidade para o usuário. Também podendo contar com descontos para quem possuir cadastro.</td>
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
        <td>Indicação de rotas dentro do estacionamento</td>
        <td>O software deve guiar os motoristas com setas e sinais visuais, levando-os até as vagas disponíveis.</td>
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
                src="https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=C%C3%B3pia%20do%20Diagrama%20do%20Estacionamento.html#R%3Cmxfile%3E%3Cdiagram%20name%3D%22P%C3%A1gina-1%22%20id%3D%222JnSQlSYLmU3ISGfXkrO%22%3E7Vzrc6M2EP9rPNN%2BSAchEPhjXpd2pulcL9f27lNHMYqtKSAfiLz%2B%2BkqAMELEdjjzcC7pTA%2BtQJjd3z60uzCD59HjVYLXq2sWkHBmW8HjDF7MbPlniX8k5amgeHNUEJYJDQqStSHc0GdSEIGiZjQgaUkrSJyxkNO1TlywOCYLrtFwkrAH%2FbQ7FgYaYY2XxCDcLHBoUv%2BhAV8VVN%2F2NvRfCV2u1J0BmhczEVYnl0%2BSrnDAHmokeDmD5wljvDiKHs9JKJmn8%2BXDC7PVD0tIzPe54PTsG7u2PxP%2FN259%2BOPfz%2Bntc3ACyl97j8OsfOKZjUKx4FlA78XhUh7e%2FHbz%2BfL6VM2Ie9Qmy6fjT4pl6QONQhyL0dnDinJys8YLOfUgECJoKx6FYgTE4R0Nw3MWsiS%2FEN658j9JZzGv0Ys%2FQU95wv4jtRmU%2F8kZxVyr%2BkV1zpTMuicJJ481UsmpK8IiwpMncUo5e%2BJ6pYSflGD9YvywQQEALiyIqxoE5rAUOC6ht6xWr274SUAVx0vBsc0dfYD0OzqWcUffMu%2FXvB0OOUlizMkZy%2BIgrWNCHNQedkPKkdKOmg9f%2F8RPl7dXz3bM7s%2Bv2DK1nRNogOYTWVIhHZwI8mUsDgJs4EIsLLR2D1iY8tuO3b2lWsmrZLELgClUu4XH%2FhaRasx9LSdtg5M59yQbYyb%2BR1KOF5TFOBK8YEfAUgjHZqnyHDWeXpGCpQuc8Nk5nJ3CKbLScWwdnS0GYGBWAoOVJt%2Fi4FT6WTFiaxJLx4HTFQlKbtUYl0h7lE9II00eKf9SO%2F4qj39xy9HFY23q4kkNhG48fSmXywe1q%2BRwc1k%2B2lwXfKDy0V9wD1sFmLIsWZA9AMdxsiR8t9kkgRZymHioydttEbeiJSTEnN7rgcoWp%2FORUfHAFdxs5DTg5glGaosUj15eVw8tjKV0Z%2BlAv7lUwRxjqUN5JOAYSD0XQUSu9dKOchKtp6jzvgd0zs3tsT2S6ZIOr%2FOVnn%2Btq%2Fl2na%2Bp%2Bde6CRhF5%2BGeKm9PSuUdqIeYjjvvqvKO31jKMpbqWeVttwWoxQZF7h80xKJvGVMTJ2m%2ByRS7GQtY68ccHGpe7Wk%2BERzS58p6iF2eCsCsW5wSsddQAVppWDaBmpyqtknFD3lhnzS%2B9fGUZSmFaKvN%2BXjWBxlCvcFUyiE4inB47ulO1bYcpRbj8dTc44v9J7klxxcSQwRHZiZsS5i87B5jludBpu4ehVolvOHSc9oUwmaF34k4UejpO17HMYLdvePmRpKpZamenahjxs1%2Fk4Te0QUufZ%2BAAc9SZYCnbS6Q6zT46Y1sLhwzVXZwcwFqxgLsaSxeYypGU3y1qZuo4rvA7az4%2Fs6l%2Blb8tui5R2Du68WOApjOtIDpwAaa3M7AdBsBF7J69Eit0jI3AH%2BlWe5yQEKZdEQ%2FRYyzhArHlP5sYDZd4bU8zKLwdMFlnehM%2Bg%2Fhz8Lf8S0JP7KUcrGDEKfcMs5ZVDvhNKRLOcFZw2GxjIc0JudVjbED%2Bl5RewKOnhRq30TAFkCh3sJer4u5eG2kuyv9KwYfRXQiHokkWy2H1Z%2Fl2AbaI0sHnYBGyVEETF0NB%2FQbmIVgaI9mWo5JQ3Rn1WI0kLpTR2lHjAIEty%2FUN0LfjehB8DmtfMAbwqd%2FWHx2tHuHw%2FVoCEWTQqiNdN8MPdTRyTd2wFU6diCAugP3I%2ByZTZlUN4J9pG7eUQ12VQ9BYy%2Bzd2US6QvBZnKvb5AOkPIbokJwaGCqpMk7MMcCppnrPzgwjy3lp2LJYwOl22i7RK7XDZSo4dKBP2zM6XbatQ9gLcGYsATHaiuNTHTHSNOz9M4U1%2FYHhSUwt0JXOMExz3tRZCX0LovrnSjWgiUJyY%2FyQmlKU06iSTbBO3rR2UOlxo3XoGJ2bB%2Bsk%2BtayCxvdJH17JQsMyHEvJrgSYJ8%2F4IlSxzTZ1xQq%2BJ2e%2F%2F9sXR2wUYqwUMDdiG1PoOpUJffMrqWEghIi2waLH0DdR3H0uO%2FOTK77YYt6hw4Y961FamLmx4g2%2BPv64OtSftgD3T2waixUG8%2BuF1Q6lXKF21GhOOMk7hhud%2Be5QDqrYDKcpgvWQ1rOTp1jxw2UN9axxgs1bEdubtbnPxJ2Q4bNGJDd97Ndjhza%2FtCPcfvKqatAfSaxVSof97Uv05ISmpxYG5N7gldZOEU%2Bxrdxm7Id4YL5trZa%2BY4L1WknEyQgXYjXeKPveVBnXJx76W2F5E4EQN6uGKw7%2Bg6D1x7WAs6dIPoDtB9B8C2Amc3wuxJIcwBjRqs1zHz69l6szxU9YGhAGbuPk%2FlpytyB7156wDnpyynmEnznLnGQWfst%2BeQ2WC0YWmcRSRhVbAjWJrzl6ZrVkRCFyIASo%2BAzUCNx%2BNzp0aZ%2FmzjCB2GW03lbps6rQYZR%2F1whTDYMIV7t88Da%2FtCfdvUAd5OfNvA9CYFTAR34Gn%2FMm8j99wIGnrGpdda4cGRdCFlRaU%2BovEizKSbKolL7ZT2motwJlyHLy6TdwuSl4DMrF5Eg0BefpaQlD7j23wpCb%2B15EPOGfds5l7ItTLOimpTvrT%2BIbJSjepfMytJCRNxTJFb7DVBaAM9lmt78VElDeowtdHLiPwuD%2BmZ%2BZcfTeCgV4nDRvTutgSfw0q8re3tB5B4bxJ25q6u056Z9RtWwm05q3cJf4cONyQMVJp3NAm3FYR%2FAAnXrLbsqOrze19I38sK%2Bba82tmX0FsfoiVnEEQ0zj%2FnGTDB89l%2BH98Zs876%2Bu%2B7ekDf8qGWpMKwJdUDVwQm%2BPpiKaWduf8SkUf2PcUTBKp35avPOqCu79OeABs0V7PgwV6pFcPNl6eL0zff74aX%2FwM%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E"
                style="width: 500px; height: 450px; margin: 0 auto;"
            />
        </td>
    </tr>
    <tr>
    </tr>
</tbody>
