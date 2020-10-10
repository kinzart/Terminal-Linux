# Terminal-Linux
Tutorial pra min mesmo! Linguagem Linux




<h1>COMANDOS</h1> 

auto prenchimento (=melhor de todos)

    tecla = [tab]



admin

    sudo


update

    sudo apt-get update
    

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


para mover um diretório acima
        
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
    
mover o aruivo

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
    

procurar por alguma palavra dentro de um arquivo

    grep nome-desejavel nome-arquivo.ext













Reinstalaçao de desktop
    
    sudo apt-get remove --purge ubuntu-desktop && sudo apt-get install ubuntu-desktop
