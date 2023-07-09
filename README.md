### Passo 1 - Precisamos incluir a biblioteca fstream
    #include <fstream>   
### Passo 2 - Escolher o tipo do objeto: ofstream(apenas escrita), ifstream(apenas leitura) ou fstream(leitura e escrita)
### Passo 3 - Nesse exemplo vou criar o objeto fstream
    fstream arquivo;
### Passo 4 - Para abrir um arquivo precisamos usar o objeto criado no passo anterior e usar o seu método open
    arquivo.open("nome.extensão");    
 ### Passo 5 - Fechando o arquivo
    arquivo.close();
### Leitura - Escrevendo no arquivo, precisamos indicar que vai ser uma ação de escrita
    arquivo.open("nome.extensão", ios::out)
    arquivo << "Oi";
### Escrita - Lendo o arquivo e mostrando na tela, também precisamos indicar que vai ser uma leitua
    arquivo.open("nome.extensão", ios::in)
    string linha; 
    if((arquivo.is_open(){//verifica se o arquivo está aberto
        while(getline(arquivo, linha){
            cout << "\n" << linha; //mostrando linha por linha do arquivo
        }
    }
    
### Tipos de parâmetros do open
     1 - arquivo.open("nome.extensão", ios::app); //impede a sobrescrição de linhas
     2 - arquivo.open("nome.extensão", ios::out); //indicando que o modo da vez é de escrita
     3 - arquivo.open("nome.extensão", ios::in); //indicando que o modo da vez é de leitura
      
