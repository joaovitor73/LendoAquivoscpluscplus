# Lendo e escrevendo em arquivos com c++
### Passo 1 - Precisamos incluir a biblioteca fstream
    #include <fstream>   
### Passo 2 - Escolher o tipo do objeto ofstream(apenas escrita), ifstream(apenas leitura) ou fstream(leitura e escrita)
### Passo 3 - criar o objeto
    fstream arquivo;
### Passo 4 - Abrir um arquivo com o objeto arquivo
    arquivo.open("nome.extensão");
### Passo 5 - Escrevendo no arquivo
    arquivo << "Oi";
### Passo 6 - Lendo arquivo
    string linha; 
    if((arquivo.is_open(){//verifica se o arquivo está aberto
        while(getline(arquivo, linha){
            cout << "\n" << linha; //mostrando linha por linha do arquivo
        }
    }
### Passo 6 - Fechando o arquivo
    arquivo.close();
    
### Tipos de parâmetros do open
     1 - arquivo.open("nome.extensão", ios::app); //impede a sobrescrição de linhas
     2 - arquivo.open("nome.extensão", ios::out); //indicando que o modo da vez é de escrita
     3 - arquivo.open("nome.extensão", ios::in); //indicando que o modo da vez é de leitura
      
