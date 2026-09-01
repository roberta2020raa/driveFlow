# DriveFlow — Requisitos Não Funcionais

##  Segurança

**RNF01 — Proteção dos dados financeiros**  
Os dados financeiros de cada usuário devem ser protegidos contra acesso por outros usuários.

**RNF02 — Armazenamento seguro de senhas**  
As senhas dos usuários devem ser armazenadas de forma segura e não devem ser armazenadas em formato que permita sua visualização direta.

**RNF03 — Autenticação de acesso**  
O acesso aos dados financeiros deve exigir autenticação do usuário.

**RNF04 — Sessão do usuário**  
O sistema não deve desconectar automaticamente o usuário após um período de inatividade no MVP.

---

##  Responsividade

**RNF05 — Responsividade**  
O DriveFlow deve funcionar adequadamente em celulares, tablets e computadores.

**RNF06 — Mobile First**  
A interface deve ser projetada seguindo a abordagem **Mobile First**, priorizando a experiência em dispositivos móveis.

A interface deve permitir que o usuário registre e consulte informações financeiras de maneira prática durante sua rotina de trabalho.

---

##  Desempenho

**RNF07 — Velocidade de carregamento**  
As telas do DriveFlow devem apresentar um carregamento rápido, inclusive em conexões mais lentas.

**RNF08 — Velocidade das operações**  
O cadastro, alteração e exclusão de ganhos e gastos devem ocorrer rapidamente, proporcionando uma resposta clara ao usuário.

---

##  Acessibilidade

**RNF09 — Acessibilidade**  
A interface deve considerar usuários com diferentes necessidades visuais, motoras e cognitivas.

**RNF10 — Legibilidade e contraste**  
Os textos e elementos visuais devem apresentar tamanho, contraste e legibilidade adequados.

**RNF11 — Elementos interativos**  
Botões, campos e demais elementos interativos devem ser facilmente identificáveis e utilizáveis.

---

##  Usabilidade

**RNF12 — Facilidade de uso**  
Uma pessoa que nunca utilizou o DriveFlow deve conseguir compreender suas principais funcionalidades sem necessidade de um manual.

**RNF13 — Cadastro simplificado**  
O registro de ganhos e gastos deve exigir poucos passos.

**RNF14 — Clareza das informações**  
As informações financeiras devem ser apresentadas de forma simples e organizada, evitando excesso de informações em uma mesma tela.

---

##  Confiabilidade

**RNF15 — Persistência dos dados**  
Os ganhos e gastos registrados pelo usuário devem ser armazenados de forma que não sejam perdidos durante o funcionamento normal do sistema.

**RNF16 — Atualização do balanço**  
O balanço financeiro deve ser atualizado automaticamente após o cadastro, alteração ou exclusão de um ganho ou gasto.

---

##  Compatibilidade

**RNF17 — Compatibilidade com navegadores**  
O DriveFlow deve ser compatível com os principais navegadores:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

**RNF18 — Compatibilidade no MVP**  
Não haverá navegador ou dispositivo previamente excluído do suporte no MVP.

---

##  Manutenibilidade e evolução

**RNF19 — Estrutura preparada para evolução**  
O sistema deve possuir uma estrutura que permita a inclusão de novas funcionalidades sem a necessidade de reconstrução completa do produto.

Entre as funcionalidades que poderão ser adicionadas futuramente estão:

- Gráficos;
- Controle de combustível;
- Controle de quilometragem;
- Metas;
- Relatórios;
- Notificações.
