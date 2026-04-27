# Incidente 1 — Falha de permissão

## Problema
Usuário não conseguia acessar o arquivo.

## Diagnóstico
Verificou-se com ls -l.

## Investigação
Arquivo sem permissões.

## Solução
chmod 644 sistema.txt

## Validação
Usuário conseguiu acessar.
