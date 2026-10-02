# Info Exe

Bem-vindo à organização oficial da **Info Exe** no GitHub.

Este espaço é utilizado para centralizar o desenvolvimento, manutenção e documentação dos projetos internos e das soluções desenvolvidas para clientes.

## Sobre a Info Exe

A **Info Exe** desenvolve e implementa soluções tecnológicas orientadas às necessidades dos seus clientes, abrangendo áreas como desenvolvimento de software, integração de sistemas, automatização de processos e implementação de soluções de gestão.

Esta organização GitHub funciona como ponto central para a gestão do código-fonte, documentação técnica e colaboração entre os membros da equipa.

## Organização dos Repositórios

Os repositórios encontram-se organizados de acordo com o projeto, produto ou cliente a que pertencem.

Dependendo do projeto, poderão existir repositórios destinados a:

- Aplicações e plataformas internas;
- Desenvolvimento de soluções para clientes;
- Integrações com sistemas externos;
- Scripts e ferramentas de apoio;
- Base de dados e automatizações;
- Documentação técnica;
- Projetos de investigação e desenvolvimento.

Cada repositório deverá possuir o seu próprio `README.md`, onde são documentadas as informações específicas do projeto, incluindo sempre que aplicável:

- Objetivo do projeto;
- Tecnologias utilizadas;
- Estrutura da aplicação;
- Configuração do ambiente de desenvolvimento;
- Processo de instalação;
- Processo de deployment;
- Regras de contribuição;
- Documentação técnica relevante.

## Fluxo de Desenvolvimento

Sempre que aplicável, os projetos seguem um fluxo de desenvolvimento baseado em Git e Pull Requests.

De forma geral:

```text
feature/* ──► dev ──► rel ──► main
                           ▲
hotfix/* ─────────────────┘
```

As branches poderão variar consoante as necessidades de cada projeto, devendo as regras específicas estar documentadas no respetivo repositório.

### Branches principais

- `main` — versão estável e destinada a produção;
- `dev` — integração de novas funcionalidades e correções em desenvolvimento;
- `rel` — preparação e validação de versões antes da passagem para produção;
- `feature/*` — desenvolvimento de novas funcionalidades;
- `fix/*` — correção de problemas;
- `hotfix/*` — correções urgentes sobre versões em produção.

## Issues e Pull Requests

Sempre que possível, as alterações devem estar associadas a uma **Issue**.

As Issues permitem documentar:

- Novas funcionalidades;
- Bugs;
- Melhorias;
- Alterações técnicas;
- Refatorações;
- Problemas de segurança;
- Tarefas de manutenção.

O desenvolvimento deverá ser realizado numa branch própria e posteriormente integrado através de **Pull Request**.

Antes de efetuar merge, deverá ser confirmado que:

- A alteração resolve o problema identificado;
- O código foi testado;
- Não foram introduzidas regressões conhecidas;
- A documentação foi atualizada quando necessário;
- Não existem ficheiros sensíveis ou configurações locais no commit.

## Convenções de Commits

Sempre que possível, deverão ser utilizados commits claros e descritivos, seguindo uma estrutura semelhante a **Conventional Commits**:

```text
feat: adicionar nova funcionalidade
fix: corrigir problema existente
docs: atualizar documentação
refactor: reorganizar código sem alterar comportamento
test: adicionar ou atualizar testes
perf: melhorar desempenho
security: corrigir problema de segurança
chore: tarefas de manutenção
```

Quando existir uma Issue associada, recomenda-se incluir a respetiva referência.

Exemplo:

```text
fix(tickets): corrigir atualização do estado da ocorrência (#42)
```

## Segurança

Nunca deverão ser adicionados aos repositórios:

- Passwords;
- Credenciais de bases de dados;
- Chaves privadas;
- API Keys;
- Tokens de autenticação;
- Certificados privados;
- Ficheiros `.env` com informação real;
- Backups de bases de dados com dados de produção;
- Informação confidencial de clientes.

Os projetos deverão disponibilizar ficheiros de exemplo, como:

```text
.env.example
```

contendo apenas a estrutura necessária para configurar o ambiente.

Qualquer vulnerabilidade ou exposição acidental de informação sensível deverá ser comunicada internamente assim que for identificada.

## Documentação

A documentação faz parte integrante dos projetos.

Sempre que uma alteração introduza novos processos, regras de negócio, configurações ou decisões técnicas relevantes, a documentação correspondente deverá ser atualizada.

Dependendo do projeto, poderão existir documentos como:

```text
README.md
CONTRIBUTING.md
SECURITY.md
DEPLOYMENT.md
CHANGELOG.md
docs/
```

## Boas Práticas

Antes de submeter alterações:

1. Confirmar que a branch está atualizada;
2. Rever as alterações efetuadas;
3. Executar os testes disponíveis;
4. Remover código de debug;
5. Confirmar que não existem dados sensíveis;
6. Criar commits claros e focados;
7. Abrir um Pull Request com uma descrição adequada.

## Projetos

Os projetos existentes nesta organização podem possuir diferentes tecnologias, arquiteturas e processos de desenvolvimento.

As instruções específicas de cada projeto devem ser consultadas diretamente no respetivo repositório.
