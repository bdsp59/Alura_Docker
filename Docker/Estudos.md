# DOCKER

Considerando um ambiente de trabalho onde tenhamos a necessidade de termos diversas aplicações rodando, cada uma com um tipo de linguagem
e um tipo de versão dessa linguagem, mas todas tento a necessidade de se utilizar a mesma porta de acesso em determinado momento.
Se tal situação ocorrer precisamos ter uma maneira de separar essas aplicações de modo que uma não interfira no funcionamento da outra,
podemos pensar em algumas soluções:
    - Utilizar uma máquina para cada aplicação, mas não é uma solução viável visto que o custo seria muito elevado;
    - Utilizar máquinas virtuais para cada aplicação de modo que ficassem independentes do sistema operacional principal. Mas para essa situação
    teremos a necessidade de ter um Hypervisor, responsável por contextualizar o SO da VM, deixando o SO original isolado;
    - Utilizar containers para separar cada aplicação. Deixamos de ter necessidade de utilizar um Hypervisor, visto que agora o container fará o 
    isolamento do SO. 

Dependendo do que se queira fazer e da maneira que se queira fazer, podemos fazer uso de VM ou containers. Nesse curso vamos ver a utilização de 
containers.

## Como Containers Funcionam
     - Containers vão funcionar como processos dentro do SO. O que nos garante um consumo de recursos menor que as VMs, visto que teremos processos 
    e não virtualizações.

## Namespace
    - É um conceito que permiti garantir o isolamento, entre processos no nosso SO, em determinados níveis.
    - Principais Namespace
