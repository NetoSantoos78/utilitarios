# WebSocket Secury
* 1° PASSO: DESATIVAR TODAS AS PORTAS DO PAINEL <br>
*2° PASSO: COPIAR O SCRIPT ABAIXO E COLAR DENTRO DA VPS E DÁ ENTER E ESPERE TERMINAR DE INSTALAR<br>
cd /etc/SSHPlus/ && wget https://www.dropbox.com/s/muh8otpcjb9qa6d/WebSocket && wget https://www.dropbox.com/s/zv01bftfjj58wt8/pub.key && wget https://www.dropbox.com/s/pj5s9x23boj840q/priv.pem && chmod 777 WebSocket && cd $HOME<br>

3° PASSO: COPIAR O COMANDO ABAIXO E COLAR DENTRO DA VPS NOVAMENTE E DÁ ENTER<br>

mkdir /opt/sshplus<br>
echo > /opt/sshplus/sshplus<br>

4° PASSO: TROQUE (SUA_MENSAGEM_AQUI) POR ALGUM NOME SEU(OBRIGATÓRIO) COPIA E COLA DENTRO DA VPS E DA ENTER<br>

screen -dmS novoWS /etc/SSHPlus/WebSocket -proxy_port 0.0.0.0:80 -msg=BOTE_SUA_MENSAGEM_AQUI<br>

5° PASSO: IR NO MENU DO SCRIPT E VERIFICAR A OPÇÃO INFO VPS E OBSERVAR SE TEM A WEBSOCKET SECURITY NA 80<br>
