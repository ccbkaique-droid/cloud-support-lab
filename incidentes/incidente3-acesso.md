# Incidente 3 — Falha de acesso ao sistema

## Problema
Usuário não conseguia acessar sistema.

## Diagnóstico
Verificada  a conectividade com o servidor utilizando o comando:
```bash
ping localhost
O comando retornou resposta normalmente, com 0% de perda de pacotes, indicando que a conectividade com o servidor estava funcionando corretamente.
## Evidência
21 packets transmitted, 21 received, 0% packet loss
##Interpretação
-Foi descartado o problema de conectividade de rede e iniciou-se a investigação do serviço e da porta.

##  Diagnóstico
Verifiquei os processos em execução com o comando:
```bash
ps aux | grep python
A saída não apresentou nenhum processo relacionado ao serviço http.server, indicando que o serviço não estava rodando.
## Solução
Iniciar o serviço usando:
python3 -m http.server 8000
## Validação
Foi testado o serviço e validado, usando o comando:
curl localhost 8000
