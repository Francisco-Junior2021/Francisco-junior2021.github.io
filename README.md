## Welcome to GitHub Pages
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <link rel="stylesheet" type="text/css" href="css/stylesheet.css" media="screen" />
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Listas de Comandos do Git</title>
    <link rel="shortcut icon" type="image/png" href="img/logo.png" />
</head>

<body>
    <header class="background-color-text">
        <div class="logo">
            <a href="https://github.com/" target="_blank">
                <img src="img/logo.png" anima_quando_visivel="cresce">
            </a>
        </div>
        <h1> Comandos git</h1>
        <div class="logo">
            <a href="https://www.ifpb.edu.br/cajazeiras" target="_blank">
                <img src="img/logoIf.png" anima_quando_visivel="cresce">
            </a>
        </div>
    </header>

    <section class="description" id="content">
        <h3>Comandos do Git</h3>
        <br>
        <ul id="lista">
            <li><b>Git Init</b> - Inicializa um repositório git em um diretório ou reinicializa um existente.</li>
            <li><b>Git Status</b> - Apresenta o status atual do repositório.</li>
            <li><b>Git log</b> - Mostra todo o histórico dos commits.</li>
            <li><b>Git branch [nome_da_branch]</b> - Cria uma nova branch.</li>
            <li><b>Git checkout</b> - Navegar pelas branch's criadas.</li>
            <li><b>Git clone</b> - Cria um clone de um repositório do github.</li>
            <li><b>Git add [nome_do_arquivo]</b> - Armazena o arquivo ou arquivos no
                no seu <em>Stage</em> para que sejam <em>comitados</em> posteriormente.</li>
            <li><b>Git config --global user.name "[seu-nome]"</b> - Setar um usuário.</li>
            <li><b>Git config --global user.email [seu-email]</b>- Setar um email.</li>
            <li><b>Git ignore </b> - Ignorando Arquivos.</li>
            <li><b>Git merge </b>-Permite que você pegue as linhas de desenvolvimento independentes criadas pelo git
                branch e as integre em um único branch.</li>
            <li><b>Git revert [hash_do_commit ou nome_do_commit]</b> - Permite reverter commits existentes.</li>
        </ul>
        <br>
        <h3>Comandos Linux</h3>
        <ul id="lista">
            <li><b>mkdir [nome]</b> - Cria um diretório/pasta para trabalhar em um projeto.</li>
            <li><b>rm [nome do arquivo]</b> - Remove um arquivo, lista de arquivos ou pasta.</li>
            <li><b>ls</b> - Lista todos os arquivos do diretório.</li>
            <li><b>cd</b> - Acessa uma determinada pasta (diretório).</li>
        </ul>
    </section>
    <section>
        <div class="background-color-text">
            <h2 class="title-h1">Descrição dos Comandos</h2>
        </div>
        <div class="description">
            <h3>Git Init</h3>
            <p>Este comando cria um repositório Git vazio - basicamente um diretório .git com subdiretórios para
                objects, refs/heads, refs/tagsarquivos, e modelo. Um branch inicial sem nenhum commit será criado.
                Ao executar git init em um repositório existente não sobrescreverá coisas que já estão lá.
                O principal motivo para executar novamente o git init é selecionar os modelos recém-adicionados.
            </p>
        </div>
        <div class="description">
            <h3>Git Status</h3>
            <p>Exibe caminhos que têm diferenças entre o arquivo de índice e o commit HEAD atual, caminhos que têm
                diferenças entre a árvore de trabalho e o arquivo de índice e caminhos na árvore de trabalho que não
                são rastreados pelo Git (e não são ignorados pelo gitignore [5] ) O primeiro é o que você iria
                cometer executando git commit; o segundo e o terceiro são o que você pode confirmar executando git
                add
                antes de executar git commit.
            </p>
        </div>
        <div class="description">
            <h3>Git Log</h3>
            <p>Liste os commits que são alcançáveis ​​seguindo os parentlinks do (s) commit (s) fornecido (s),
                mas exclua os commits que são alcançáveis ​​daquele (s) fornecido (s) com um ^ na frente deles.
                A saída é fornecida em ordem cronológica reversa por padrão.
            </p>
        </div>
        <div class="description">
            <h3>Git branch</h3>
            <p>
                O comando git branch [nome_da_branch] permite que o usuário crie uma nova ramificação para poder
                editar
                o código sem interferir na branch principal. Uma ramificação no git é um ponteiro para as alterações
                feitas
                nos arquivos do projeto. Essa ramificação é muito utilizada em situações que o usuário deseja
                adicionar um novo recurso
                ou corrigir um erro, gerando uma nova ramificação garantindo que o código da ramificação criada não
                seja mesclado nos arquivos
                do projeto principal.
            </p>
        </div>
        <div class="description">
            <h3>Git checkout</h3>
            <p>
                O comando git checkout permite que o usuário altere entre as branch's criadas, esse comando é
                utilizado com o mesmo propósito do
                git branch, pois com ele o usuário muda para a branch criada para fazer novas atualizações, o
                comando é utulizado da seguinte forma:
                "git checkout [nome_da_branch]". O comando git branch -b [nome_da_branch] cria uma branch e jé
                altera para a branch criada, fazendo
                uma parte do trabalho do git checkout.
        </div>
        <div class="description">
            <h3>Git clone</h3>
            <p>O comando git clone é usado para criar uma cópia de um repositório específico dentro de um
                repositório.
            </p>
        </div>
        <div class="description">
            <h3>Git add [nome_do_arquivo]</h3>
            <p>O comando git add [nome-do-arquivo] é utilizado para adicionar um arquivo ou realizar alterações em
                um arquivo existente no
                diretório, ao ser adicionado, este arquivo ou alteração são armazenados no <em>stage</em> e
                posteriormente podem ser comitados para
                o repositório git. <br> Ex: <b> git add</b> <em>index.html</em>
            </p>
        </div>
        <div class="description">
            <h3>git config --global user.name "[seu-nome]" e git config --global user.email [seu-email] </h3>
            <p>Estes comandos git são tutlizados para definir seu usuário e email no git, o nome será usado para
                associar os
                commits aos usuários que realizaram alguma alteração no repositório. <br>
                Ex: <b>git config --global user.name </b> <em>"João padrão"</em> <br>
                Ex: <b>e git config --global user.email </b> <em>joaopadrao@mail.com</em>
            </p>
        </div>
        <div class="description">
            <h3>.gitignore</h3>
            <p>É extremamente normal ignorar arquivos no Git para não salvarmos arquivos de configuração dos nossos
                editores,<br>
                arquivos temporários do nosso sistema operacional, dependências de repositório, etc. <br>
                Para isso criamos um arquivo chamado .gitignore e adicionamos os nomes dos arquivos nele. <br>
            </p>
        </div>
        <div class="description">
            <h3>Git merge</h3>
            <p>
                O comando git merge permite que você pegue as linhas de desenvolvimento independentes criadas pelo
                git branch e as integre em um único branch. Observe abaixo um exemplo.
            </p>
            <img src="img/merge.png">
        </div>
        <div class='description' anima_quando_visivel="aparece">
            <h3>git revert [hash_do_commit ou nome_do_commit]</h3>
            <p>
                Esse comando cria um novo commit ignorando os commit passados em seu parametro.
                Bastante facil de se utilizar além do fato de por ser um commit, tem a possibilidade de ser
                revertido pelo proprio git revert.
            </p>
        </div>
        <div class="description">
            <h3>$ nano</h3>
            <p>Esse comando cria um arquivo diretamente do terminal sem precisar usar alguma IDE, por exemplo:" $
                nano index.html",
                cria um arquivo em HTML.
                OBS: É indicado o uso do nano para a criação de arquivos pequenos. Arquivos muito grandes é
                aconselhável o uso de IDE.
            </p>
        </div>
        <div class="description" anima_quando_visivel="aparece">
            <h3>$ rm</h3>
            <p>Este comando remove uma pasta ou arquivo, por exemplo, para apagar um arquivo text.txt
            <p class="code">
                $ rm test.txt
            </p>
            o Comando pode ser seguido por -r, -f, -i ou -v, respectivamente:
            <p class="comment">
                // Apaga pastas e subpastas
            </p>
            <p class="code">
                $ rm -r pasta_de_atividades
            </p>
            <p class="comment">
                // Ignora o pedido de confirmação para apagar um arquivo ou pasta
            </p>
            <p class="code">
                $ rm -f pasta_de_atividades
            </p>
            <p class="comment">
                // Pede confirmação para apagar arquivo ou pasta
            </p>
            <p class="code">
                $ rm -i pasta_de_atividades
            </p>
            <p class="comment">
                // Lista arquivos deletados
            </p>
            <p class="code">
                $ rm -v pasta_de_atividades
            </p>
            </p>
        </div>     

        <div class="container">
            <div class="contact-box">
                <div class="left"></div>
                <div class="right">
                    <h2>Contato</h2>
                    <input type="text" class="field" placeholder="Seu Nome">
                    <input type="text" class="field" placeholder="Seu E-mail">
                    <input type="text" class="field" placeholder="Telefone">
                    <textarea placeholder="Mensagem" class="field"></textarea>
                    <button class="btn">Enviar</button>
                </div>
            </div>
<<<<<<< HEAD
        </header>
        <section id="content">
            <h3>Alguns comandos do Git</h3>
        
            <ul id="lista">
                <li><b>Git Init</b> - Inicializa um repositório git em um diretório.</li>
                <li><b>Git Status</b> - Apresenta o status atual do repositório.</li>
                <li><b>mkdir [nome]</b> - Cria um diretório/pasta para trabalhar em um projeto.</li>
                <li><b>Git log</b> - Mostra todo o histórico dos commits</li>
            </ul>
        </section>
        <footer>
            <p>Site construído pela turma do 2º período (2020.2) de ADS - IFPB Campus Cajazeiras</p>
        </footer>
    </div>
</body>

</html>

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
