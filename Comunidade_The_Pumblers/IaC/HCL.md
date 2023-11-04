Especificação de sintaxe nativa da HCL
Esta é a especificação da sintaxe e semântica da sintaxe nativa para LCP. HCL é um sistema para definir linguagens de configuração para aplicações. O modelo de informação HCL é projetado para suportar múltiplas sintaxes concretas para configuração, mas essa sintaxe nativa é considerada o formato primário e é otimizado para criação e manutenção humana, em oposição à máquina geração de configuração.

A linguagem consiste em três sublinguagens integradas:

A linguagem estrutural define a configuração hierárquica geral estrutura, e é uma serialização de corpos, blocos e atributos HCL.

A linguagem de expressão é usada para expressar valores de atributo, como literais ou como derivações de outros valores.

A linguagem do modelo é usada para compor valores juntos em cadeias de caracteres, como um dos vários tipos de expressão na linguagem de expressão.

Em uso normal, esses três subidiomas são usados juntos na configuração arquivos para descrever uma configuração geral, com a linguagem estrutural sendo usado no nível superior. As linguagens de expressão e modelo também podem ser usado isoladamente, para implementar recursos como REPLs, depuradores e integração em sintaxes HCL mais limitadas, como o perfil JSON.

[Link](https://github.com/hashicorp/hcl/blob/main/hclsyntax/spec.md)