# resumo-lab-02
resumo-lab-02


Resumo do Laboratório Azure DIO
Este laboratório explorou os principais benefícios e conceitos da nuvem pública, usando o Microsoft Azure como exemplo. Abaixo estão os pontos chave sobre como a nuvem garante disponibilidade e confiabilidade:

Acordo de Nível de Serviço (SLA)
O SLA (Service Level Agreement) é um acordo formal entre o provedor de nuvem (como a Microsoft) e o cliente. Ele define a porcentagem de tempo que um serviço estará disponível e funcionando.

Um SLA maior significa um tempo de inatividade (downtime) menor e uma disponibilidade maior. Isso, por sua vez, acarreta um custo mais alto.

Em resumo: quanto mais tempo seu serviço precisa estar online, mais você investe para garantir essa promessa de disponibilidade.

Zonas de Disponibilidade (Availability Zones)
Ao criar uma máquina virtual no Azure, você escolhe onde ela será alocada para garantir que o serviço permaneça ativo mesmo se houver uma falha em uma localização específica.

1 Zona: A máquina virtual está em um único datacenter dentro de uma região. Se esse datacenter falhar, o serviço ficará indisponível.

2 ou 3 Zonas: A máquina virtual é replicada em diferentes datacenters fisicamente isolados (zonas de disponibilidade) dentro da mesma região. Se uma zona falhar, o tráfego é automaticamente roteado para outra zona, garantindo a continuidade do serviço e uma indisponibilidade mínima. Mais zonas de disponibilidade proporcionam maior confiabilidade e menor tempo de inatividade, mas também aumentam o custo.

Contas de Armazenamento
A forma como você armazena seus dados também impacta a disponibilidade e a segurança. As contas de armazenamento no Azure oferecem diferentes opções de redundância para proteger seus dados contra falhas.

LRS (Local-Redundant Storage): Os dados são replicados três vezes dentro de um único datacenter. É a opção de menor custo e menor disponibilidade.

ZRS (Zone-Redundant Storage): Os dados são replicados em três zonas de disponibilidade diferentes, garantindo que estejam seguros mesmo que um datacenter inteiro falhe.

GRS (Geo-Redundant Storage): Os dados são replicados em uma região secundária a centenas de quilômetros de distância.

GZRS (Geo-Zone-Redundant Storage): Uma combinação das duas últimas. Os dados são replicados em várias zonas na região primária e, em seguida, replicados para uma segunda região, também com várias zonas.

A escolha do tipo de armazenamento afeta diretamente a durabilidade e o custo, pois cada nível de redundância oferece uma garantia diferente de que seus dados não serão perdidos.

Em conclusão, a nuvem oferece a flexibilidade para você escolher o nível de disponibilidade e segurança de acordo com suas necessidades e orçamento, permitindo um controle granular sobre o SLA dos seus serviços.
