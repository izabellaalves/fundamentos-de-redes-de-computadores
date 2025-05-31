# Modelo OSI X Modelo TCP/IP

## Modelo OSI

OSI é a sigla para Open System Interconnection, ou seja, Interconexão de Sistemas Abertos. É um modelo que define 7 camadas para que sistemas de computadores possam usar para se comunicar em uma rede.

O Modelo OSI é o primeiro modelo de Protocolo de Comunicação e define 7 camadas para garantir a comunicação dos dispositivos em uma rede.

O Modelo OSI é um modelo conceitual e abstrato que define o cenário ideal de como uma rede deveria se comunicar.

### Camadas do Modelo OSI

1. Aplicação: esta camada é onde o usuário interage com a rede, como a interface utilizada.
2. Apresentação: esta camada cuida da apresentação dos dados, cuida de como os dados serão formatados, codificados e protegidos,
3. Sessão: esta camada abre, mantém e fecha a sessão de comunicação entre dois dispositivos.
4. Transporte: esta camada garante que os dados cheguem corretamente ao programa certo dentro do computador de destino. Para isso, usa os protocolos TCP e UDP.
5. Rede: esta é uma camada de roteamento, ela introduz a capacidade de rotear o tráfego de um ponto da rede a outro, por meio de sub-redes. De forma simplificada, essa camada é responsável por descobrir a melhor rota entre duas redes.
6. Enlace de Dados: esta camada é responsável pela organização dos dados a serem enviados em conjuntos de bits denominados **quadros** (frames) e endereçamento físico com endereços MAC.
7. Física: esta camada trata da sinalização da rede e da conversão de bits em sinais elétricos. Nesta camada temos cabos, switchs, roteadores, etc.


### PDU (Protocol Data Unit)

Nas camadas do modelo OSI, cabeçalhos contendo informações são adicionados aos dados a serem transmitidos, este ato se chama encapsulamento.

Em cada camada, possui uma estrutura própria e damos um nome específico ao conjunto de dados com informações encapsuladas. Chamamos esses conjuntos de "PDU".

## Modelo TCP/IP

O Modelo TCP/IP também é um protocolo de comunicação, mas ao contrário do Modelo OSI, este modelo só possui quatro camadas. Elas são:

1. Aplicação: onde estão os protocolos que os aplicativos usam para se conectar com a rede, como HTTP, HTTPS, DNS, FTP, etc.
2. Transporte: Permite que programas em diferentes computadores conversem entre si com seguraçna e eficiencia, utilizando o protocolo TCP (confiável e garante a entrega) ou UDP (sem garantia mas é mais leve, ideial pra vídeo, aúdios, etc).
3. Internet: Esta camada permite que os pacotes IP cheguem de um computador a outro, mesmo que estejam em redes diferentes.
4. Host/Rede: esta camada conecta o computador (host) à rede física. O modelo TCP/IP não define um protocolo específico aqui, apenas exige que seja possível enviar pacotes IP.

## Modelo TCP/IP X Modelo OSI

| Modelo OSI                   | Modelo TCP/IP         | Função Principal                                        |
|-----------------------------|------------------------|---------------------------------------------------------|
| 7. Aplicação                | 4. Aplicação           | Interface com os aplicativos do usuário (HTTP, FTP...)  |
| 6. Apresentação             | 4. Aplicação           | Formatação, compressão e criptografia dos dados         |
| 5. Sessão                   | 4. Aplicação           | Controle e gerenciamento das sessões de comunicação     |
| 4. Transporte               | 3. Transporte           | Comunicação entre processos, controle de erros e fluxo  |
| 3. Rede                     | 2. Internet             | Roteamento de pacotes e endereçamento IP                |
| 2. Enlace de Dados (Link)   | 1. Host/Rede            | Comunicação entre dispositivos da mesma rede            |
| 1. Física                   | 1. Host/Rede            | Transmissão física dos bits (cabos, sinais, etc.)       |


## Pilha de Protocolos da Internet

A internet utiliza uma pilha de protocolos mista, ou seja, ela é o resultado de duas pilhas de protocolo, a TCP/IP e a OSI. No final fica assim:

5. Aplicação
4. Transporte
3. Rede
2. Enlace
1. Física

# Questões sobre o Modelo OSI x Modelo TCP/IP

### 1. Qual é a principal função do Modelo OSI?
- ( ) Conectar dispositivos físicos na rede  
- ( ) Definir protocolos de transporte como o TCP  
- ( ) Garantir segurança na comunicação via internet  
- (X) Definir camadas conceituais para comunicação entre sistemas abertos  

---

### 2. Quantas camadas existem no Modelo OSI?
- ( ) 4  
- (X) 7  
- ( ) 5  
- ( ) 3  

---

### 3. Em qual camada do Modelo OSI ocorre o roteamento de pacotes?
- ( ) Aplicação  
- ( ) Enlace de Dados  
- (X) Rede  
- ( ) Transporte  

---

### 4. A camada de **Transporte** no Modelo OSI utiliza quais protocolos para garantir a entrega dos dados?
- (X) TCP e UDP  
- ( ) IP e HTTP  
- ( ) FTP e DNS  
- ( ) SSL e TLS  

---

### 5. A camada de **Apresentação** no Modelo OSI é responsável por:
- ( ) Encaminhar pacotes entre redes  
- ( ) Transmitir bits por cabos físicos  
- (X) Codificar, comprimir e criptografar dados  
- ( ) Estabelecer e manter sessões de comunicação  

---

### 6. Qual camada do Modelo OSI organiza os dados em quadros (frames) e usa o endereço MAC?
- ( ) Sessão  
- (X) Enlace de Dados  
- ( ) Física  
- ( ) Rede  

---

### 7. Qual é a estrutura usada para representar os dados em cada camada do Modelo OSI?
- ( ) Bitstream  
- (X) Pacote  
- ( ) Cabeçalho  
- ( ) PDU (Protocol Data Unit)  

---

### 8. O Modelo TCP/IP possui quantas camadas?
- ( ) 7  
- ( ) 5  
- (X) 4  
- ( ) 6  

---

### 9. Qual camada do Modelo TCP/IP é responsável pelo endereçamento IP e roteamento?
- ( ) Aplicação  
- ( ) Transporte  
- (X) Internet  
- ( ) Host/Rede  

---

### 10. Em qual camada do Modelo TCP/IP se encontram os protocolos como HTTP, FTP e DNS?
- (X) Aplicação  
- ( ) Transporte  
- ( ) Internet  
- ( ) Host/Rede  
