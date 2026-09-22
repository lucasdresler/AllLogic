# Git e GitHub — AllLogic

## Objetivo

Registrar as configurações e padrões comuns de Git e GitHub utilizados pelos projetos da AllLogic.

Este documento registra informações de configuração e operação compartilhadas entre os projetos. Não contém tokens, senhas, chaves privadas ou outras credenciais secretas.

## Identidade Git

- **Nome:** Lucas Dresler
- **E-mail:** lucasdresler@live.com

A identidade acima é a identidade Git global utilizada nos projetos da AllLogic.

## GitHub

- **Conta:** `lucasdresler`
- **Plataforma:** GitHub
- **Protocolo das operações Git:** SSH
- **Host:** `github.com`
- **Porta SSH:** `22`

A autenticação SSH foi validada com sucesso em 21/09/2026.

## GitHub CLI

O GitHub CLI (`gh`) está instalado e autenticado na conta `lucasdresler`.

- Conta ativa: `lucasdresler`
- Protocolo das operações Git: SSH

Tokens de autenticação não devem ser registrados neste documento.

## Repositórios oficiais

| Projeto | Repositório | Branch principal |
|---|---|---|
| SGA | `git@github.com:lucasdresler/alllogic-sga.git` | `main` |
| Site Institucional | `git@github.com:lucasdresler/alllogic-site.git` | `main` |
| AllLogic Scheduler | `git@github.com:lucasdresler/alllogic-scheduler.git` | `main` |
| OfertaIA | `git@github.com:lucasdresler/ofertaia.git` | `main` |

## Fluxo de versionamento

O fluxo padrão de versionamento deve preservar alterações rastreáveis e separadas por finalidade.

### Antes do versionamento

1. Validar a alteração.
2. Executar `git status`.
3. Revisar `git diff`.
4. Executar `git diff --check`.
5. Confirmar que somente os arquivos esperados serão versionados.

### Versionamento

1. `git add` dos arquivos necessários.
2. Revisar o estado do staging.
3. Criar o commit com mensagem descritiva.
4. Enviar para o repositório remoto com `git push`.
5. Confirmar o estado final do repositório.

### Regra geral

Não versionar credenciais, tokens, senhas, chaves privadas ou arquivos que contenham segredos.

## Segurança

Não registrar neste documento:

- tokens do GitHub;
- senhas;
- chaves privadas SSH;
- credenciais de serviços;
- conteúdo de arquivos `.env` com dados secretos.

A documentação deve registrar apenas a configuração necessária para compreender e reproduzir o fluxo de versionamento, sem expor segredos.

## Manutenção

Este documento deve ser atualizado quando houver alteração relevante na configuração comum de Git/GitHub da AllLogic, na conta utilizada, no protocolo de acesso ou na organização dos repositórios.

Alterações específicas de um projeto devem permanecer documentadas na documentação daquele projeto quando não forem aplicáveis aos demais.
