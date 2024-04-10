# Projeto Academia

### HU (história do usuário) - Elicitação

O cliente está tendo problemas relacionados com a superlotação de sua academia. Para isso, ele precisa de uma solução para controlar os convites e o monitoramento da quantidade de pessoas malhando no certo horário. Exemplificando, estes dois fatores, que são os principais problemas para superlotação, precisam ser solucionados. 

<br>

### Papeis

- alunos da academia
- funcionários da recepção

<br>

### Narrativa Livre

1. O aluno vai até a recepção para fazer sua matrícula na academia.
2. O aluno mostra seu interesse em contratar o serviço.
3. O recepcionista orienta o cliente em relação ao aplicativo e o funcionamento da academia.
4. O recepcionista apresenta o contrato para o aluno após mostrá-lo o interior da academia.
5. Após feito o contrato e concluída a matrícula, o aluno já tem acesso ao aplicativo e à academia.
6. Ao desejar ir à academia o aluno poderá consultar o aplicativo, onde encontrará todas as informações necessárias para que faça o uso da academia, são elas: horário de aulas, treino montado pelo professor da academia e superlotação da academia.

<br>

### Requisitos

O cliente perguntou como funcionará o sistema em geral, em relação da matrícula do aluno e o contrato.

A matrícula e o contrato deverão ser feitos na recepção, para ter um melhor controle dos alunos e um padrão. Dessa forma, é possível explicarem com mais detalhes as partes importantes do contrato e da matrícula

O cliente perguntou como poderíamos fazer para tentar solucionar o problema da superlotação. Disse que já possui um aplicativo para sua academia com as seguintes abas: treino, horários de aulas, financeiro e contrato.

Falamos que era possível criar uma nova aba em seu aplicativo, a “lotação” . Dentro, será possível visualizar em um gráfico quais são os horários de picos da academia e quantas pessoas estão lá dentro. Para realizar esta funcionalidade, demos a ideia de utilizar as catracas como modo de contagem, assim, quando entrar alguma pessoa, o contador atualiza os dados da quantidade de pessoas presentes na academia, e a mesma coisa, quando alguém sair.

O cliente gostaria de saber como os personais entrariam sem alterar na contagem da superlotação(no aplicativo), já que eles não fazem o uso dos aparelhos. 

Dissemos que é possível fazer a entrada destes pela porta de funcionários, onde não contaria como uma pessoa que utilizará os aparelhos.

O cliente gostaria fazer a questão dos convites remotos, para que a recepção não fique sobrecarregada e consigam tratar apenas dos assuntos mais importantes.

Utilizaremos do mesmo principio da criação de uma nova aba de “convites” no aplicativo. O aluno matriculado na academia realizará o cadastro do convidado que deseja levar e assim gerar um QRcode único para que o convidado possa entrar na academia. Este, após gerado, só poderá ser utilizado em até 24h apenas uma vez na catraca.

O cliente perguntou como conciliaria em relação à superlotação e os convites

Definiremos um termo de contrato onde só poderão gerar os convites fora de horário de pico. Dessa forma no aplicativo(na aba convites) ficará restrito a geração dos convites para minimizar a superlotação , visto que , a prioridade do cliente são somente seus alunos matriculados.

<br>

### Requisitos Funcionais e não Funcionais

**RF01:** “O sistema deverá ter uma aba para realizar a matrícula do aluno”

**RF02:** “Dados básicos, como nome, e-mail, endereço, cpf, contato de emergência, sexo, a definição da senha e data de nascimento deverão ser preenchidos”

**RF03:** “Na aba de login, deverá ter dois campos para inserir os dados, a matrícula ou cpf e senha”

**RF04:** “O sistema deverá ter uma aba para visualizar o contrato e aceitar os termos”

**RF05:** “O sistema tem abas já existentes, que são:  treino, horários de aulas, financeiro e contrato”

**RF06:** “Na aba de treino, é possível visualizar os exercícios propostos pelo professor da academia”

**RF07:** “Na aba horários, é possível visualizar todas as aulas da academia”

**RF08:** “Na aba financeiro, é possível realizar o pagamento das mensalidades, gerando um boleto e ver se está em débito”

**RF09:** “Na aba de contrato, é possível visualizar todo o contrato proposto pela academia”

**RF10:** “O sistema passará a ter duas novas abas: lotação e convites”

**RF11:** “Na aba lotação será possível visualizar quantas pessoas presentes na academia”

**RF12:** “Aparecerá uma mensagem para saber se é recomendado ir na academia naquele horário, devido sua lotação”

**RF13:** “Na aba de convites, é possível preencher dados básicos do convidado, como nome e cpf, para gerar o QRCode”

**RF14:** “Se houver superlotação, a tela de convites será automaticamente bloqueada”

<hr>

**RNF01:** “Disponibilidade do sistema em 98% do tempo”

**RNF02:** “Catraca com funcioanlidade de entrada e saída”

**RNF03:** “Backup do sistema realizado todos os domingos”

**RNF04:** “criptografia dos dados do banco de dados”

**RNF05:** “Sistema operalizado no Windos”

**RNF06:** “Banco de dados será na linguagem de MySQL”

<br>

### Regras de Negócio

**RN01:** “Cada CPF só pode ter uma matrícula vinculada”

**RN02:** “Os cadastrados devem ter CPF válidos.”

**RN03:** “Uma matrícula não poderá ser realizada sem que um recepcionista esteja logado no sistema”

**RN04:** “O sistema de caixa deve registrar as matrículas”

**RN05:** “As senhas utilizadas no sistema devem conter letras maiúsculas, minúsculas, números e caracteres especiais.”

**RN06: “**A utilização da academia só fica disponível após aceitar os termos”

**RN07:** “Só é atualizado o débito após realizado o pagamento do boleto”

**RN08:** “Apenas serão aceitos pagamentos feitos por boleto”

**RN09: “**As movimentações de entrada e saída da academia devem ser registradas”

**RN10:** “O aluno pode retirar até 5 convites por mês”
