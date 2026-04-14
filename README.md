# codex-setup-practices

> Laboratório da **Plasma Clara Nexus** pra treinar setup, disciplina de repo e documentação que não enrola. 🔥

## O que é isso

Este repositório é um campo de prática pra setup de ambiente, rotina de contribuição e escrita de documentação útil.
Nada de README Jesules vazio que só existe pra dizer que existe. Aqui a ideia é: **clareza, contexto e rastreabilidade**.

## Por que esse repo existe

- Evitar onboarding quebrado e improviso de última hora.
- Centralizar padrões mínimos de colaboração.
- Praticar fluxo limpo: editar, revisar, testar, commitar e abrir PR.

## Estrutura atual

- `README.md`: visão geral, propósito e instruções de uso.
- `InitialSetup.txt`: script de bootstrap (AGENTS + git-meta + kubo) com fallback para erro HTTP 403 ao resolver versão do kubo.
- `for-AGENTS.md`: referência rápida com lembretes para agentes e contribuições assistidas.

## Regras de contribuição (sem maquiagem)

1. Leia a documentação antes de sair codando no susto.
2. Faça mudanças pequenas e explicáveis.
3. Escreva commits com intenção clara.
4. Abra PR com contexto e impacto real.
5. Se algo quebra, documenta o estrago e o caminho de correção.

## Fluxo sugerido

```bash
git checkout -b chore/improve-readme
# edita arquivos
git add README.md for-AGENTS.md
git commit -m "docs: expandir README e referenciar guia para agentes"
```

## Nota da Plasma

Tecnologia sem documentação vira feudo.
Automação sem contexto vira teatro.
E colaboração sem regra mínima vira DAO de ego com governance de gritaria.

Então sim: escrever README decente também é infraestrutura. 💥


## Setup rápido

```bash
bash InitialSetup.txt
```

Se a infra bloquear a descoberta da versão mais recente do kubo, o script usa uma versão fallback automaticamente (configurável por `KUBO_FALLBACK_VERSION`).
