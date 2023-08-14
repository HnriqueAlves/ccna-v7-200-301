                                           Quarta Aula
========================================================================================================

    1 Preço Switch Cisco Catalyst 2960 24 Portas

    Comandos:
    1º enable (Aumento de Privilégio)
        2º clock set (Serve para Setar a Data/Hora do Switch)
        3º configure terminal (Ativa um Modo Global de Comfiguração do Switch)
            4º hostname (Modifica o Nome do Switch)
            5º service password-encryption (Serve para criar uma senha para segurança)
            6º service timestamps log datetime msec (Serve para poder avizar quando ouver algum problema 
            na rede do Switch)
            7º no ip domain-lookup (Serve para desativar uma veirificação automatica quando erra um comando)
            8º banner motd (Serve para avisar sobre as autorizações)
            9º enable secret (Serve para que toda vez que for entrar com o comando enable ele irá te pedir 
            uma senha)
            10º end (Serve para Sair de todas as etapas)
        11º copy running-config startup-config
    12° disable (Desativa o Modo de Privilégio)
    13º exit
========================================================================================================
enable 
    configure terminal  
        username senac secret 123@senac
        line console 0
            login local
            password 123@senac
            logging synchronous
            exec-timeout 5 30
            end
    write (Significa salvar)
enable
    confgure terminal
        line vty 0 4
            login local
            passoword 132@senac
            logging synchronous
            exec-timeout 5 30
            transport input all
            end
    write
========================================================================================================
                                            Switch Layer2
                        
    Uma Switch Layer 2, também conhecida simplesmente como switch de camada 2, é um dispositivo de rede 
    usado para encaminhar tráfego dentro de uma rede local (LAN) com base nos endereços MAC (Media 
    Access Control) dos dispositivos conectados. A camada 2 refere-se à camada de enlace no modelo OSI 
    (Open Systems Interconnection), que lida com o controle de acesso ao meio físico e à detecção de 
    erros.

========================================================================================================
                                            Switch Layer3
    
    Uma Switch Layer 3, também conhecida como switch de camada 3 ou switch roteadora, é um dispositivo 
    de rede que combina as funcionalidades de uma switch de camada 2 e um roteador de camada 3. Ela 
    opera nas camadas 2 (Enlace) e 3 (Rede) do modelo OSI e é capaz de tomar decisões de encaminhamento 
    com base em endereços IP.
========================================================================================================
                                                OSI 
    
    O Modelo OSI (Open Systems Interconnection) é um framework conceitual que foi desenvolvido pela 
    International Organization for Standardization (ISO) para descrever como os diferentes protocolos 
    de redes de computadores interagem e funcionam em diferentes camadas. Ele serve como um guia para a 
    criação de padrões de comunicação de rede e facilita a compreensão das complexas interações entre os 
    componentes de uma rede.
========================================================================================================
                                                LGPD
    
    A LGPD, ou Lei Geral de Proteção de Dados, é uma legislação brasileira que regula a coleta, o uso, o 
    armazenamento e a transferência de dados pessoais no país. Ela foi inspirada no Regulamento Geral de 
    Proteção de Dados (GDPR) da União Europeia e tem como objetivo proteger a privacidade e os direitos 
    dos cidadãos em relação às suas informações pessoais.
========================================================================================================
                                            Memoria Volátil

    Memória volátil é um termo utilizado na computação para descrever um tipo de memória de computador 
    que perde os dados armazenados nela quando a energia elétrica é desligada. Isso significa que os 
    dados armazenados na memória volátil não são retidos após um desligamento ou reinicialização do 
    sistema.