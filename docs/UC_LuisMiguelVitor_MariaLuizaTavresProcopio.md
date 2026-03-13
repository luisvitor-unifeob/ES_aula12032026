## UC01 — Realizar Login (UC EXEMPLO - FAZER DESSA FORMA PARA TODOS OS CASOS DE USO, NESSE MESMO DOCUMENTO)

### Ator Principal
Usuário

### Objetivo
Permitir que o usuário acesse o sistema.

### Pré-condições
- Usuário deve possuir cadastro ativo.

### Pós-condições
- Sessão iniciada com sucesso.

### Fluxo Principal
1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema autentica o usuário e redireciona para a tela inicial.

### Fluxos Alternativos
- **A1 — Senha incorreta:**  
  O sistema exibe mensagem de erro.

- **A2 — Conta bloqueada:**  
  O sistema impede o login e instrui o usuário a recuperar o acesso.

### RF Relacionados
- (inserir RF aqui)

### RNF Relacionados
- (inserir RNF aqui)

### RN Relacionadas
- (inserir RN aqui)





## UC013 — Emitir Relatório de Inadimplência

### Ator Principal
Gerente

### Objetivo
Identificar alunos inadimplentes.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório gerado.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema processa dados.
3. Sistema exibe resultado.


### Fluxos Alternativos
- **A1 — Nenhum aluno inadimplente:**  
  Sistema informa ausência.

- **A2 — Falha na geração:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN01



## UC014 — Emitir Relatório de Alunos Ativos

### Ator Principal
Gerente

### Objetivo
Listar alunos ativos.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema gera lista.


### Fluxos Alternativos
- **A1 — Nenhum aluno ativo:**  
  Sistema informa ausência.

- **A2 — Falha na consulta:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- Nenhuma




## UC015 — Emitir Relatório de Acessos

### Ator Principal
Gerente

### Objetivo
Consultar histórico de entradas.

### Pré-condições
- Registros existentes.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema compila dados.
3. Exibe histórico.

### Fluxos Alternativos
- **A1 — Nenhum acesso registrado:**  
  Sistema informa ausência.

- **A2 — Falha na consulta:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- Nenhuma




## UC016 — Emitir Relatório de Ocupação de Aulas

### Ator Principal
Gerente

### Objetivo
Avaliar demanda das aulas.

### Pré-condições
- Aulas registradas.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema analisa reservas.
3. Exibe ocupação.

### Fluxos Alternativos
- **A1 — Nenhuma aula cadastrada:**  
  Sistema informa ausência.

- **A2 — Falha na geração:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF05

### RN Relacionadas
- RN02




## UC017 — Enviar Notificação de Vencimento

### Ator Principal
Sistema

### Objetivo
Avisar sobre mensalidade.

### Pré-condições
- Mensalidade próxima do vencimento.

### Pós-condições
- Notificação enviada.

### Fluxo Principal
1. Sistema identifica vencimento.
2. Gera notificação.
3. Envia ao aluno.


### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda nova tentativa.

- **A2 — Dados de contato inválidos: **  
  Sistema exibe erro.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma





## UC018 — Enviar Confirmação de Agendamento

### Ator Principal
Sistema

### Objetivo
Confirmar reserva.

### Pré-condições
- Agendamento realizado.

### Pós-condições
- Aluno notificado.

### Fluxo Principal
1. Sistema registra agendamento.
2. Envia confirmação.

### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda reenvio.

- **A2 — Agendamento cancelado antes do envio:**  
  Notificação não enviada.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma





## UC019 — Enviar Notificação de Avaliação Disponível

### Ator Principal
Sistema

### Objetivo
Avisar liberação de avaliação.

### Pré-condições
- Nova avaliação permitida.

### Pós-condições
- Aluno informado.

### Fluxo Principal
1. Sistema verifica elegibilidade.
2. Envia notificação.

### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda nova tentativa.

- **A2 — Aluno sem contato cadastrado:**  
  Sistema registra erro.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma





## UC020 — Atualizar Situação do Aluno

### Ator Principal
Sistema

### Objetivo
Manter status atualizado.

### Pré-condições
- Pagamento registrado.

### Pós-condições
- Situação regularizada.

### Fluxo Principal
1. Sistema recebe confirmação de pagamento.
2. Atualiza status do aluno.


### Fluxos Alternativos
- **A1 — Falha na atualização:**  
  Sistema mantém status anterior.

- **A2 — Pagamento inconsistente:**  
  Sistema solicita verificação manual.


### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN07



