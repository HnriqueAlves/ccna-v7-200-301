                                         Quinta Aula
========================================================================================================
O que é Ethernet         10Mbps
        FastEthernet     100Mbps
        GigabitEthernet  1000Mbps
    
    C = Cabo Par Metalico
    F = Fibra 
    W = Rede sem fio 

Comando: 

enable
    configure terminal
        ip default-gateway 192.168.1.254
        interface vlan 1
            description Interface de SVI
            ip address 192.168.1.25X 255.255.255.0
            no shutdown
            end
    write

enable 
    configure terminal
        ip domain-name senac.intra
        crypto key generate rsa general-keys modulus 1024
        ip ssh version 2
        ip ssh time-out 60
        ip ssh authentication-retries 2
        line vty 0 4
            transport input ssh
            end
    write

Acesso Remoto Switch:

ssh -l senac 192.168.1.250

Comando de Teste:

    show runnig-config
    show ip interface brief
    ping 192.168.1.1
========================================================================================================
                                            Ethernet
            
    Ethernet é um conjunto de tecnologias de rede de computadores que permite a comunicação entre dispos-
    itivos dentro de uma rede local (LAN - Local Area Network). Foi desenvolvido nos anos 1970 pela Xerox 
    Corporation como uma maneira de conectar computadores em uma rede local para compartilhar recursos e 
    trocar informações.
========================================================================================================
                                            FastEthernet
                    
    Fast Ethernet é uma versão aprimorada da tecnologia Ethernet que oferece velocidades de transmissão 
    de dados mais rápidas do que as oferecidas pela Ethernet tradicional. Enquanto a Ethernet original 
    opera a 10 megabits por segundo (Mbps), o Fast Ethernet opera a 100 Mbps, proporcionando uma melhoria 
    significativa na velocidade de transmissão de dados em redes locais (LANs).
========================================================================================================
                                            GigabitEtehrnet
                        
    Gigabit Ethernet é uma tecnologia de rede que oferece uma velocidade de transmissão de dados de 1 
    gigabit por segundo (Gbps), ou seja, 1 bilhão de bits por segundo. Ela é uma evolução da tecnologia 
    Ethernet e uma versão mais rápida do que a Fast Ethernet, que opera a 100 megabits por segundo (Mbps).
========================================================================================================
                                                VLAN

Uma VLAN (Virtual Local Area Network) é uma técnica de segmentação de redes em um ambiente de rede local 
(LAN) em que dispositivos são agrupados logicamente, independentemente de sua localização física na rede. 
Isso permite criar redes virtuais isoladas dentro de uma rede física, proporcionando vantagens em termos 
de segurança, gerenciamento e eficiência.
========================================================================================================
                                                SSH
                                    
    SSH (Secure Shell) é um protocolo de rede utilizado para comunicação segura e criptografada entre dois 
    computadores. Ele foi desenvolvido para substituir métodos mais antigos e menos seguros de acesso 
    remoto e transferência de arquivos, como o Telnet e o FTP, que transmitiam dados de forma não cripto-
    grafada, tornando-os suscetíveis a interceptação e ataques.
    