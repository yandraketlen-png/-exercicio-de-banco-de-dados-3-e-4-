cria um modelo usando modo DER no estilo br modelo pra mim pra revolver esse problema  Para responder este exércicio, poderão utilizar o software Dia (instalado nos computadores do Laboratório de informática, sala 109), ou utilizar algumas aplicações online, tais como o BR Modelo  - sis4.com, ou o BR modelo web (https://www.brmodeloweb.com/lang/pt-br/index.html), ou Drawdb (https://www.drawdb.app/). 
1 - Um médico trata de pacientes. Do médico deseja-se saber CRM, Nome e suas especialidades. Um paciente, no qual há a necessidade de sabermos seu Nome, Endereço e Idade, é tratado por vários médicos. Um paciente realiza vários tipos de exames. Um tipo de exame, no qual há a necessidade de armazenar seu Número, Data e Descrição, é feito por vários pacientes.

2 - Um médico trata de pacientes. Do médico deseja-se saber CRM, Nome e suas especialidades. O médico solicita exames para vários pacientes. Um paciente, no qual há a necessidade de sabermos seu Nome, Endereço e Idade, é tratado por vários médicos. Um paciente realiza vários tipos de exames, solicitados pelos médicos. Um tipo de exame, no qual há a necessidade de guardar seu Número, Data e Descrição, é feito por vários pacientes a pedido dos médicos.

Exercício 1 — Médico ↔ Paciente (relacionamento Trata, N:N) e Paciente ↔ Tipo de exame (relacionamento Realiza, N:N).

Exercício 2 — Igual ao anterior, mais o relacionamento ternário Solicita, ligando Médico, Paciente e Tipo de exame ao mesmo tempo (representando que o médico pede um exame específico para um paciente específico).

Alguns pontos que você pode querer ajustar ao abrir no BR Modelo:

CRM, Nome (do paciente) e Número estão sublinhados como chave primária de cada entidade — no enunciado não há campo de identificação explícito para paciente, então usei Nome; se preferir, pode trocar por um "Código do paciente" (mais correto na prática, já que nome não é um bom identificador).
Especialidade foi desenhada como atributo multivalorado (elipse dupla), pois um médico pode ter mais de uma especialidade.
As cardinalidades foram marcadas como N:N em todos os relacionamentos, conforme o texto ("vários médicos"/"vários pacientes" nos dois sentidos).
