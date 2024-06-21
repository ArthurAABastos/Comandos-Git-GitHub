# DIO | Resumos Git & GitHub

Repositório para armazenar resumos sobre o Git e GitHub do curso de Vrsionamento de Código do Git e GitHub do [BootCamp Santander](https://web.dio.me/track/santander-2024-backend-com-java).


## 📄 Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/pt)

## 💻 Resumos da Aula

| Aulas | Links |
|------|----------|
| Criando e clonando repositórios | [Link]()|
| Salvando Alterações no Repositório Local | [Link](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/599dd3dd-d189-474f-a55c-22f37b4472da?back=/track/santander-2024-backend-com-java)|
|Desfazendo Alterações no Repositório Local| [Link]()|
| enviando e Baixando Alterações com o Repositório Remoto | [Link]()|
| Trabalhando com Branches - Criando, Mesclando, | |
 Deletando e Tratando Conflitos  | [Link]()|
  | Trabalhando com Branches - Comandos Úteis do Dia a Dia | [Link]()|

## ⌨️ Comandos
  ```
git init <nome do repositório>
//cria um repositório local

git clone <link do Repositório>

git remote -v

git remote add origin <link do Repositório>

git status

git add <nome do arquivo>

git add . 
//Para adicionar todos os arquivos e epastas de uma única vez para a área de preparação.

git commit -m"identificação do commit"

git log 

git reflog 
// Exibe um log mais detalhado dos commit's

echo nome_pasta/ > .gitignore 
//comando para adicionar uma pasta a ser ingnorada no commit

echo > .gitignore 
//Para remover a pasta a ser ignorada no commit

########## Desfazendo alterações no respositório local ##########

rm -rf <diretorio>
//Comando para remover todo um diretório.

git restore 
//Recupera todas as mudanças efetuadas na árvore de trabalho.

git commit --amend -m"novo nome para o commit"
// Comando para mudar a mensagem de identificação do último commit

git reset <diretorio/nome_arquivo>
// Remove um arquivo especifico da area de trabalho 

git reset --soft <hash do commit que quer restaurar>

--> Efeito: Redefine apenas o ponteiro da branch atual (HEAD) para o commit especificado.

--> Área de stage: As mudanças no commit permanecem na área de stage.
Trabalho atual: As alterações ficam inalteradas no diretório de trabalho.

--> Uso: Útil quando você quer desfazer um commit, mas manter as alterações prontas para serem novamente commitadas.


git reset --mixed <hash do commit que quer restaurar>
// para remover um arquivo da área de preparação.

--> Efeito: Redefine o ponteiro da branch atual (HEAD) e a área de stage para o commit especificado.

--> Área de stage: As mudanças no commit são removidas da área de stage.
Trabalho atual: As alterações ficam inalteradas no diretório de trabalho.

--> Uso: Útil quando você quer desfazer um commit e preparar novamente as alterações para um novo commit.

git reset --hard <hash do commit que quer restaurar>

--> Efeito: Redefine o ponteiro da branch atual (HEAD), a área de stage e o diretório de trabalho para o commit especificado.

--> Área de stage: As mudanças no commit são removidas da área de stage.
Trabalho atual: As alterações no diretório de trabalho são perdidas e tudo é redefinido para o estado do commit especificado.

--> Uso: Útil quando você quer desfazer completamente um commit e todas as alterações associadas, retornando ao estado exato do commit especificado. Atenção: as mudanças serão perdidas permanentemente.

Resumo:

--soft: Mantém as alterações na área de stage.
--mixed: Mantém as alterações no diretório de trabalho, mas limpa a área de stage.
--hard: Perde todas as alterações e retorna ao estado do commit especificado.

#########################################################################

############### ENVIANDO E BAIXANDO NO REPOSITÓRIO LOCAL ################

git remote add origin <url-do-repositorio>
// Comando para conectar ao repositório local ao repositório remoto.

git push -u origin main
// Envia suas alterações para o repositório remoto

git pull
// Puxa as alteraçãos do repositório remoto para o repositório local.

git checkout -b <nome-nova-branch>
// Comando para cirar um branch de teste.

git checkout main
// Comando para retornar a branch main e desfazer as alterações.

git branch
// Lista todas as branch do respositório

git branch -v
// Lista o último commit de cada branch

git merge <nome-da-branch>
// Mescla as alterações da branch teste na branch main

git branch -d <nome-branch-a-exluir>
// Comando para excluir uma branch

  ```

  ## 🔎 Referências 
 - [CHACON, Scott. Pro-Git.  1ª edição. 11-05-2014 ](https://git-scm.com/book/pt-br/v2)
  - [AQUILES, Alexandre. Controlando versões com Git e GitHub.  1ª edição. 01-08-2014 ](https://www.casadocodigo.com.br/pages/sumario-git-github)
