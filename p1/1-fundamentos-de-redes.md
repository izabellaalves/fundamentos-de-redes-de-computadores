# Fundamentos de Redes de Computadores 

Uma rede de computadores é um conjunto de dois ou mais computadores interligados entre si através de um protocolo. As redes de computadores permitem que os dispositivos compartilhem recursos entre si, como arquivos e acesso à internet. 

## Principais dispositivos 

Alguns dispositivos comuns quando se está trabalhando com Redes de Computadores são: 

- **Roteadores**: Servem para conectar diferentes redes entre si. 
- **Switches**: Servem para conectar diferentes dispositivos a uma mesma rede. 
- **Firewalls**: Protegem as redes contra acesso não autorizado. 
- **Access Point**: Permitem que dispositivos se conectem a uma rede via Wi-Fi. 

## Protocolo TCP/IP

Para que todos os computadores de uma rede possam trocar informações entre si, é necessário que eles adotem as mesmas regras em relação ao envio e recebimento de informações. 

Essas regras são chamadas de Protocolo de Comunicação, e um deles é o Protocolo TCP/IP. 

Quando usamos o Protocolo TCP/IP como Protocolo de Comunição, existem alguns parâmetros que devem ser configurados nos dispositivos que fazem parte da rede, são eles: 

### IP (Internet Protocol)

O IP é um número que serve para identificar um dispositivo em uma rede, ele é formato por 4 números separados por ponto, e cada número tem como valor máximo 255. Segue um exemplo: 

```shell
X.Y.Z.W

192.168.10.5
```

Existem diferentes classes de IP, que determinam o tamanho da rede, elas são: 

- **Classe A**
    - Faixa de IPs: 1 até 127 
    - Máscara de sub-rede: 255.0.0.0
    - Destinada a receber grandes quantidades de Host (16 milhões)

- **Classe B**
    - Faixa de IPs: 128 até 191
    - Máscara de subrede: 255.255.0.0
    - Destinada uma média quantidade de Host (65 mil)
 
- **Classe C**
    - Faixa de IPs: 192 até 223
    - Máscara de subrede: 255.255.255.0
    - Destinada a uma pequena quantidade de Host (254 pessoas)
 
- **Classe D**
    - Faixa de IPs: 224 até 239
    - Utilizado para transmissões em grupo (multicasting)
    - Máscara de subrede: 239.255.255.255
 
- **Classe E**
    - Faixa de IPs: 240 até 255
    - Reservado para testes e pesquisa
    - Máscara de subrede: 255.255.255.255
    
Para se comunicar em uma rede que itiliza o Protocolo TCP/IP, todos os dispositivos devem ter um IP e uma máscara de sub-rede. Lembrando que todos os dispositivos de uma rede devem ter a mesma máscara de sub-rede. 

Para identificar o IP de uma rede, colocamos o 0 no final, da seguinte forma: 

```shell
X.Y.Z.0
```

Este é o endereço da rede. 


## Tipos de Redes de Computadores 

- **LAN:** LAN significa Local Area Network e é uma rede formada por servidores, computadores e outros dispositivos que estão no mesmo local físico, seja dentro de uma casa, uma empresa, etc.

- **MAN:** MAN significa Metropolitan Area Network e é uma rede de média distância, ela abrange uma cidade ou uma região metropolitana.

- **WAN:** WAN significa Wide Area Network e é uma rede de longa distância. Essas redes são responsáveis pela comunicação global.

- **WLAN, WMAN e WWAN:** São redes sem fio dos tipos vistos acima, elas podem usar Wi-Fi ou algum outro tipo de conexão.

- **PAN:** PAN significa Personal Area Network e são utilizadas para que dispositivos se conectem numa distância limitada, como Bluetooth.

## Topologia de Rede

A topologia diz respeito a como os dispositivos de uma rede estão interconectados ou como os dados são transmitidos entre eles. Alguns exemplos de topologias são:

- **Topologia em Estrela:** Nesta topologia todos os dispositivos são conectados a um HUB ou um Switch central. Ela é fácil de configurar mas se houver algum problema no HUB pode afetar todos os dispositivos.
- **Topologia em Barramento:** Nesta topologia todos os dispositivos são conectados a um só cabo, embora seja simples, se o cabo falhar pode afetar toda a rede.
- **Topologia em Anel:** Nesta topologia cada dispositivo está conectado a outros dois dispositivos, formando um loop fechado. Embora seja resistente a falhas individuais, pode acontecer da falha em um dispositivo atrapalhar toda a rede.
- **Topologia em Malha:** Esta topologia conecta um dispositivo a todos os outros dispositivos da rede, embora seja bem confiável, é mais complexa e requer mais cabos.
- **Topologia em Árvore:** É uma combinação de outras topologias. Nela, os dispositivos individuais são conectados a um HUB ou Switch formando uma topologia em estrela, e os HUBs ou Switchs de cada grupo são conectados ao mesmo barramento.
- **Topologia Ponto-a-Ponto:** É uma topologia de rede que conecta dois dispositivos diretamente.
- **Topologia Daisy-Chain:** A topologia Daisy Chain conecta dispositivos em série, um após o outro, até chegar ao destino.

A topologia de rede mais utilizada é a em estrela.

---

## ✅ Questões Objetivas (Múltipla Escolha)

1. **Qual dispositivo de rede é responsável por conectar diferentes redes entre si?**  
   a) Switch  
   b) Access Point  
   c) Firewall  
   d) Roteador - certo

2. **Qual das alternativas representa corretamente um endereço IP Classe C?**  
   a) 10.0.0.1  
   b) 172.16.0.1  
   c) 192.168.1.1 - certo
   d) 224.0.0.1  

3. **Qual das topologias de rede conecta todos os dispositivos a um único cabo, tornando a rede vulnerável caso esse cabo seja danificado?**  
   a) Estrela  
   b) Malha  
   c) Barramento - certo
   d) Anel  

4. **Em relação às máscaras de sub-rede, qual é a correta para a Classe B?**  
   a) 255.0.0.0  
   b) 255.255.255.0  
   c) 255.255.0.0 - cert0
   d) 255.255.255.255  

5. **Qual tipo de rede é projetado para cobrir uma área como uma cidade inteira?**  
   a) LAN  
   b) MAN - certo
   c) WAN  
   d) PAN  

6. **O que é necessário para que dois dispositivos consigam se comunicar em uma rede TCP/IP?**  
   a) Ter o mesmo endereço MAC  
   b) Estar na mesma rede física  
   c) Ter IPs diferentes e mesma máscara de sub-rede - certo
   d) Ter o mesmo endereço IP  

---

## 🧠 Questões Discursivas

7. **Explique a função de cada um dos seguintes dispositivos de rede: Roteador, Switch, Access Point e Firewall.**

Um roteador serve para conectar diferentes redes entre si, um Switch serve para conectar diferentes dipositivos entre si, um Access Point serve para conectar uma rede à uma rede cabeada via Wi-Fi e um Firewall serve para proteger a rede contra acesso não autorizado.

8. **Descreva o que é uma máscara de sub-rede e qual a sua importância em uma rede TCP/IP.**

A máscara de sub-rede é um conjunto de quatro números separados por ponto que indica qual parte do endereço IP representa a rede e qual parte representa os dispostivos, ela é importante para uma rede TCP/IP pois descreve qual é a classe da rede, quantos usuários podem ter naquela rede e também é necessária para o funcionamento de uma rede pois todos os dispositivos de uma rede devem ter uma máscara de subrede.

9. **Compare as topologias Estrela, Barramento e Malha em termos de confiabilidade, custo e complexidade.**

A topologia em estrela tem uma confiabilidade baixa, um custo médio e uma complexidade baixa.
Uma topologia em barramento tem uma confiabilidade baixa, um custo baixo e uma complexidade baixa.
Uma topologia em malha tem uma confiabilidade alta, um custo alto e uma complexidade alta.

10. **O que significa o endereço IP `192.168.10.0` em uma rede? E por que usamos o `.0` no final?**

Este endereço de IP é o Network ID, e o 192 no começo indica que pertence a classe C. O ".0" no final indica que este é o endereço da rede.

---

## 🧩 Questões de Associação

11. **Associe os tipos de redes às suas características:**

| Tipo de Rede | Característica                                   |
|--------------|--------------------------------------------------|
| ( A ) LAN    | ( A ) Conecta dispositivos em uma casa           |
| ( B ) MAN    | ( B ) Abrange cidades inteiras                   |
| ( C ) WAN    | ( C ) Rede usada por grandes corporações         |
| ( D ) PAN    | ( P ) Comunicação de curto alcance, como Bluetooth |

---

## 🔧 Questões Práticas / de Aplicação

12. **Você precisa configurar uma rede em um pequeno escritório com 20 computadores. Qual classe de IP e máscara de sub-rede você escolheria e por quê?**

Escolheria a classe C, que tem a máscara de subrede 255.255.255.0. Pois essa classe suporta até 254 dispositivos, que é bem mais do que o necessário para esta rede. Todas as outras classes podem ter muito mais dispositivos do que o necessário para esta.

13. **Imagine que sua rede doméstica parou de funcionar. Após testes, você identificou que o problema está no dispositivo que conecta todos os outros. Qual topologia essa rede provavelmente utiliza e qual é o dispositivo problemático?**

Provavelmente é uma topologia em estrela, e o dispositivo central é um Switch ou um HUB.