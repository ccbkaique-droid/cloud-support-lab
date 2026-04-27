# Incidente 1 — Falha de acesso por permissão

##  Problema
Usuário não conseguia acessar o arquivo sistema.txt.

##  Diagnóstico
Verifiquei as permissões do arquivo usando ls -l.

##  Investigação
O arquivo estava sem permissões (----------), impedindo qualquer acesso.

##  Solução
Apliquei chmod 644 sistema.txt para permitir leitura.

##  Validação
Teste realizado com outro usuário confirmou acesso ao arquivo.

##  Comandos utilizados

```bash
ls
ls -l sistema.txt
cat sistema.txt
chmod 000 sistema.txt
chmod 644 sistema.txt

