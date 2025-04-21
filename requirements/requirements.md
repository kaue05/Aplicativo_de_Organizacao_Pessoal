# Requisitos Funcionais

## Requisito Funcional 1: Cadastro de Usuário

**Descrição**: O sistema deve permitir que o usuário se cadastre fornecendo um e-mail e uma senha.

### Requisitos:
- O sistema deve validar se o e-mail fornecido é único.
- O sistema deve validar se o formato do e-mail está correto.
- A senha deve ser armazenada de forma segura, utilizando hashing.
- O sistema deve enviar um e-mail de confirmação para o endereço informado.
- O sistema deve garantir que o e-mail de confirmação tenha um link válido por no máximo 24 horas.

### Fluxo de Funcionamento:
1. O usuário acessa a página de cadastro.
2. O usuário insere o e-mail e senha nos campos correspondentes.
3. O sistema valida o e-mail e a senha.
4. Se os dados forem válidos, o sistema envia um e-mail de confirmação para o endereço informado.
5. O usuário deve confirmar o e-mail clicando no link recebido.
6. O sistema ativa a conta e permite o login.

---

## Requisito Funcional 2: Alteração de Usuário

**Descrição**: O sistema deve permitir que o usuário altere seus dados pessoais.
(como nome, email, senha etc).

### Requisitos:
- O sistema deve validar se o novo e-mail informado não está em uso por outro usuário.
- O sistema deve validar se o formato do e-mail é válido.
- O sistema deve solicitar autenticação (senha atual) para alterar o e-mail ou senha.
- A senha deve ser armazenada de forma segura, utilizando hashing.
- O sistema deve informar ao usuário que seus dados foram atualizados com sucesso.

### Fluxo de Funcionamento:
1. O usuário acessa a página "Conta".
2. O usuário altera os campos que deseja.
3. O sistema valida o e-mail e a senha.
4. Se os dados forem válidos, o sistema exibe uma mensagem de confirmação de alteração.
5. O sistema altera os campos no banco de dados.


1. O usuário acessa a página de cadastro.
2. O usuário insere o e-mail e senha nos campos correspondentes.
3. O sistema valida o e-mail e a senha.
4. Se os dados forem válidos, o sistema envia um e-mail de confirmação para o endereço informado.
5. O usuário deve confirmar o e-mail clicando no link recebido.
6. O sistema ativa a conta e permite o login.
---

## Requisito Funcional 3: Cadastro de Tarefas

**Descrição**: O sistema deve permitir que o usuário crie tarefas.

### Requisitos:
- O sistema deve validar se o título da tarefa não está vazio.
- O sistema deve permitir a alteração do nível de urgência da tarefa.
- O sistema deve permitir a inclusão de descrição, data da tarefa, horário da tarefa e som de notificação (opcional).
- O sistema deve registrar a data e hora da criação da tarefa.
- O sistema deve associar a tarefa ao usuário autenticado.
- O sistema deve permitir associar a tarefa a um grupo (opcional).

---

## Requisito Funcional 4: Alteração de Tarefas

**Descrição**: O sistema deve permitir que o usuário edite tarefas existentes.

### Requisitos:
- O sistema deve validar se a tarefa pertence ao usuário logado.
- O sistema deve permitir alterar o título, descrição, data, hora, som da notificação e grupo da tarefa.
- O sistema deve registrar a data da última modificação da tarefa.
- O sistema deve informar ao usuário quando a tarefa for alterada com sucesso.

---

## Requisito Funcional 5: Exclusão de Tarefas

**Descrição**: O sistema deve permitir que o usuário exclua tarefas.

### Requisitos:
- O sistema deve validar se a tarefa pertence ao usuário autenticado.
- O sistema deve solicitar uma confirmação antes da exclusão da tarefa.
- O sistema deve remover a tarefa de forma definitiva do banco de dados.
- O sistema deve atualizar os dados de pontuação do usuário, se aplicável.
- O sistema deve informar que a exclusão foi realizada com sucesso.

---

## Requisito Funcional 6: Marcação de Tarefas Concluídas

**Descrição**: O sistema deve permitir que o usuário marque tarefas como concluídas.

### Requisitos:
- O sistema deve validar se a tarefa pertence ao usuário logado.
- O sistema deve alterar o status da tarefa para "concluída".
- O sistema deve registrar a data e hora da conclusão.
- O sistema deve atualizar a pontuação do usuário.
- O sistema deve permitir que a tarefa seja desmarcada, se necessário.

---

## Requisito Funcional 7: Cadastro de Grupo de Tarefas

**Descrição**: O sistema deve permitir que o usuário crie grupos de tarefas.

### Requisitos:
- O sistema deve validar se o nome do grupo não está vazio.
- O sistema deve permitir criar grupos com nome e cor personalizados.
- O sistema deve associar o grupo ao usuário logado.
- O sistema deve informar quando o grupo for criado com sucesso.
- O sistema deve permitir alterar ou excluir grupos posteriormente.

---

## Requisito Funcional 8: Pontuação sobre Tarefas

**Descrição**: O sistema deve calcular e exibir uma pontuação com base nas tarefas realizadas.

### Requisitos:
- O sistema deve adicionar pontos quando uma tarefa for concluída.
- O sistema deve remover pontos se a tarefa for desmarcada ou excluída.
- O sistema deve exibir a pontuação total atual do usuário.
- O sistema deve permitir que o usuário visualize um histórico de pontuação (opcional).
- O sistema deve recalcular a pontuação em caso de alterações nas tarefas.

---

## Requisito Funcional 9: Relatório de Desempenho

**Descrição**: O sistema deve permitir que o usuário visualize seu relatório de desempenho ou progresso nas tarefas.

### Requisitos:
- O sistema deve exibir o total de tarefas criadas, concluídas e pendentes.
- O sistema deve exibir gráficos ou tabelas com o desempenho ao longo do tempo.
- O sistema deve permitir filtrar o relatório por data ou grupo de tarefas.
- O sistema deve calcular a taxa de conclusão de tarefas do usuário.
- O sistema deve atualizar o relatório em tempo real conforme as tarefas são modificadas.

---

## Requisito Funcional 10: Segurança de Informações

**Descrição**: O sistema deve armazenar as informações dos usuários e suas tarefas de forma segura.

### Requisitos:
- A senha do usuário deve ser armazenada com criptografia (hashing).
- O sistema deve utilizar autenticação segura (Firebase Auth).
- O acesso aos dados deve ser restrito ao usuário autenticado.
- As regras de segurança do banco de dados devem impedir acesso indevido.
- As requisições devem ser feitas por HTTPS para proteger os dados em trânsito.

-------