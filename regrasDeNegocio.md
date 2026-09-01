# DriveFlow — Regras de Negócio

##  Usuário

**RN01 — Cadastro por e-mail**  
Um usuário pode possuir mais de uma conta no DriveFlow, desde que cada conta utilize um e-mail diferente.

**RN02 — Dados obrigatórios**  
Para criar uma conta, o usuário deve informar nome, e-mail, senha e telefone.

**RN03 — E-mail único**  
Não deve ser permitido cadastrar uma nova conta utilizando um e-mail já associado a outra conta.

**RN04 — Confirmação de exclusão**  
A exclusão da conta deve exigir uma confirmação do usuário antes de ser realizada.

---

##  Veículos

**RN05 — Múltiplos veículos**  
Um usuário pode cadastrar mais de um veículo.

**RN06 — Dados do veículo**  
O cadastro de um veículo deve conter marca, modelo, ano, placa e quilometragem.

**RN07 — Compartilhamento de veículo**  
Um mesmo veículo pode estar associado a mais de um usuário.

---

##  Aplicativos

**RN08 — Múltiplos aplicativos**  
O usuário pode cadastrar quantos aplicativos desejar.

**RN09 — Aplicativos utilizados**  
Os aplicativos cadastrados representam as plataformas utilizadas pelo usuário para realizar seu trabalho.

**RN10 — Exclusão de aplicativo com registros vinculados**  
Um aplicativo não poderá ser excluído enquanto possuir ganhos registrados relacionados a ele.

---

##  Ganhos

**RN11 — Dados do ganho**  
Cada ganho registrado deve conter valor, data, aplicativo, quantidade de corridas e observação.

**RN12 — Valor mínimo do ganho**  
O valor de um ganho deve ser sempre maior que zero.

**RN13 — Alteração de ganhos**  
O usuário pode editar um ganho já registrado.

**RN14 — Exclusão de ganhos**  
O usuário pode excluir um ganho já registrado.

---

##  Gastos

**RN15 — Categorias de gastos**  
O MVP deve disponibilizar as categorias:

- Combustível
- Alimentação
- Manutenção
- Outros

**RN16 — Categoria opcional**  
O preenchimento da categoria não será obrigatório para o registro de um gasto.

**RN17 — Dados obrigatórios do gasto**  
Cada gasto deve conter valor, data, categoria e descrição.

**RN18 — Alteração de gastos**  
O usuário pode editar um gasto já registrado.

**RN19 — Exclusão de gastos**  
O usuário pode excluir um gasto já registrado.

---

##  Balanço financeiro

**RN20 — Cálculo do balanço**  
O balanço financeiro deve ser calculado pela diferença entre o total de ganhos e o total de gastos.

**Fórmula:**

> **Balanço = Total de ganhos − Total de gastos**

**RN21 — Períodos de consulta**  
O usuário poderá consultar seu balanço financeiro por:

- Dia
- Semana
- Mês
- Período personalizado

**RN22 — Ausência de registros**  
Quando não houver ganhos ou gastos registrados no período consultado, o sistema deve apresentar o valor de **R$ 0,00**.

**RN23 — Balanço negativo**  
O balanço financeiro poderá apresentar valores negativos quando os gastos forem superiores aos ganhos.
