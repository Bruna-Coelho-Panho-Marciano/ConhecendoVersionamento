# Conhecendo Versionamento Git

## O que é Git?
Git é um sistema de controle de versão distribuído usado para rastrear mudanças no código-fonte durante o desenvolvimento de software.
Ele permite que múltiplos desenvolvedores trabalhem no mesmo projeto simultaneamente sem interferir no trabalho uns dos outros.

## Como surgiu o Git?
O Git surgiu em 2005, criado por **Linus Torvalds** (criador do kernel Linux), como uma solução para o desenvolvimento do projeto Linux. A principal motivação foi a licença do sistema de controle de versão BitKeeper ser revogada para os desenvolvedores do Linux, tornando-o pago e criando a necessidade de um novo sistema, gratuito, rápido e distribuído.

## Quem Criou o Git?
O Git foi criado por **Linus Torvalds**, o  mesmo criador do Linux. Surgiu da necessidade de um sistema de controle de versão mais eficiente após problemas com o BitKeeper. 

## Os Comandos Principais do Git são:

### Configuração:
git config --global user.name "Seu Nome" <br>
git config --global user.email "seu@email.com"

### Inicialização:
git init &nbsp;&nbsp;&nbsp;&nbsp; # Cria novo repositório <br>
git clone [url] &nbsp;&nbsp;&nbsp;&nbsp;             # Baixa repositório existente

### Fluxo Básico:
git status &nbsp;&nbsp;&nbsp;&nbsp;                  # Verifica estado dos arquivos <br>
git add [arquivo] &nbsp;&nbsp;&nbsp;&nbsp;           # Prepara arquivos para commit <br>
git add .  &nbsp;&nbsp;&nbsp;&nbsp;                  # Prepara todos os arquivos <br>
git commit -m "mensagem" &nbsp;&nbsp;&nbsp;&nbsp;    # Salva as alterações <br>
git push origin main &nbsp;&nbsp;&nbsp;&nbsp;        # Envia para repositório remoto 

### Branches:
git branch   &nbsp;&nbsp;&nbsp;&nbsp;                # Lista branches <br>
git branch [nome] &nbsp;&nbsp;&nbsp;&nbsp;           # Cria nova branch <br>
git checkout [branch] &nbsp;&nbsp;&nbsp;&nbsp;       # Muda para branch <br>
git checkout -b [branch] &nbsp;&nbsp;&nbsp;&nbsp;    # Cria e muda para branch <br>
git merge [branch]  &nbsp;&nbsp;&nbsp;&nbsp;         # Une branches 

### Atualização:
git pull origin main &nbsp;&nbsp;&nbsp;&nbsp;        # Baixa e integra alterações <br>
git fetch origin &nbsp;&nbsp;&nbsp;&nbsp;            # Apenas baixa alterações 

### Comandos de Consulta:
git log  &nbsp;&nbsp;&nbsp;&nbsp;                   # Histórico de commits <br>
git log --oneline &nbsp;&nbsp;&nbsp;&nbsp;          # Histórico resumido <br>
git diff &nbsp;&nbsp;&nbsp;&nbsp;                   # Mostra diferenças

### Comandos Úteis do Dia a Dia:
git commit -am "msg" &nbsp;&nbsp;&nbsp;&nbsp;       # Add + commit em arquivos rastreados <br>
git push -u origin main &nbsp;&nbsp;&nbsp;&nbsp;    # Define upstream na primeira vez <br>
git pull --rebase  &nbsp;&nbsp;&nbsp;&nbsp;         # Atualiza com rebase

### Comandos de Emergência:
git restore [arquivo] &nbsp;&nbsp;&nbsp;&nbsp;      # Desfaz alterações não commitadas <br>
git reset --hard [hash] &nbsp;&nbsp;&nbsp;&nbsp;    # Volta para commit específico (CUIDADO!)

### Fluxo Diário Típico:
git status → git add . → git commit -m "msg" → git pull → git push <br>

### Configuração Básica:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"



