# Terminal-Linux
Tutorial pra min mesmo! Linguagem Linux




<h1>COMANDOS</h1> 

auto prenchimento (=melhor de todos)

    tecla = [tab]



admin

    sudo



update

    sudo apt-get update
    


trocar senha root:
    
    sudo passwd root
    


interromper processo

    ctrl + c
    

parar processo

    ctrl + z


mover para o inicio da linha

    ctrl + a
    
    
mover para o fim da linha

    ctrl + e
    
    


<h2>caminhando em diretorios:</h2>



caminho para pasta atual

    pwd


para mover um diretório acima (backstage)
        
      cd.. 

para ir diretamente para a pasta home

      cd /
        
 para ir diretamente para a pasta inicial
  
      cd ~
 
 para mover para os diretórios anteriores.
 
      cd-





<h2>Listando</h2>



listar diretorio

    ls
    
listar diretorios e subdiretorios

    ls -R
    
listar arquivos ocultos

    ls -a
  
listar arquivos e diretorios com detalhes

    ls -al


listar arquivos dentro do diretorio atual com detalhes


    ll
    

<h2>Lendo conteudos</h2>

lendo o conteudo interno do arquivo

    cat arquivo.ext
    

colocando uma linha de codigo dentro do arquivo via terminal


    echo "texto que vai colocar" >> arquivo.js
    
    
apagando linha de dentro do arquivo (3ª linha)

    sed -i '3d' arquivo.ext 
    
    
apagando linhas de dentro do arquivo (3ª e 4ª linha)

    sed -i '3,4d' arquivo.ext
    



<h2>Criar, mover, renomear e remover</h2>


criar pasta

    mkdir nome-pasta
    
criar pasta dentro de outra (criar 2 pastas)

    mkdir nome-pasta1/nome-pasta2
    
criar arquivo (nao deixe de colocar a extensao do aquivo)

    touch nome-arquivo.ext
    
criar um arquivo dentro de uma pasta existente

    touch diretorioX/nome-arquivo.ext 


copiar arquivo (dentro do diretorio que esta o arquivo)

    cp nome-arquivo
 
 
copiar arquivo e enviar para outra pasta

    cp nome-arquivo.ext /diretorioX/diretorioY/aqui


copiar todos arquivos dentro de um diretório para outro diretório
    
    cp * /home/dellamor/public_html/wp-content/uploads


mover o arquivo

    mv nome-arquivo.ext /diretorioX/diretorioY/aqui
    
    
renomear arquivo

    mv nome-aruiqvo.ext novo-nome.ext
    
    
remover um diretorio (remove tudo dentro)

    rm nome-diretorio




<h2>Buscar diretorios e arquivos</h2>


localizar arquivo (cai listar tudo que tiver essa palavra)

    locate -i nome-arquivo

localizar dois arquivos de uma vez

    locate nomearquivo1 * nomearquivo2
    
    locate -i nome * arquivo
    

procurar o arquivo em um diretorio especifico

    find /home/ -name nome-arquivo.ext

    
procurar aruqivos em um diretorio atual

    find . -name nome-arquivo.ext
    

procurar por alguma palavra ou texto dentro de um arquivo

    grep nome-desejavel nome-arquivo.ext

procurar uma palavra ou texto dentro de varios arquivos no diretorio atual

    grep nome-desejavel . *
    
procurar texto ou palavra no diretorio atual e nos subdiretorios 

    grep -R nome-desejavel *

gravar saidas da pesquisa em um arquivo

    grep nome-desejavel arquivo.txt > arquivodesaida.txt

filtrar saidas da pesquisa e seus caminhos:

    grep -R 'nome-desejavel' ./ | cut -d: -f1 | uniq





<h2>Compactando e desconpactando (zip)</h2>


Compactando um arquivo e nomeando a pasta compactada
    
    zip arquivo nomedacompactacao.zip
    


Compactando diretorios e subdiretorios:

    zip -r compactado.zip diretorio


Compactando mais de um diretorio:

    zip -r compactado.zip diretorio1 diretorio2 diretorio3


Compactando diretorios e subdiretorios e ignorando algum diretorio indesejavel:

    zip -r compactado.zip diretorio --exclude "/public_html/wp-content/uploads"
  
  
  
descompactando um arquivo no local

    unzip pastacompactada.zip
    
    
descompactando um arquivo em uma nova pasta

    unzip pastacompactada.zip -d diretorio
    

Reinstalaçao do nodeJS (para a proxima versao)

        sudo npm cache clean -f

        sudo npm install -g n

        sudo n stable 
        
  
  obs: no lugar de stable, colocar a versao (12.6.1)




Reinstalaçao de desktop
    
    sudo apt-get remove --purge ubuntu-desktop && sudo apt-get install ubuntu-desktop
    
    
    
    
    
    
    
    
    
    
 <h2>LOGANDO EM SITE DE UM VHM NO HOSTGATOR</h2>


        ssh -p 22022 user@domain.com
   
   
   Digite a senha do usuario cpanel quando pedir o password

  
  
    
    
    
