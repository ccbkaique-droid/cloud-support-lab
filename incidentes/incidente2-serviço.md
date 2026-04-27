# Incidente 2 — Serviço indisponível

## Problema
Sistema web não respondia.

## Diagnóstico
Servidor acessível, mas serviço não respondia.

## Investigação
Serviço não estava rodando.

## Solução
Reiniciado serviço com python3 -m http.server 8000.

## Validação
Sistema voltou a responder.
