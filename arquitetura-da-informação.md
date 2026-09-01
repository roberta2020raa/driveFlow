# DriveFlow — Arquitetura da Informação

## Objetivo

Organizar as principais informações e funcionalidades do DriveFlow de forma que o usuário consiga encontrar e utilizar os recursos do sistema de maneira simples e intuitiva.

A arquitetura foi pensada considerando principalmente o contexto de uso do motorista de aplicativo, que poderá utilizar o produto durante sua rotina de trabalho pelo celular.

---

## 1. Home

A Home será a primeira tela apresentada ao usuário após o login.

A informação principal será o **saldo do mês**, acompanhado de um resumo dos ganhos e gastos.

Também estarão disponíveis ações rápidas para:

- Registrar ganho;
- Registrar gasto.

### Decisão

O saldo será apresentado com a possibilidade de **ocultar ou revelar o valor através de um ícone de olho**.

### Justificativa

Como o DriveFlow trabalha com informações financeiras, o usuário deve poder escolher se deseja deixar os valores visíveis na tela.

---

## 2. Navegação principal

O DriveFlow terá uma navegação principal para permitir o acesso às áreas essenciais do sistema.

A estrutura inicial será:

- Home
- Movimentações
- Dashboard
- Perfil

Como o produto será desenvolvido seguindo uma abordagem **Mobile First**, a navegação será posteriormente estudada considerando o uso em dispositivos móveis.

---

## 3. Movimentações

Ganhos e gastos serão agrupados dentro de uma área chamada **Movimentações**.

### Estrutura

```text
Movimentações
├── Ganhos
└── Gastos
```

### Justificativa

Ganhos e gastos representam movimentações financeiras e, portanto, serão tratados como partes de uma mesma área do produto.

---

## 4. Dashboard

O Dashboard será uma área destinada à **análise das informações financeiras**.

Enquanto a Home apresenta um resumo rápido da situação financeira, o Dashboard terá como objetivo permitir uma análise mais detalhada.

Poderá apresentar futuramente:

- Gráficos;
- Gastos por categoria;
- Comparações entre períodos;
- Evolução dos ganhos;
- Evolução dos gastos.

---

## 5. Perfil

O Perfil será responsável pelas configurações e informações relacionadas ao usuário.

### Estrutura inicial

```text
Perfil
├── Dados pessoais
├── Veículos
└── Aplicativos
```

### Justificativa

Durante o cadastro inicial, o usuário fornecerá seus dados pessoais, veículos e aplicativos utilizados.

Após a criação da conta, essas informações poderão ser alteradas posteriormente através do Perfil.

---

## 6. Cadastro inicial

O cadastro será estruturado em etapas para coletar as informações necessárias para iniciar a utilização do DriveFlow.

```text
Cadastro
   ↓
Dados pessoais
   ↓
Veículo
   ↓
Aplicativos
   ↓
Conta criada
   ↓
Home
```

---

## 7. Estrutura geral

```text
DriveFlow
│
├── Home
│   ├── Saldo
│   ├── Ganhos
│   ├── Gastos
│   ├── Registrar ganho
│   └── Registrar gasto
│
├── Movimentações
│   ├── Ganhos
│   └── Gastos
│
├── Dashboard
│   └── Análises financeiras
│
└── Perfil
    ├── Dados pessoais
    ├── Veículos
    └── Aplicativos
```

## Princípios considerados

- Simplicidade;
- Facilidade de navegação;
- Mobile First;
- Acesso rápido às informações financeiras;
- Redução da quantidade de passos para tarefas frequentes;
- Organização clara das funcionalidades.
