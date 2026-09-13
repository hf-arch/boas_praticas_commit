## Convenção de Commits e Branches

Este repositório foi desenvolvido como parte das atividades realizadas durante a aula de CI/CD (Integração Contínua e Entrega Contínua) do curso de Desenvolvimento de Software.

O objetivo deste projeto é documentar e aplicar boas práticas relacionadas à utilização de commits e branches, estabelecendo uma convenção que facilite a organização, manutenção e compreensão do histórico de alterações em um projeto de software.

### 📚 Referência

A estrutura e parte das convenções apresentadas neste repositório foram desenvolvidas com base e inspiração no repositório [Padrões de Commits](https://github.com/iuricode/padroes-de-commits)
, de Iuri Silva (@iuricode).

O conteúdo foi utilizado como referência para o estudo e adaptação das convenções de commits e boas práticas de versionamento abordadas neste projeto. O repositório original também utiliza como referência os conceitos de Conventional Commits.

### 📌 Objetivo

A padronização tem como principais objetivos:

Manter um histórico de commits organizado e consistente.
Facilitar a identificação das alterações realizadas.
Melhorar a comunicação entre os integrantes da equipe.
Facilitar a criação de changelogs e releases.
Padronizar a criação e utilização de branches.
### 🌿 Convenção de Branches

As branches devem seguir um padrão que permita identificar rapidamente o tipo e o objetivo da alteração.

#### / Estrutura

#### "tipo": "descrição"


##### Exemplos:

feature/autenticacao-usuario

fix/correcao-login

hotfix/erro-pagamento

refactor/servico-usuarios

docs/atualiza-readme

test/teste-autenticacao

chore/atualiza-dependencias


#### Boas práticas

Utilize nomes curtos e descritivos.
Prefira letras minúsculas.
Utilize - para separar palavras.
Evite caracteres especiais e espaços.
A branch deve representar claramente o objetivo da alteração.

### 📝 Convenção de Commits

Os commits devem seguir uma estrutura padronizada para facilitar a leitura do histórico.

#### / Estrutura
#### "tipo": "descrição"

##### Exemplos:

feat: adiciona autenticação de usuários

fix: corrige validação do formulário

docs: atualiza documentação da API

test: adiciona testes para autenticação

refactor: simplifica serviço de usuários

chore: atualiza dependências

style: ajusta formatação do código

perf: otimiza consulta de usuários

ci: adiciona pipeline de testes


#### 📏 Regras para mensagens de Commit

As mensagens devem:

Ser claras e objetivas.
Utilizar o verbo no presente.
Começar com o tipo da alteração.
Evitar mensagens genéricas como update, fix, changes ou teste.
Descrever o que foi alterado, e não necessariamente como foi implementado.
#### ❌ Evite
update
fix
mudanças
alterações
teste
coisas novas

#### ✅ Prefira
feat: adiciona recuperação de senha
fix: corrige erro na validação do e-mail
docs: adiciona instruções de instalação

#### 🔄 Fluxo de Trabalho

Um fluxo básico pode seguir estas etapas:

1. Atualizar a branch principal
git checkout main
git pull

2. Criar uma nova branch
git checkout -b feature/nova-funcionalidade

3. Realizar as alterações

Após implementar a alteração, verifique os arquivos modificados:

git status

4. Criar o commit
git add .
git commit -m "feat: adiciona nova funcionalidade"

5. Enviar a branch
git push -u origin feature/nova-funcionalidade

6. Criar o Pull Request

Após o push, deve ser criado um Pull Request para revisão e posterior merge na branch principal.

#### 📚 Exemplo Completo

Para implementar uma nova funcionalidade de autenticação:

Branch
feature/autenticacao-usuario

Commits
feat: adiciona estrutura de autenticação
feat: implementa login de usuários
test: adiciona testes para autenticação
docs: documenta fluxo de autenticação

Pull Request
feature/autenticacao-usuario
        ↓
      main

### 🎯 Resumo

A regra principal é:

Branches identificam o objetivo do trabalho; commits identificam as alterações realizadas durante esse trabalho.

Exemplo:

Branch:
feature/autenticacao-usuario

Commits:
feat: adiciona estrutura de autenticação
feat: implementa login de usuários
test: adiciona testes de autenticação
docs: documenta autenticação


Seguindo essas convenções, o histórico do projeto se torna mais previsível, organizado e fácil de entender.