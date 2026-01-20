# DHCP Fundamentals

Este documento apresenta o entendimento dos conceitos básicos de DHCP
(Dynamic Host Configuration Protocol) aplicados a ambientes de suporte de TI.

## O que é DHCP
DHCP é um serviço de rede responsável por atribuir automaticamente
endereços IP e configurações de rede aos dispositivos que se conectam
a uma rede.

As informações entregues normalmente incluem:
- Endereço IP
- Máscara de rede
- Gateway padrão
- Servidores DNS

## Por que o DHCP é importante
Sem DHCP, os dispositivos precisam ser configurados manualmente,
o que aumenta o risco de erros, conflitos de IP e dificulta a escalabilidade
da rede.

O uso de DHCP permite:
- Redução de erros humanos
- Evitar conflitos de IP
- Facilidade de expansão da rede
- Manutenção simplificada

## Funcionamento básico
Quando um dispositivo entra na rede, ele solicita um endereço IP.
O servidor DHCP responde oferecendo um IP disponível dentro de um intervalo
pré-configurado (pool). O dispositivo aceita esse IP por um período
determinado (lease).

## Problemas comuns relacionados ao DHCP
- Dispositivo recebe IP 169.254.x.x indicando falha na atribuição de IP
- Pool de endereços esgotado
- Conflito de IP causado por endereços configurados manualmente
- Gateway ou DNS incorretos entregues pelo DHCP

## Visão aplicada ao suporte de TI
Em ambientes corporativos, o DHCP é essencial para manter a rede estável,
organizada e escalável. Identificar falhas de DHCP é uma das tarefas
mais comuns em suporte técnico de redes.
