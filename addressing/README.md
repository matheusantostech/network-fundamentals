# Network Addressing and Troubleshooting Basics

Este documento descreve os conceitos fundamentais de endereçamento de rede
utilizados em ambientes corporativos de suporte de TI.

O objetivo é demonstrar entendimento prático sobre como dispositivos se
comunicam dentro de uma rede local (LAN) e acessam a Internet (WAN).

---

## IP Address

Um endereço IP identifica unicamente um dispositivo dentro de uma rede.
Cada computador, servidor ou dispositivo conectado precisa de um IP exclusivo
para se comunicar corretamente.

Exemplo:
- Notebook: 192.168.1.10
- Servidor: 192.168.1.20

Se dois dispositivos utilizarem o mesmo IP, ocorre um conflito de IP,
causando instabilidade na rede.

---

## Subnet Mask

A máscara de sub-rede define quais dispositivos pertencem à mesma rede local.
Dispositivos considerados "vizinhos" podem se comunicar diretamente sem a
necessidade de acesso à Internet.

Exemplo comum:
- IP: 192.168.1.10
- Máscara: 255.255.255.0

Nesse caso, todos os endereços iniciados por 192.168.1 pertencem à mesma rede.

---

## Default Gateway

O gateway é o ponto de saída da rede local para outras redes, como a Internet.
Quando um dispositivo precisa se comunicar com um endereço que não pertence
à sua rede local, o tráfego é encaminhado para o gateway.

Exemplo:
- Gateway: 192.168.1.1

Se o gateway estiver incorreto ou inacessível, a rede local pode funcionar,
mas o acesso à Internet não.

---

## DNS (Domain Name System)

O DNS é responsável por traduzir nomes de domínio em endereços IP.
Computadores não acessam sites por nome, apenas por IP.

Exemplo:
- google.com → endereço IP correspondente

Problemas de DNS podem causar falha no acesso a sites, mesmo quando a conexão
com a Internet está ativa.

---

## Basic Troubleshooting Logic

Em um cenário de suporte técnico, a verificação de problemas de rede deve seguir
uma ordem lógica:

1. Verificar se o dispositivo possui um endereço IP válido
2. Verificar se o gateway está configurado corretamente
3. Verificar se o DNS está funcionando
4. Verificar possível conflito de IP

Essa abordagem evita diagnósticos incorretos e acelera a resolução de problemas.
