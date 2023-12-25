# *Instalação*

## *Requisitos*

* [Python 3.8.6](https://www.python.org/downloads/release/python-386/)
* Libs: SpeechRecognition, pyttsx3 e [PyAudio](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio)



## *Guia de instalação*

* O funcionamento da Íris se baseia no uso da linguagem de programação Python, sendo necessário o uso da versão 3.8.6 da mesma para que as funções da assistente virtual sejam realizadas da melhor forma possível e evitando transtornos à seus usuários. 
* Para a intalação do Python, é necessário o acesso ao site oficial python.org na pasta downloads para a obtenção dos instaladores necessários (neste caso o da versão 3.8.6) para adquirir a linguagem nas máquinas Windows. 
* Com o instalador em mãos, execute-o como administrador e abra-o marcando a opção "Add Python to PATH", para que assim tenha o comando python disponível. Após isso, apenas siga o processo padrão de instalação de programas no Windows. 
* Com o Python já instalado, é necessário também a obtenção de bibliotecas específicas, a SpeechRecognition, a pyttsx3 e a PyAudio. No caso das bibliotecas SpeechRecognition e pyttsx3, sua instalação se baseia no uso do `pip install` ao início do terminal. Assim, basta utilizar-se do `pip install SpeechRecognition` e do `pip install pyttsx3` (que podem ser encontrados e copiados do pypi.org,  site oficial de bibliotecas Python) em sua IDE para inicializá-las. 
* Já a outra biblioteca necessária na nossa assistente virtual, a PyAudio, não funciona apenas com a inicialização pelo pip install em versões acima da 3.6 do Python, o que nos obriga a realizar uma instalação manual da mesma. Para esta, é necessário o acesso no [link](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio) e o download do arquivo `PyAudio-0.2.11-cp39-cp39-win_amd64`. 
* Posteriormente, basta dar um pip install dentro do diretório desejado para conseguir efetuar a instalação de mais esta biblioteca. Com isso pronto, basta se aventurar dentro dos códigos a fim de prover mais e mais funções para nossa assistente virtual Íris e, assim, facilitar as ações cotidianas.

### *Instalação do Python no ubuntu*
```bash
sudo apt update
sudo apt upgrade
sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev libsqlite3-dev wget libbz2-dev
wget https://www.python.org/ftp/python/3.8.6/Python-3.8.6.tgz
tar -xf Python-3.8.6.tgz
cd Python-3.8.6
./configure --enable-optimizations
make -j8  # Use -j com o número de núcleos do seu processador
sudo make altinstall
```
### *Instalação das libs SpeechRecognition e pytssx3 no ubuntu*

```bash
pip install SpeechRecognition
pip install pyttsx3
```
### *Instalação de PyAudio no ubuntu*

```bash
pip install caminho/para/o/arquivo/nome_do_arquivo.whl
```    
* Substitua `nome_do_arquivo.whl` pelo nome específico do arquivo que você baixou do site do PyAudio no Unofficial Windows Binaries for Python Extension Packages. Certifique-se de que o arquivo .whl seja compatível com a versão do Python que você está usando. Se você estiver usando um ambiente virtual, ative-o antes de instalar as bibliotecas.

# Guia de uso

A assistente virtual Íris funciona a partir de 4 botões principais que visam auxiliar o usuário em diferentes aspectos no cotidiano. A começar, o usuário pode ficar por dentro de como funciona a Íris e como utilizá-la a partir do botão SOBRE A ÍRIS, que mostra informações sobre o projeto, guia de uso e também de instalação. Além disso, o usuário tem duas formas de utilizá-la, ou apertando o botão FALAR COMANDO, que abre seu dispositivo de saída de voz permitindo que fale apenas um comando através da captura de áudio e posteriormente encerra o sistema sendo necessário apertá-lo novamente para dar um outro comando, ou pelo botão MANTER ASSISTENTE ATIVA, em que a captação de áudio ocorre de forma ininterrupta até que o programa seja encerrado e os comandos só são executados no momento em que é dito o nome da assistente (Íris). Por fim, caso não seja mais necessário o uso da assistente, o cliente tem a opção de clicar no botão SAIR para finalizar os trabalhos da Íris.
Segue uma lista de comandos que podem ser executados por nossa assistente virtual:
1. Alteração do nome da assistente a partir de: 
  - nome_assistente = "..."
2. Definição do comando de parada: 
  - parada = "..."
3. Busca de notícias na internet a partir de palavras como 'pesquise','bard','qual', 'o que é'
  - Íris, quais são as notícias de hoje? R: As notícias são: Saiba quem é o suspeito de ser o maior devastador da Amazônia preso hoje; GLOBONEWS AO VIVO: assista ao 'Estúdio i'...
4. Conversão das horas de algarismos para a hora por extenso
  - Íris, me diga o horário 21h53 por extenso R: O horário é nove horas e cinquenta e três minutos
5. Verificação de palavrões (se o usuário utilizou-se de palavrões ao falar com a assistente)
  - Íris, te acho uma chata R: Por favor pare de usar palavras chulas, fale novamente com mais educação
6. Traduções de idiomas no estilo google tradutor
  - Íris, traduza: Oi, tudo bem em inglês? R: Hey how's it going?
7. Contar piadas
  - Íris, conte-me uma piada R: Por que a mulher do Hulk divorciou-se dele? Porque ela queria um homem mais maduro; Você conhece a piada do pônei? Pô nei eu...; ...
8. Busca de músicas no youtube e colocá-las para tocar
  - Íris, toque a música Burguesinha - Seu Jorge R: Tocando Burguesinha - Seu Jorge
9. Cantar músicas
  - Íris, cante uma música R: "No mundo da magia digital
                              Eu sou uma voz especial
                              Para fazer seu dia brilhar

                              Com carinho e emoção
                              Eu canto a sua canção
                              Com amor e devoção

                              Entre bits e bytes vou voar
                              Com você sempre a caminhar
                              Nossa conexão é singular, ..."
                    
                              Por favor me dê palmas!
10. Abrir o e-mail
  - Íris, abra o email R: Abrindo e-mail
11. Busca de significado de palavras na internet
  - Íris, procure por Amor R: Forte afeição por outra pessoa, nascida de laços de consanguinidade ou de relações sociais.
12. Falar o horário em que está sendo utilizada
  - Íris, diga-me as horas R: Agora são 22h06
13. Pedir ao usuário que repita o comando caso não tenha sido compreendido
  - R: Não foi possível reconhecer o áudio.
14. Conversas com o usuário
  - Íris, está tudo bem? R: Poderia estar melhor se tivesse passado em lógica...
15. Botão que fecha tudo
16. Botão que abre a nova janela
17. Entrada e Saída de áudio
18. Resposta se o microfone não está entregando áudio
19. Testagem do microfone~
20. Erro na busca de informações pedidas pelo usuário