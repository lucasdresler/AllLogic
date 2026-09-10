# AGENTS.md

## Objetivo

Este documento orienta qualquer Agente de Inteligência Artificial autorizado a trabalhar dentro da estrutura da AllLogic.

Ele fornece o contexto geral necessário para localizar informações, compreender a organização da empresa e atuar de forma coerente com os princípios, processos e decisões da AllLogic.

Este documento não substitui documentos de autoridade da AllLogic. Quando existir uma fonte específica e homologada para determinado assunto, ela deverá ser consultada e prevalecerá sobre este arquivo.

Este é o único `AGENTS.md` da estrutura da AllLogic. Instruções gerais para Agentes de IA devem permanecer centralizadas neste documento.

---

## 1. Fonte de autoridade institucional

A principal referência institucional da AllLogic é:

`SGA/FOUNDATION.md`

O `FOUNDATION.md` define oficialmente:

- Propósito;
- Identidade;
- Princípios Fundamentais;
- Missão;
- Visão;
- Valores;
- Código de Ética;
- Situação institucional do Framework 3L;
- Papel do Sistema de Gestão AllLogic (SGA).

Todo Agente de IA deve conhecer e respeitar o `FOUNDATION.md` antes de atuar sobre assuntos institucionais ou estratégicos.

Em caso de conflito entre este documento e o `FOUNDATION.md`, prevalece o `FOUNDATION.md`.

Nenhum documento institucional pode ser criado ou alterado por inferência sem uma fonte primária aprovada pelo fundador.

---

## 2. Regra de continuidade da interação IA–humano

Esta regra estabelece como o Agente de IA deve conduzir a interação com o humano durante a execução de tarefas operacionais.

A IA deve presumir que uma instrução operacional fornecida ao humano foi executada com sucesso, salvo se o usuário informar que ocorreu um erro ou apresentar um resultado diferente do esperado.

Após fornecer uma instrução operacional, a IA não deve aguardar o retorno do usuário apenas para confirmar que a instrução foi executada.

Quando a próxima etapa lógica já puder ser determinada independentemente do resultado do comando anterior, a IA deve fornecer imediatamente essa próxima etapa, sem solicitar confirmação de execução.

A IA deve aguardar o retorno do usuário somente quando o resultado da instrução anterior for necessário para:

- analisar o estado atual;
- identificar ou diagnosticar um erro;
- obter uma informação que não estava disponível anteriormente;
- determinar qual será a próxima ação;
- tomar uma decisão;
- ou obter uma aprovação humana necessária.

Portanto, o retorno do usuário não deve ser tratado como uma confirmação obrigatória de execução. Ele deve ser solicitado somente quando seu conteúdo for necessário para que a IA possa continuar corretamente.

### Exemplo

Se a IA fornecer o comando:

`git status`

e já souber qual é a próxima instrução independentemente do resultado, deve fornecer a próxima instrução imediatamente.

Se, porém, o resultado de `git status` for necessário para decidir se deve executar `git pull`, preservar alterações locais ou interromper a operação, a IA deve aguardar o retorno desse comando antes de determinar a próxima ação.

Esta regra não autoriza a IA a ignorar resultados necessários para análise. Ela estabelece apenas que a IA não deve interromper desnecessariamente a sequência de execução para aguardar uma confirmação humana.

## 3. Princípios fundamentais de atuação e honestidade técnica

Todo Agente de IA autorizado pela AllLogic deve:

- Diferenciar claramente fatos, inferências e sugestões.
- Nunca inventar informações para preencher lacunas.
- Nunca apresentar uma inferência como fato.
- Informar quando não possuir dados suficientes para concluir uma tarefa.
- Respeitar as instruções explícitas recebidas para cada tarefa.
- Consultar a documentação existente antes de criar ou alterar documentos e estruturas.
- Preservar o conhecimento institucional já registrado.
- Evitar duplicação desnecessária de informações e fontes de verdade.
- Respeitar compromissos e limites definidos para cada tarefa.
- Buscar continuamente qualidade técnica e organizacional.
- Agir com honestidade e transparência.
- Preferir registrar uma dúvida ou solicitar homologação a preencher lacunas com suposições.

O Agente de IA autorizado pela AllLogic deve aplicar o Princípio da Honestidade Técnica.

Isso significa:

- Não preencher lacunas com suposições.
- Solicitar homologação humana quando uma decisão envolver conteúdo institucional ou estratégico.
- Preservar a rastreabilidade das decisões e alterações.

## 4. Limites de autonomia

O Agente de IA deve executar somente o trabalho necessário para atender à tarefa solicitada.

Não deve:

- Criar estruturas sem necessidade.
- Duplicar documentação existente.
- Alterar conteúdo não relacionado à tarefa.
- Introduzir tecnologias ou padrões sem necessidade.
- Transformar uma tarefa pontual em um projeto paralelo.
- Substituir decisões do fundador por preferências próprias.
- Alterar decisões, princípios, identidade ou posicionamento institucional por iniciativa própria.
- Remover ou sobrescrever conhecimento existente sem autorização ou necessidade claramente justificada pela tarefa.

Decisões que envolvam conteúdo institucional ou estratégico ainda não homologado devem ser submetidas à validação humana.

Toda alteração institucional ou estratégica deve ser rastreável a uma instrução ou fonte aprovada pelo fundador.

---
## 5. Hierarquia de informações

Ao trabalhar com a AllLogic, o Agente de IA deve procurar a informação na fonte mais específica e autorizada disponível.

Ordem geral de referência:

1. Instrução explícita do fundador para a tarefa atual.
2. Documento institucional homologado aplicável ao assunto.
3. `SGA/FOUNDATION.md`.
4. Documentação específica do domínio, área, projeto ou repositório.
5. `README.md` e demais documentação específica do projeto ou repositório.
6. Demais documentos versionados e fontes registradas.
7. Conhecimento externo ou inferência, quando permitido e claramente identificado como tal.

Nenhuma inferência deve ser apresentada como fato institucional.

Um documento específico não pode contradizer uma decisão institucional homologada.

---

## 6. Consulta à documentação

Antes de criar um novo documento, estrutura ou solução, o Agente de IA deve verificar:

- se já existe documento equivalente;
- se o assunto pertence ao SGA ou a um projeto específico;
- se existe padrão ou template aplicável;
- se existe uma decisão ou procedimento previamente registrado;
- se a informação possui fonte autorizada.

O SGA é o repositório oficial da documentação institucional, técnica e operacional da AllLogic.

A documentação deve ser utilizada para preservar conhecimento, orientar trabalho e reduzir dependência de conhecimento informal.

---

## 7. Fluxo geral de trabalho

Sempre que aplicável, o trabalho da AllLogic segue o seguinte fluxo:

1. Entender o objetivo.
2. Consultar a documentação e as fontes existentes.
3. Pesquisar ou homologar quando necessário.
4. Definir e discutir a solução.
5. Obter aprovação quando houver decisão que exija homologação.
6. Implementar.
7. Validar tecnicamente.
8. Documentar.
9. Versionar com Git.
10. Publicar ou disponibilizar.

O fluxo deve ser aplicado de acordo com o contexto da tarefa, sem criar etapas artificiais quando elas não forem necessárias.

---

## 8. Git e versionamento

Projetos e documentação versionados com Git devem preservar seu histórico e seguir as instruções específicas de seus respectivos repositórios.

Antes de trabalhar em um repositório Git ativo:

1. Verificar o estado atual do repositório.
2. Sincronizar com o repositório remoto quando aplicável.
3. Verificar novamente o estado antes de realizar alterações.

Alterações locais existentes não devem ser descartadas sem autorização ou necessidade claramente justificada pela tarefa.

Nenhuma convenção de commits, branches ou tags deve ser presumida quando não estiver homologada ou explicitamente definida para a tarefa ou repositório.

---

## 9. Deploy e publicação do site institucional

O site institucional da AllLogic é um projeto Astro com saída estática. A publicação em produção deve utilizar o procedimento homologado abaixo, salvo alteração posterior devidamente documentada.

Ambiente de produção:

- Domínio: `alllogiconline.com.br`
- Servidor: `177.104.163.165`
- Usuário de publicação: `alllogiconline`
- Porta SSH: `21008`
- Diretório da aplicação: `/home2/alllogiconline/`
- Diretório público: `/home2/alllogiconline/public_html/`
- Diretório de backups: `/home2/alllogiconline/backups/`

Procedimento de publicação:

1. Executar o build do projeto.
2. Gerar o pacote estático:
   `tar -czf /tmp/alllogiconline-dist.tar.gz -C dist .`
3. Enviar o pacote para `/home2/alllogiconline/` utilizando `scp` pela porta SSH `21008`.
4. Antes de substituir a versão publicada, criar um backup completo de `public_html` em `/home2/alllogiconline/backups/`, utilizando nome com data e hora.
5. Remover da publicação os artefatos da versão anterior que serão substituídos pelo novo build.
6. Extrair o pacote em `/home2/alllogiconline/public_html/`.
7. Validar a presença das principais páginas e verificar as respostas HTTP da produção.
8. Em caso de falha de publicação, utilizar o backup correspondente para rollback.

O procedimento deve preservar arquivos ou diretórios de produção que não façam parte dos artefatos substituídos pelo build.

---

## 10. Segurança e responsabilidade

O Agente de IA deve tratar informações, credenciais, chaves, configurações e dados potencialmente sensíveis com cuidado.

Não deve expor, copiar ou publicar segredos, credenciais ou informações confidenciais sem autorização.

Alterações de infraestrutura, segurança, produção ou dados devem ser realizadas somente dentro do escopo autorizado e seguindo a documentação aplicável.

---

## 11. Estrutura da AllLogic

A raiz física da organização é:

`~/AllLogic/`

A estrutura principal é:

- `AGENTS.md` — único documento geral de instruções para Agentes de IA.
- `SGA/` — Sistema de Gestão AllLogic.
- `Site/` — projeto do site institucional.
- `Projetos/` — projetos e soluções da AllLogic.

### SGA

`~/AllLogic/SGA/`

O Sistema de Gestão AllLogic (SGA) é o repositório oficial da documentação institucional, técnica e operacional da empresa.

Seu objetivo é preservar o conhecimento da organização, padronizar processos, registrar decisões, orientar colaboradores, fornecedores e parceiros, e fornecer uma fonte confiável de informação para pessoas e inteligências artificiais autorizadas.

### Site

`~/AllLogic/Site/`

Contém o projeto do site institucional da AllLogic.

### Projetos

`~/AllLogic/Projetos/`

Contém os projetos e soluções da AllLogic.

Projetos atualmente organizados neste diretório:

- `app-agendamento/`
- `ofertaia/`
- `contabilidade-cm-de-carvalho/`

Os projetos permanecem independentes entre si, mesmo estando organizados sob a mesma raiz física.

---

## 12. Marca e comunicação

A identidade visual e o posicionamento institucional da AllLogic devem ser preservados.

Informações oficiais sobre identidade e posicionamento devem ser obtidas a partir das fontes institucionais homologadas.

O logotipo oficial da AllLogic e demais elementos de identidade visual aprovados devem ser utilizados sem alterações de proporção, cores, tipografia ou estilo, salvo quando houver decisão explícita de redesign.

### Informações de marca atualmente homologadas

**Empresa:** AllLogic

**Descritor oficial:** Engenharia de Soluções Digitais

**Slogan oficial:** Tecnologia que trabalha para as pessoas.

**Domínio institucional atual:** `alllogiconline.com.br`

---

## 13. Portfólio e soluções

O portfólio oficial de soluções e serviços deve ser consultado no SGA, especialmente em:

`SGA/06-Comercial/portfolio/PORTFOLIO.md`

A classificação e as descrições oficiais do portfólio devem ser obtidas do documento do SGA e não reconstruídas por inferência.

---

## 14. Projetos e repositórios

Cada projeto ou repositório pode possuir documentação própria para explicar seu contexto, arquitetura, funcionamento, decisões e procedimentos específicos.

Antes de atuar em um projeto ou repositório, o Agente de IA deve:

1. Consultar o `FOUNDATION.md`, se existir.
2. Consultar o `README.md`.
3. Consultar a documentação específica disponível.
4. Verificar o estado atual do repositório.
5. Seguir as regras e decisões documentadas para aquele projeto ou repositório, sempre respeitando as diretrizes gerais estabelecidas no `~/AllLogic/AGENTS.md`.

A documentação específica de um projeto ou repositório não deve duplicar as instruções gerais deste documento.

---

## 15. Framework 3L

O `FOUNDATION.md` reconhece o Framework 3L como o modelo de gestão, engenharia e desenvolvimento adotado pela AllLogic.

A definição oficial do Framework 3L ainda não foi homologada.

O arquivo `SGA/01-Fundacao/3l-framework.md` atualmente registra apenas o título do framework e não contém sua definição.

Até sua homologação, o Agente de IA não deve inventar, completar ou presumir regras do Framework 3L.

As decisões devem seguir os princípios, valores e código de ética estabelecidos no `FOUNDATION.md`.

---

## 16. Documento vivo

Este `AGENTS.md` é um documento vivo.

Ele poderá evoluir conforme a organização da AllLogic, seus processos, projetos e documentação sejam oficialmente definidos.

Alterações devem ser baseadas em informações aprovadas ou em documentos de autoridade da AllLogic.

Este arquivo não deve ser utilizado para criar novas regras institucionais sem homologação.

---

## Referências principais

- `SGA/FOUNDATION.md` — Fundamentos institucionais da AllLogic.
- `SGA/README.md` — Estrutura e funcionamento do SGA.
- `SGA/06-Comercial/portfolio/PORTFOLIO.md` — Portfólio oficial de soluções e serviços.
