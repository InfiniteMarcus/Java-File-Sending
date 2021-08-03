# Java-File-Sending

Este repositório possui dois tipos de aplicações cliente-servidor de envio/recebimento de arquivos em Java, uma com implementação utilizando o protocolo **TCP** e uma com **UDP**.

## Propósito

Estas aplicações foram desenvolvidas para estudar e comparar as diferentes implementações de serviços da camada de transporte de redes na linguagem Java. 

É conhecido que o protocolo TCP possui diversas vantagens sobre o UDP, principalmente em termos de retransmissão de dados e controle de fluxo. No entanto, também é comumente notável que a maior robustez deste primeiro protocolo tende a gerar maiores tempos de execução que o segundo.

Este repositório, então, representa uma pequena prova de conceito desta diferenciação entre ambos.

## Execução

Para executar os códigos, basta entrar no diretório `src`, escolher entre `tcp` ou `udp` e executar separadamente os códigos cliente e servidor.

Para o cliente, na pasta `cliente`:

```sh
  javac Cliente.java
  java Cliente
```

Para o servidor, na pasta `servidor`:

```sh
  javac Servidor.java
  java Servidor
```

## Comparação

Para comparar as diferentes implementações, foram coletados os dados de tempo de execução entre elas, tanto ao enviar arquivos quanto receber. Estes valores, em milisegundos, foram agrupados em gráficos de dispersão. As médias e desvios padrão também foram calculados.

Todos os dados estão na pasta `comp`, na planilha `data.xls`.

## Imagens

<p align="center"> <strong> Gráficos de comparação de envio de arquivos: </strong> </p>

![Comparação de envio TCP vs UDP](https://github.com/Infinitemarcus/Java-File-Sending/blob/main/img/send.png)

<p align="center"> <strong> Gráficos de comparação de recebimento de arquivos: </strong> </p>

![Comparação de recebimento TCP vs UDP](https://github.com/Infinitemarcus/Java-File-Sending/blob/main/img/receive.png)

## Autor

* Marcus Vinícius N. Garcia ([Infinitemarcus](https://github.com/Infinitemarcus))
