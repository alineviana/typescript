# TypeScript

### Inferência de tipos:
- Permite ao compilador deduzir automaticamente o tipo de uma variável, função, expressão ou objeto com base em seu valor e uso no código.

### Interface:
- Uma forma de definir a estrutura de um objeto, especificando quais propriedades e métodos ele deve ter. Isso facilita a criação de tipos personalizados e ajuda a garantir que os objetos em seu código atendam aos requisitos desejados.

### Generic:
- Permitem que você parametrize tipos, valores ou comportamentos, tornando possível escrever código que funcione com vários tipos diferentes sem sacrificar a verificação de tipos estática que o TypeScript oferece

### Extends:
- Através do uso da palavra-chave extends, podemos herdar propriedades de interfaces ou tipos existentes, o que nos permite criar componentes que aproveitam propriedades de outros componentes ou elementos.

### Ferramenta útil: 
- Transform json to typescript

<br><br>

No TypeScript, tanto type quanto interface são usados para criar definições de tipos e estruturas de dados personalizadas. No entanto, eles têm algumas diferenças chave em termos de funcionalidade e comportamento:

### - Declaração:
- Interface: É mais adequada para definir estruturas de objetos, classes e contratos em geral. Também é usada para descrever a forma de objetos e a estrutura de classes.
- Type: É usado para criar tipos personalizados que podem representar qualquer tipo, incluindo primitivos, uniões, interseções e mais.

### - Extensibilidade:
- Interface: É facilmente extensível usando a palavra-chave extends, o que permite criar interfaces que herdam propriedades e métodos de outras interfaces.
- Type: Não é diretamente extensível. Você pode usar uniões e interseções para criar tipos mais complexos, mas não há uma sintaxe direta de extensão.

### - Herança:
- Interface: Permite herdar de outras interfaces usando a palavra-chave extends.
- Type: Não permite herança direta de tipos. Você pode alcançar herança usando uniões e interseções.

### - Interseção:
- Interface: Pode ser estendida por meio de interseção (A & B), combinando várias interfaces em uma.
- Type: Também suporta interseções, permitindo criar tipos complexos combinando outros tipos.

### - União:
- Interface: Não suporta uniões diretamente.
- Type: Pode representar uniões usando | para combinar diferentes tipos.

### - Declarar múltiplas vezes:
- Interface: Pode ser declarada múltiplas vezes usando a mesma identificação, e as declarações serão mescladas.
- Type: Não permite declarações múltiplas com a mesma identificação.

### - Compatibilidade de atribuição:
- Interface: As interfaces têm verificação de compatibilidade estrutural mais rigorosa.
- Type: Ocasionalmente, tipos podem ser mais flexíveis na verificação de compatibilidade.

<br><br>

### Em resumo, a escolha entre type e interface depende das suas necessidades. Use interface para definir contratos, estruturas de classe e herança. Use type para criar tipos personalizados, especialmente quando você precisa de uniões, interseções ou tipos mais complexos. Em muitos casos, a escolha entre os dois é uma questão de preferência e de se adequar ao estilo do seu código.