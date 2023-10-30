# Comandos Git

* **Git status**: Visualizar o cenário no desenvolvimento atual
* **Git add < file name >**: Adiciona a alteração na stage área
* **Git commit -m "< mensagem referência >"**: Salvar a versão atual
* **Git reset --hard < hash >**: Retornar para o comit anterior e todas alterações feitas
* **Git reset --soft < hash >**: Retornar para a área de stage, assim pode-se fazer os ajustes desejados.
* **Git reset --staged < hash >**: Tirar da área de stage e retornar a àrea de alteração
* **Git restore < filename >**: Descartar as alterações
* **Git clone < https >**: Clona o repositório
* **Git config --local -e**: Para editar a configuração local
* **Git config --global -e**: Para editar a configuração global
* **Git log**: Histórico de commits
* **Git push**: Envia o commit local para o principal
* **Git pull**: Atualiza as alterações feita por outro usuário
* **Git checkout -b < nome branch >**: Cria um novo ramo 
* **Git merge**: Fusão entre a branch criada e outra branch
* **Git branch -d < nome da branch >**: Apaga uma branch.
* **Git branch**: Visualiza as branch's existentes
* **Git config --global init.defaultBranch main**: Definindo convenção para branch principal
* **Git checkout < nome da branch >**: Muda para a branch digitada
* **Git branch -a**: Mostra também os apontamentos remotos
* **Git log --oneline**: Visualização da árvore de commit's
* **Git reflog**: Lista de commit's existentes
* **Git stash**: Envia um arquivo para outra branch, mas só pode ser usado após adicionar o arquivo à stage área com "git add ..."
* **Git stash pop**: Coleta o arquivo da stage àrea para a branch atual. 
* **Git stash list**: Lista as stash's que estão prontas para serem mudadas de branch.
* **Git log --oneline -graph**: Mostra a plilha de comites até a criação das branch's  