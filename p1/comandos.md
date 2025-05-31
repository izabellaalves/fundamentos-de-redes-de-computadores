# Configuração Inicial de Switch no Packet Tracer

## Modos de Operação

Existem três modos de operação, o modo Usuário (enable), o modo Privilegiado (configure terminal) e o modo de Configuração Global.

### ```enable```

Entra no modo privilegiado. (Switch#)

### ```configure terminal``` ou ```conf t ```

Entra no modo de configuração global.

## Configurações básicas do dispositivo

### ```hostname NOME```

Define um nome para o dispositivo.

### ```banner motd #mensagem#```

Define uma mensagem de aviso ao acessar o dispositivo.

### ```no ip domain lookup```

Desativa as traduções.

### ```copy running-config startup-config``` ou ```wr```

Salva as configurações feitas.

### ```exit```

Sai do modo de configuração atual.

## Segurança 

Ter uma senha no console é de extrema importância para a segurança do equipamento pois evita acessos não autorizados. A porta console da acesso total ao equipamento, então, alguém indesejado pode tentar derrubar a rede ou fazer algo errado caso não tenha nenhuma verificação.

### ```line console 0```

Acessa configuração da porta console. O 0 indica a primeira porta virtual.

### ```password SENHA```
Define uma senha para o console.

### ```login```

Obriga o uso da senha definida no console.

## Configuração do Gateway no Roteador

Um gateway é a porta de acesso da sua rede para as outras redes, através dele os dados podem ser enviados para outras redes e recebidos de outras redes, como entre uma rede local (LAN) e a internet.

### ```show ip interface brief```

Exibe as interfaces e estados das portas.

### ```interface gigabitetheret0/0/0``` ou ```int g0/0/0```

Entra na configuração da interface em questão.

### ```ip address IP MASCARA```

Define o IP da interface e a máscara de subrede.

### ```no shutdown```

Ativa a interface.

## Protocolo de Roteamento RIP

explicar para q serve o protocolo RIP

### ```router rip```

Inicia a configuração do protocolo RIP.

### ```network 192.168.10.0```

Informa que esta rede faz parte do protocolo RIP.

## VLAN no Switch

explicar o q é vlan

### ```show vlan brief```

Exibe as VLANs existentes.

### ```vlan N```

Cria uma VLAN com o número N.

### ```name NOMEDAVLAN```

Atribui um nome a VLAN criada.

### ```interface range fa0/1-10```

Seleciona um intervalo de interfaces.


### ```switchport access vlan N```

Atribui as interfaces para a VLAN desejada.

## Cabos

### Cabo Console

O cabo console é utilizado para conectar um computador diretamente a um Switch ou um roteador via porta console, através disso, podemos usar o terminal do computador para fazer as configurações iniciais do dispositivo.

### Cabo Crossover

O cabo Crossover é utilizado para conectar dispositivos do mesmo tipo.

### Cabo serial DCE

O cabo serial DCE é utilizado para conectar dois roteadores através de interfaces seriais. É necessário criar uma nova rede quando este cabo é usado.

### Cabo Straight-through

O cabo Straight-through é utilizado para conectar dispositivos diferentes.

## Conceitos Importantes

### Gateway

O gateway é o ponto de acesso da sua rede para outras redes.

### VLAN

VLAN é uma forma de segmentar uma rede física em várias redes lógicas. Por exemplo, tenho vários computadores conectados a apenas um Switch, mas posso criar diferentes VLAN's e atribuir computadores diferentes para cada VLAN.

### DHCP

DHCP é um protocolo configurado no servidor para atribuir IPs de forma automática pros dispositivos da rede.

### DNS

DNS é um protocolo responsável por traduzir nomes de domínio em endereços IP.

### UDP

UDP é um protocolo de transporte muito utilizado para vídeos e áudio pois envia dados de forma rápida, mas sem garantir que os dados foram recebidos corretamente.

### RIP

RIP é um protocolo de roteamento dinâmico utilizado para trocar informações entre os roteadores.

# 📝 Questionário - Configuração Inicial de Switch e Roteador no Packet Tracer

## Modos de Operação

1. Quais são os três modos de operação de um switch ou roteador?

Modo usuário (Switch>), Modo privilegiado (Switch#) e Modo de Configuração Globaç (Switch(config)#).

2. Para que serve o comando `enable`?
O comando enable serve para avançar pro modo de operação Privilegiado quando se está no modo de usuário.

3. O que o comando `configure terminal` permite fazer?
O comando configure terminal serve para avançar para o modo de Configuração Global quando se está no modo privilegiado.

## Configurações Básicas

4. Qual comando define um nome personalizado para o dispositivo?
hostname NOME

5. Como definir uma mensagem de aviso exibida ao acessar o equipamento?
banner motd #mensagem#

6. Para que serve o comando `no ip domain lookup`?
Este comando serve para evitar que o dispositivo tente corrigir nomes digitados incorretamente.

7. Qual comando é usado para salvar a configuração atual do dispositivo?
Copy running-config startup-config ou wr.

8. O que acontece se você não usar o `copy running-config startup-config` após configurar?
Você perde suas configurações.


## Segurança

9. Por que é importante definir uma senha para o console do dispositivo?
Pois através da porta console é possível acessar todas as configurações do dispositivo, e sem uma senha o dispositivo fica vúlneravel a qualquer um que possa plugar um cabo na porta console.

10. Qual comando entra na configuração da porta console?
line console 0.

11. O que faz o comando `password SENHA`?
Define a senha da porta console como SENHA.

12. Qual comando obriga o uso da senha no console?
login

13. O que significa o número `0` em `line console 0`?
Indica que a porta virtual é a 0.

## Gateway e IP

14. O que é um gateway em uma rede?
Um gateway é a porta de acesso da rede para outras redes, ele representa o dispositivo que faz a ligação entre diferentes redes, geralmente um roteador.

15. Qual comando exibe o status das interfaces do dispositivo?
show ip interface brief.

16. Como você entra na configuração da interface `GigabitEthernet0/0/0`?
interface gigabitethernet0/0/0 ou int g0/0/0.

17. Qual comando atribui um IP a uma interface?
ip address IP MASCARA.

18. Para que serve o comando `no shutdown`?
Para ativar a interface.

## Protocolo RIP

19. Para que serve o protocolo RIP?
O protocolo RIP serve para roteamento dinâmico, ou seja, permite que roteadores troquem informações de rota automaticamente.

20. Qual comando inicia a configuração do protocolo RIP?
router rip

21. Como indicar que a rede `192.168.10.0` deve participar do RIP?
network 192.168.10.0

## VLAN

22. O que é uma VLAN e qual sua utilidade?
VLAN é uma operação que permite que um tenhamos várias redes lógicas num unico dispositivo físico, ela é útil caso só se tenha um equipamento, mas seja necessário ter diferentes redes, seja para setores de uma empresa, etc.

VLAN permite SEGMENTAR uma rede física em diferentes redes lógicas.

23. Como visualizar as VLANs existentes no switch?
show vlan brief

24. Qual comando cria uma VLAN de número 10?
vlan 10

25. Como atribuir um nome a uma VLAN?
name NOME

26. O que faz o comando `interface range fa0/1-10`?
Define quais interfaces fazem parte de um range, neste caso, da interface fa0/1 até fa0/10.

27. Como associar uma interface a uma VLAN específica?
switchport access vlan N.

## Cabos de Rede

28. Para que serve o cabo console?
O cabo console serve para plugar em dispositivos e conseguir acessar seu terminal através de outro dispositivo, por exemplo, conectar um notebook em um switch e fazer as configurações do switch pelo terminal do notebook.

29. Qual cabo é usado para conectar dispositivos do mesmo tipo?
Para conectar dispositivos do mesmo tipo é o cabo cross over.

30. Qual cabo é necessário para conectar dois roteadores via interface serial?
Cabo serial DCE.

31. Por que é necessário criar uma nova rede ao usar um cabo DCE?

Porque a comunicação serial representa um novo enlance de rede, que requer endereço próprio.


32. Qual cabo é utilizado para conectar dispositivos de tipos diferentes?
Cabo Straight-through

## Conceitos Fundamentais

33. O que é o protocolo DHCP e qual sua função em uma rede?
O protocolo DHCP é um protocolo utilizado para atribuir IPs de forma automatica aos dispositivos da rede.

34. O que o protocolo DNS realiza?
O protocolo DNS serve para fazer a tradução de um nome de domínio em um endereço IP.

35. Em que situações o protocolo UDP é preferido e por quê?
É preferido em casos em que é necessário que a informação chegue de forma rápida, mesmo que alguma parte do conteúdo possa se perder. Pois o protocolo UDP é rápido mas não garantea confiabilidade da entrega.

Quando a velocidade é mais importante que a confiabilidade, como em vídeo ou jogos online.

36. O que é o protocolo RIP e por que ele é classificado como um protocolo de roteamento dinâmico?

Ajusta-se dinâmicamente a topologia de rede.


---

