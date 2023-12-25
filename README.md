# *Instalação*

## *Requisitos*

* [Python 3.8.6](https://www.python.org/downloads/release/python-386/)

```console
sudo apt install python
```
* Libs: SpeechRecognition, pyttsx3 e [PyAudio](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio)



## *Guia de instalação*

* O funcionamento da Íris se baseia no uso da linguagem de programação Python, sendo necessário o uso da versão 3.8.6 da mesma para que as funções da assistente virtual sejam realizadas da melhor forma possível e evitando transtornos à seus usuários. 
* Para a intalação do Python, é necessário o acesso ao site oficial python.org na pasta downloads para a obtenção dos instaladores necessários (neste caso o da versão 3.8.6) para adquirir a linguagem nas máquinas Windows. 
* Com o instalador em mãos, execute-o como administrador e abra-o marcando a opção "Add Python to PATH", para que assim tenha o comando python disponível. Após isso, apenas siga o processo padrão de instalação de programas no Windows. 
* Com o Python já instalado, é necessário também a obtenção de bibliotecas específicas, a SpeechRecognition, a pyttsx3 e a PyAudio. No caso das bibliotecas SpeechRecognition e pyttsx3, sua instalação se baseia no uso do `pip install` ao início do terminal. Assim, basta utilizar-se do `pip install SpeechRecognition` e do `pip install pyttsx3` (que podem ser encontrados e copiados do pypi.org,  site oficial de bibliotecas Python) em sua IDE para inicializá-las. 
* Já a outra biblioteca necessária na nossa assistente virtual, a PyAudio, não funciona apenas com a inicialização pelo pip install em versões acima da 3.6 do Python, o que nos obriga a realizar uma instalação manual da mesma. Para esta, é necessário o acesso no [link](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio) e o download do arquivo `PyAudio-0.2.11-cp39-cp39-win_amd64`. 
* Posteriormente, basta dar um pip install dentro do diretório desejado para conseguir efetuar a instalação de mais esta biblioteca. Com isso pronto, basta se aventurar dentro dos códigos a fim de prover mais e mais funções para nossa assistente virtual Íris e, assim, facilitar as ações cotidianas.
