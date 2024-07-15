# Gerador de Carteira BTC

Este projeto é um gerador de carteiras Bitcoin para a rede de teste (testnet) utilizando as bibliotecas `bip32`, `bip39` e `bitcoinjs-lib`. Ele cria um endereço Bitcoin e uma chave privada a partir de uma frase mnemônica (seed), que pode ser usada para gerenciar suas transações na rede testnet.

## Pré-requisitos

Antes de começar, você precisará ter o Node.js instalado em sua máquina. Você pode baixar o Node.js [aqui](https://nodejs.org/).

## Instalação
1. Instale as dependências:
    ```bash
    npm install bip39 bip32@2.0.6 bitcoinjs-lib
    ```

## Uso

Para gerar uma nova carteira Bitcoin na rede testnet, execute o seguinte comando:

```bash
node create-wallet.js
```

O programa também pode ser executado na mainnet, para isso basta alterar a constante network para (bitcoin.networks.testnet)

## Ambiente de Teste com Electrum

Para testar a carteira gerada, você pode utilizar o Electrum no modo testnet. Siga os passos abaixo para configurar o Electrum:

1 - Baixe e instale o Electrum <a href="https://electrum.org/#download">aqui</a>.

2 - Abra o Electrum e escolha a opção para rodar no modo testnet.

3 - Crie uma nova carteira e selecione a opção de usar uma frase mnemônica existente.

4 - Insira a frase mnemônica (seed) gerada pelo script.

Agora você deve conseguir ver o endereço e a chave privada gerados pelo script no Electrum e pode usá-los para realizar transações na testnet.
