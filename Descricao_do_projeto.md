## Projeto de medição de energia elétrica
#### Alunos: Vicente e Maurício
#### Univates 2018/2
#### Descrição da especificação e escolha do mini micro computador:
O projeto consiste na medição inloco e monitoramento a distância por servidor, possivelmente 
usando protocolo de comunicação MQTT.MQTT. Medição de grandezas como tensão e corrente, e possivelmente
comparação dos ângulos de tensão e corrente, para cáculo das potências aparente, ativa e reativa
de algum sistema elétrico genérico. Através de um circuito eletrônico, e conexão de um TP e um TC 
que devem isolar, e reduzir os sinais a um valor aceitável e seguro de tensão, para ser lido pela placa. 
Para isso será necessário que o mini computador possua os itens abaixo:

#### Opção escolhida: BeagleBoard:
Devido ao a Raspberry não possuir conversor A/D, e o CI com conversor A/D proposto MCP3008, possuir somente 1 conversor, a leitura seria medida com atraso (somente uma medição por vez). Optamos então pelo uso da placa beagleboard conectada a um adaptador WiFi, pois esta possui mais de 2 conversores A/D, o que possibilita leituras de tensão e corrente simultaneas.

- [x] Adaptador WiFi 802.11 B/G/N integrado
- [ ] 2 Entradas analógicas (2 conversores AD integrado)
- [x] Comunicação SPI - (utilizar CI 1 x conversor A/D MCP3008 com comunicação SPI)

![Imagem da Placa RaspBerry PI3](https://1.bp.blogspot.com/-kMfLw3oX-cM/V35bgGHg1_I/AAAAAAAASx4/VTPxcHNUSAghJXJlj-ecvcjF3h67-z6dACKgB/s1600/raspberry-pi-3-sri%2Blanka%2Bprice%2B%2Bby%2Bwww.aluth.com.jpg)

#### Opção Descartada: BeagleBoard

- [ ] Adaptador WiFi 802.11 B/G/N integrado
- [x] Porta Ethernet (conectar roteador WiFi 802.11 B)
- [x] 2 Entradas analógicas (2 x conversor AD integrado 12 bits)


![Imagem da Placa BigleBoard](https://i0.wp.com/cdn.makezine.com/uploads/2014/12/beaglebone-specs.png?resize=620%2C431)
