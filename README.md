# Indentação e Comentários em Python
## Descrição
Este repositório contém o trabalho sobre boas práticas de indentação e comentários em Python proposto pelo professor Juliano Silva. Elaborado pelo Grupo 2 da Turma ATT do curso de Desenvolvimento de Sistemas na escola técnica Proz Educação.
## 📋 Sumário

1. Introdução


2. Indentação de Código

3. Comentários em Programação


4. Exemplos Práticos

5. Conclusão


### 1.0 Introdução

- **Apresentação do Tema:** 

A importância da indentação de código e dos comentários em programação se dá ao fato de que a indentação organiza visualmente o código, tornando mais fácil para os desenvolvedores compreenderem a estrutura e a lógica do programa.
 Ela ajuda a delinear claramente as diferentes seções de código, como loops, condições e funções, facilitando a compreensão da hierarquia e do fluxo do programa e, outro ponto é que um código bem indentado é mais fácil de modificar, pois a estrutura lógica é evidente, reduzindo o risco de introduzir erros ao alterar o código.

E já os comentários explicam partes específicas do código, tornando mais fácil para outros desenvolvedores entenderem a lógica e a finalidade de certas implementações, além de facilitar nossas revisões, pois eles nos ajudam fornecendo contexto e explicações adicionais para os revisores.
Os comentários são bem comum para ser usados para registrar o histórico de alterações e as razões para determinadas mudanças no código, em projetos colaborativos, os comentários servem como um meio de comunicação entre os desenvolvedores, ajudando a coordenar esforços e esclarecer dúvidas e eles também ajudam a lembrar os desenvolvedores das funcionalidades e propósitos do código, facilitando a atualização e a manutenção do software.



- **Objetivo Geral:** 

Compreender boas práticas de indentação e comentários para melhorar a legibilidade e manutenção do código.

### 2.0 Indentação de Código
#### 2.1 Conceito de Indentação

A indentação em Python é a maneira de agrupar comandos em blocos, no console interativo padrão você terá que digitar tab ou espaços para indentar cada linha. 


A maioria dos editores de texto tem facilidades de indentação automática. Quando um comando composto é digitado interativamente, deve ser finalizado por uma linha em branco (já que o interpretador não tem como adivinhar qual é a última linha do comando). Observe que toda linha de um mesmo bloco de comandos deve ter a mesma indentação.
Basicamente indentar é um termo utilizado para escrever o código do programa de forma hierárquica, facilitando assim a visualização e o entendimento do programa. 

O exemplo abaixo mostra um código indentado:


![Screenshot_1](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/34b906ca-388f-4aef-b890-6225a96e1bad)

#### 2.2 Qual a sua importância?


A indentação é bastante importante. Para pessoas que seguem profissões de programação há que ter em conta que não estamos a trabalhar sozinhos e que outras pessoas poderão ter de via a pegar no nosso trabalho. Quem diz a indentação diz o uso de comentários.

Algumas empresas grandes como a Google/Microsoft têm até regras de organização de código para diferentes projetos. Estas regras incluem indentação/comentários/organização do código em geral etc.

NOTA: A indentação na maioria das linguagem de desenvolvimento é apenas uma questão de estética do código, isto é, caso você optar por não realização a indentação e o código estiver correto, o mesmo será compilado/executado sem problemas.

##### “Qualquer idiota pode escrever código que um computador entenda. Bons programadores escrevem código que humanos podem entender.” MARTIN FOWLER

### 2.3 Boas Práticas de Indentação

- **Consistência:** A consistência na indentação é muito importante pois garante a legibilidade e a manutenção do código. Quando nós desenvolvedores seguimos as mesmas regras de indentação, o código torna-se mais fácil de ler e entender. Isso é especialmente importante em projetos colaborativos, pois lá é onde múltiplos desenvolvedores trabalham no mesmo código.



- **Espaços vs. Tabs:** Existem duas principais maneiras de fazer a indentação do código: usando espaços ou tabs. A escolha entre espaços e tabs pode afetar a maneira como o código é exibido em diferentes editores de texto e pode ser fonte de conflitos em equipes de desenvolvimento.


**Espaços**

Usar espaços pode garantir que a indentação seja exibida da mesma forma em qualquer editor ou IDE, já que o número de espaços é fixo.


**Tabs**

Tabs: Usar tabs permite que cada desenvolvedor configure o editor para exibir o código com a largura de tabulação que preferir. No entanto, pode levar a inconsistências se os editores não estiverem configurados corretamente.


A seguir um exemplo de como você pode configurar a quantidade de espaços quando utilizar a tecla TAB no Visual Studio Code.

## File > Preferences > Settings
![Print Tab Size](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/1e918972-c47e-4c14-b328-ea3ee5ef2557)




- **Níveis de Indentação:** A correta utilização dos níveis de indentação ajuda a definir a estrutura lógica do código, tornando-o mais fácil de entender e seguir o fluxo do programa. Para melhorar as boas práticas, nós programadores podemos manter as funções e métodos curtos, evitando níveis profundos de indentação. Podemos considerar que  a refatoração do código é importante se os níveis de indentação se tornarem muito profundos, pois isso pode indicar uma complexidade excessiva.



- **Aumento de Nível de Indentação:**
  - **Blocos de Código:** Aumentar a indentação ao entrar em um novo bloco de código, como dentro de funções, loops, condições (if/else).
  - **Exemplo:**
    ```python
    def funcao_exemplo():
        if condicao:
            for item in lista:
                print(item)
    ```
- **Diminuição de Nível de Indentação:**
  - **Fim de Blocos de Código:** Diminuir a indentação ao sair de um bloco de código.
  - **Exemplo:**
    ```python
    def outra_funcao():
        while condicao:
            if outra_condicao:
                executar_algo()
            else:
                executar_outro()
        executar_final()
    ```

###### " Os programadores dependem bastante desse esquema de indentação. Eles alinham visualmente na esquerda as linhas para ver em qual escopo elas estão. Isso lhes permite pular escopos, como de implementações de estruturas if e while, que não são relevantes no momento. Eles procuram na esquerda por novas declarações de métodos, novas variáveis e até novas classes. Sem a indentação, os programas seriam praticamente ininteligíveis para humanos " Robert Cecil Martin - Clean Code


#### 2.4 Padrões de Indentações em Diferentes Linguagens e Exemplos Práticos

**Python:**

Em Python, a indentação não é apenas uma questão de estilo, mas também uma parte sintática da linguagem, pois define blocos de código.

![6dfc77f8-7419-400c-b788-db63a0c85db7](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/fd528d7e-08e5-425c-87ad-53fe02ee8ba7)

**Java:** 

O padrão de indentação amplamente utilizado em Java é usar 4 espaços por nível de indentação, sem tabulações. As chaves de abertura são geralmente colocadas na mesma linha da declaração (K&R Style).

![7e5a4a81-ef94-4b14-839c-b05823f3e6f8](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/5bf5d3db-4c98-4540-8395-718c7ab49add)

**JavaScript:**

O padrão de indentação amplamente utilizado em JavaScript é usar 2 espaços por nível de indentação, sem tabulações. Esse padrão é recomendado em várias guias de estilo populares, como o guia de estilo do Google para JavaScript e o guia de estilo do Airbnb.

![57d3b1d5-00e6-4b14-bb98-8aa83d5dd538](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/ed058ddc-0ecd-4070-b09c-04eccb495134)

#### 2.5 Ferramentas e Recursos 

**IDEs e Editores de Texto**

Existem várias ferramentas e recursos para ajudar a garantir uma indentação consistente em projetos de programação. Editores de código como Visual Studio Code (VS Code) e IntelliJ IDEA têm configurações personalizáveis para indentação e suporte para extensões como Prettier e ESLint para formatação automática. Eclipse também oferece ferramentas de formatação integradas e suporte para Java, enquanto Sublime Text permite a personalização da indentação e a utilização de plugins como SublimeLinter.



**Linters e Formatadores**

Além dos editores de código, existem ferramentas específicas para linting e formatação. Prettier suporta várias linguagens como JavaScript, TypeScript, CSS, HTML e JSON, oferecendo formatação automática do código. ESLint é focado em JavaScript e TypeScript, garantindo conformidade com padrões de estilo específicos. Checkstyle é usado para Java, verificando a conformidade com padrões de estilo de código, incluindo a indentação. Clang-Format suporta C, C++, Java e JavaScript, proporcionando uma ferramenta de formatação configurável.

### 3.0 Comentários em Programação

#### 3.1 Conceito de Comentários

Comentários são trechos de texto adicionados ao código-fonte para fornecer explicações ou documentação sobre partes específicas do código. Eles não são executados pelo compilador ou interpretador e são destinados a serem lidos por desenvolvedores humanos para ajudá-los a entender o código.


- **Definição** 

Comentários no contexto do "Código Limpo" são usados para documentar o código, explicar decisões de design, fornecer informações sobre o propósito de variáveis, funções ou blocos de código, e para qualquer outro propósito que ajude na compreensão do que o código está fazendo.

#### 3.2 Exemplos de seu Propósito e sua Importância:

- Documentação do Código: Os comentários servem como uma forma de documentação que complementa o código. Eles explicam o porquê por trás das decisões tomadas no desenvolvimento do software.

- Facilitação do Entendimento: Ajudam os desenvolvedores a entenderem mais facilmente o que cada parte do código está fazendo, especialmente em áreas complexas ou que envolvem lógica complicada.

- Manutenção e Evolução: Comentários bem escritos facilitam a manutenção e a evolução do software ao longo do tempo, permitindo que novos desenvolvedores e membros da equipe compreendam rapidamente o que foi implementado e possam fazer modificações com segurança.

- Comunicação Efetiva: Permitem uma comunicação efetiva entre membros da equipe de desenvolvimento, transmitindo informações importantes que não são óbvias apenas pela leitura do código.

###### "Nada pode ser tão útil quanto um comentário bem colocado. Nada consegue amontoar um módulo mais do que comentários dogmáticos e supérfluos. Nada pode ser tão prejudicial quanto um velho comentário mal feito que dissemina mentiras e informações incorretas. - MARTIN, Robert."


#### 3.3 Tipos de Comentários

- Comentários de Linha
Os comentários de linha são breves e geralmente estão no mesmo nível de abstração do código que estão comentando. Eles são úteis para explicar partes específicas do código que podem não ser imediatamente óbvias.

- Os Comentários de bloco
Os comentários em blocos são utilizados para adicionar notas ou explicações que abrangem múltiplas linhas de código. Eles são úteis para descrever seções inteiras de código, fornecer informações detalhadas ou explicações mais longas que não cabem em um único comentário de linha. Em diferentes linguagens de programação, os comentários em blocos têm diferentes sintaxes.

- Comentários de Documentação
Os comentários de documentação são usados para gerar documentação automática a partir do código. Eles são formatados de uma maneira específica para serem processados por ferramentas como JavaDoc em Java ou docstrings em Python. Eles incluem informações sobre o propósito da classe, métodos, parâmetros, tipos de retorno e exceções lançadas.
Os comentários de documentação são mais formais e estruturados, seguindo convenções específicas da linguagem para que ferramentas de geração de documentação possam processá-los automaticamente e gerar documentação legível para nós humanos.

- *Exemplo de Tipos de Comentários*

**Exemplos:**

##### Exemplo em Python.

```python
# Este é um comentário de linha em Python
x = 10  # Atribui o valor 10 à variável x

# Este é um exemplo de comentário de bloco.
# Pode ser utilizado para explicar um trecho de código
# ou fornecer detalhes adicionais que não cabem em um comentário de linha.
# Cada linha do comentário de bloco começa com um símbolo de cerquilha.
```
###### Comentários de bloco são utilizados para adicionar explicações mais detalhadas que podem abranger várias linhas. Em Python, eles são criados utilizando # no início de cada linha do bloco de comentários.



##### Exemplo de Comentários de Documentação em Pyhon.

![Exemplo de DocString Python](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/6cf76a2d-2712-49d8-8697-6c382e868cf3)


###### *Comentários de documentação são utilizados para gerar documentação automática do código. Em Python, eles são chamados de docstrings e são criados utilizando três aspas duplas """.*


#### Exemplo em Java:

![Print JavaDoc](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/022ce400-e8ff-40d5-83df-7f100df5c0ec)


###### Para linguagens de programação, como Java, existem ferramentas como JavaDoc que utilizam comentários de documentação para gerar documentação do código.



#### 3.4 Boas Práticas de Comentários

- **Clareza e Concisão**

A clareza proporcionada pelos comentários permite que os desenvolvedores compreendam rapidamente o propósito de cada função, método ou algoritmo, economizando tempo e minimizando erros de interpretação.
Sempre que for ser utilizado os comentários devem ser claros e concisos. O objetivo é facilitar a compreensão do código, evitando ambiguidades e explicações prolixas. Bons comentários explicam o "porquê" de uma solução, especialmente em trechos complexos ou que envolvam decisões de design não óbvias.

###### "Códigos claros e expressivos com poucos comentários são de longe superiores a um amontoado e complexo com muitos comentários. Ao invés de gastar seu tempo criando comentários para explicar a bagunça que você fez, use-o para limpar essa zona. - MARTIN, Robert."

- **Relevância**

Um código bem comentado é mais claro e legível. Comentários ajudam a explicar a lógica por trás de um determinado trecho de código, detalhando a intenção do programador. Isso torna o código mais fácil de entender, mesmo para outros desenvolvedores que possam não estar familiarizados com a parte específica do sistema. Além do mais os Comentários explicam por que certas decisões de design foram tomadas, se esses comentários não são atualizados junto com as mudanças no código, o raciocínio original pode ser perdido, dificultando futuras refatorações ou depurações.

###### "O uso adequado de comentários é compensar nosso fracasso em nos expressar no código. Observe que usei a palavra fracasso. E é isso que eu quis dizer. Comentários são sempre fracassos. Devemos usá-los porque nem sempre encontramos uma forma de nos expressar sem eles, mas seu uso não é motivo para comemoração. - Martin, Robert​​."


- **Evitar Comentários Desnecessários**

Evite comentários que apenas repetem o que o código já está explicando. Comentários que descrevem o óbvio poluem o código e dificultam a manutenção.
De acordo com  Robert C. Martin escritor do livro Clean Code, "Comentários são desnecessários se o código está bem escrito. Clareza e legibilidade deve estar na linha de código e não nos comentários."

###### "Se nossas linguagens de programação fossem expressivas o suficiente ou se tivéssemos o talento para manipular com destreza tais linguagens de modo a expressar nossa intenção, não precisaríamos de muitos comentários. - Martin, Robert​​."​​.



- **Atualização dos Comentários**

Manter os comentários atualizados é crucial para a manutenção de um código saudável e compreensível. Comentários desatualizados podem ser mais prejudiciais do que a ausência de comentários, pois podem levar a deixar o código poluído e tendo mal-entendidos sobre o funcionamento atual do código. 

###### "Por que eu não gosto de comentários? Porque eles mentem. Nem sempre, e não intencionalmente, mas é muito comum. Quanto mais antigo um comentário for e quanto mais longe estiver do código o qual ele descreve, mais provável será que esteja errado.- Martin, Robert."

##### Aqui estão algumas razões específicas para a importância da atualização dos comentários:

**Evitar Desinformação:**

Comentários desatualizados podem fornecer informações incorretas sobre o que o código faz, levando a interpretações errôneas e potencialmente a erros ao modificar o código.

**Facilitar a Manutenção:**

Código bem comentado e atualizado é mais fácil de manter. Desenvolvedores que trabalham no código no futuro podem entender rapidamente a lógica e as intenções por trás das implementações.

**Auxiliar na Colaboração:**

Em projetos de equipe, comentários atualizados são essenciais para uma comunicação clara entre os membros da equipe. Eles ajudam a todos a entender o propósito e o funcionamento do código sem precisar decifrar a lógica por conta própria.


**Melhorar a Legibilidade:**

Comentários atualizados ajudam a manter o código legível e compreensível. Eles fornecem contexto e explicações para trechos complexos, tornando o código mais acessível a todos os desenvolvedores, independentemente de seu nível de familiaridade com a base de código.


#### 3.5 Comentários em Diferentes Linguagens

- *Exemplos de comentários em Java, C, C++:*

**Java**


![Print Comentário Java](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/d6f1eab0-520a-4aa0-bcf4-da4ebcd7220b)

**C/C++***


![Comentário em C](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/8f7793d3-7693-4037-9fc7-61ac5f6f49af)

**JavaScript**


![Print comentário JS](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/213389d7-51bf-4bc5-93bb-e482c72c1936)

###### *Para se ter práticas boas ao escrever seu código, é importante usar comentários eficazes para melhorar a compreensão e manutenção. Comentários de linha única são ideais para explicações rápidas e diretas. Para descrever seções maiores ou mais complexas do código, utilize comentários em bloco. É essencial que os comentários expliquem o "porquê" do código, fornecendo contexto e justificativa, em vez de apenas descrever o "o quê" está sendo feito, algo que geralmente já é evidente pelo próprio código. Evite comentários redundantes que apenas repetem o que o código já diz, pois isso não agrega valor e pode confundir quem lê.*

### 4.0 Explorando Ferramentas e Recursos em Comentários.

#### 4.1 Linters e Analisadores de Código

- **ESLint (JavaScript)**

O ESLint é uma ferramenta de linting para JavaScript que pode ser configurada para verificar não apenas o código, mas também a qualidade e consistência dos comentários.

As funcionalidades para Comentários do ESLint pode ser estendido com plugins e regras personalizadas para garantir que os comentários estejam formatados corretamente, usem linguagem clara e sigam convenções específicas.
Site - ESLint

- **Pylint (Python)**

O Pylint é um analisador de código estático para Python que não só verifica o código, mas também pode analisar a qualidade dos comentários e docstrings.

As funcionalidades para Comentários do Pylint inclui regras específicas para garantir que os comentários estejam presentes e sigam as convenções de documentação estabelecidas pela comunidade Python.
Site - Pylint

#### **Como Essas Ferramentas Funcionam?**

ESLint e Pylint são configurados através de arquivos de configuração onde você pode definir quais regras específicas deseja aplicar aos comentários em seu código.
Ambos os linters podem ser integrados em pipelines de CI/CD para garantir que padrões de comentários sejam mantidos ao longo do desenvolvimento.
Eles oferecem feedback imediato durante a escrita do código ou como parte do processo de revisão de código, ajudando a manter a qualidade e a consistência dos comentários em um projeto.

#### **Benefícios de Utilizar Linters para Comentários**

Padronização - Garantem que todos os desenvolvedores sigam as mesmas práticas de documentação.
Qualidade - Ajudam a melhorar a clareza e a precisão dos comentários, facilitando a compreensão do código.
Manutenção - Facilitam a manutenção do código ao garantir que informações relevantes estejam sempre documentadas de forma adequada.
Essas ferramentas são essenciais para equipes de desenvolvimento que buscam melhorar a qualidade do código, incluindo a documentação, ao longo do ciclo de vida do projeto.


#### 4.2 Geradores de Documentação

**JavaDoc**

JavaDoc é uma ferramenta padrão para a geração automática de documentação a partir de comentários no código-fonte Java. Ela é essencial para desenvolvedores Java que desejam criar documentação clara e consistente para suas classes, métodos, campos e outros elementos.


**Funcionalidades Principais:** Comentários Especiais: Utiliza comentários no estilo /** ... */ antes de classes, métodos, construtores e campos para extrair informações de documentação.


**Tags JavaDoc:** Usa tags especiais como @param, @return, @throws, entre outras, para descrever parâmetros, valores de retorno, exceções lançadas e outros detalhes relevantes.


**Geração de Documentação:** Produz documentação em formato HTML navegável, que inclui uma tabela de conteúdos, links cruzados entre classes e métodos, e referências úteis para facilitar a navegação.


**Integração com IDEs:** Muitos ambientes de desenvolvimento integrado (IDEs) para Java oferecem suporte nativo para JavaDoc, permitindo que os desenvolvedores visualizem e gerem a documentação diretamente na interface do usuário.


**Exemplo de uso:**


![9ad71034-7a80-4bfc-a6e3-8c5c31cde82e](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/5d2aa1b0-a7c7-40a2-ac43-ead50de8dfc7)

###### Neste exemplo, os comentários JavaDoc associados ao método soma descrevem os parâmetros (@param) e o valor de retorno (@return), que são então utilizados pelo JavaDoc para gerar documentação detalhada.

**Sphinx**

Sphinx é uma ferramenta flexível de documentação utilizada principalmente na comunidade Python. Ele permite a criação de documentação estruturada e esteticamente agradável a partir de docstrings no código-fonte, escritas em reStructuredText (reST).


**Funcionalidades Principais:** reStructuredText: Utiliza reST para escrever docstrings, que são então compiladas pelo Sphinx em diferentes formatos de saída, como HTML, PDF, ePub, entre outros.


**Temas e Personalização:** Oferece suporte a temas personalizáveis para estilizar a aparência da documentação gerada, garantindo uma apresentação profissional e consistente.


**Extensibilidade:** Pode ser estendido com plugins e extensões para adicionar funcionalidades adicionais, como integração com diagramas, testes de unidade, entre outros.


**Integração com Python:** Integrado com o ecossistema Python, Sphinx é amplamente adotado para documentar bibliotecas, frameworks e projetos Python de todos os tamanhos.

**Exemplo de uso:**


![526b3486-8dd2-40df-ba06-d41c44885a0e](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/5298b4d9-63e0-43e8-8731-146c5fe4fc30)

###### Neste exemplo, usando reStructuredText, descrevemos a função soma, incluindo detalhes sobre os parâmetros (:param) e o valor de retorno (:return). O Sphinx usa essas informações para gerar documentação estruturada e navegável.

**Após o estudo do nosso grupo recomendamos Tanto JavaDoc quanto Sphinx pois são ferramentas poderosas que automatizam o processo de documentação a partir de comentários no código-fonte. Elas são essenciais para manter a documentação consistente e de alta qualidade em projetos Java e Python, respectivamente, facilitando a compreensão e o uso do código por nós desenvolvedores.**


#### 4.3 Exemplos Práticos

- Códigos mal comentados: 

![d21446ce-6a69-4891-923f-5a807a2b50dc](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/6a779d49-da79-4be4-a809-f9c95ade0ddb)

###### Neste exemplo a cima o comentário está longe do código o qual descreve.


![99cb5d7f-490a-4cdd-85cb-5653fc57de63](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/2f08cc91-02cc-4973-8cef-11431ab48783)

###### Neste exemplo a cima existem muitos comentários o que deixa o código confuso.

- Códigos bem comentados:


![a9c16700-31eb-41bd-be91-b7dd1b7375f9](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/ca7d4df4-b334-41ed-b0ea-aafef9c2b985)

###### Neste exemplo a cima o comentário destaca a importância de algo que talvez pareça irrelevante, porém tem sua relevância e necessita ser comentado.


![c65d6349-c88d-4e96-8a1d-5d6686d747d5](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/d495abbf-4a47-4870-a4a5-697a179f76a7)

###### Já neste exemplo o comentário explica sobre a consequência que o desenvolvedor que executar este código irá gastar seu tempo e que possa não valer a pena, neste caso, explica porque um caso de teste em particular está desabilitado e serve de aviso.

*Livro: Clean Code*

#### 4.4 Refatoração

- Uma breve demonstração sobre refatoração de comentários em código.

**Antes da Refatoração**


![cb6888df-02c6-4db4-b617-e5218e035f4f](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/73822d5c-742a-4e61-8ee1-7f981f76900d)

**Depois da Refatoração**


![b94bf901-7e14-4766-902f-482c4d8c45f4](https://github.com/Riquelme213/Trabalho-Indentacao-e-Comentario/assets/172221396/64a73701-9e1c-4d00-9551-7a48a4d22701)

* Nesses dois exemplos podemos observar que o comentário acima (# imprime os detalhes) nos indica que a função imprime_divida faz mais do que uma tarefa só, por isso a refatoração é necessária.


### 5.0 Conclusão


#### 5.1  Resumo dos Pontos Principais

A indentação de código tem grande importância para a programação, pois organiza visualmente o código, tornando mais fácil para os desenvolvedores compreenderem a estrutura e a lógica do programa. Ela na maioria das linguagens de desenvolvimento é apenas uma questão de estética do código e existem várias ferramentas e recursos para ajudar a garantir uma indentação consistente em projetos de programação. Há boas práticas de indentação: Consistência e Espaços e Tabs (o tamanho do espaço é fixo e do tab pode variar). 

Os comentários também são muito importantes para o algoritmo, já que explicam partes específicas do código, tornando mais fácil para outros desenvolvedores entenderem a lógica e a finalidade de certas implementações, além de facilitar as revisões. Existem alguns tipos de comentários: os comentários de linha, os comentários de bloco e os comentários de documentação. Além disso, assim como na indentação, existem várias ferramentas e recursos para ajudar a manter a qualidade e a consistência dos comentários em um projeto e, existem boas práticas de comentários: Clareza e Concisão, Relevância, Evitar Comentários Desnecessários e Atualização dos Comentários.


#### 5.2 Livros para Sugestão:

- **"O livro Código Limpo: Habilidades Práticas do Agile Software - MARTIN, ROBERT."**

Este livro foca em práticas e princípios para escrever código limpo e de fácil manutenção. Ele cobre temas como a importância de nomes claros, simplicidade, refatoração, testes e boas práticas de design. Ideal para desenvolvedores que desejam melhorar a qualidade do seu código e seguir metodologias ágeis.

- **"Arquitetura Limpa: o Guia do Artesão Para Estrutura e Design de Software - MARTIN, ROBERT."**

Ele explora princípios de arquitetura de software, discutindo como estruturar sistemas de maneira que sejam robustos, escaláveis e de fácil manutenção. Aborda temas como a separação de preocupações, design orientado a componentes e padrões de arquitetura.


- **"Entendendo Algoritmos: Um Guia Ilustrado Para Programadores e Outros Curiosos - Aditya BhargavaAditya Bhargava"** 

Este livro oferece uma introdução acessível e visual aos algoritmos. Utilizando diagramas e ilustrações, explica conceitos complexos de maneira simples e prática, tornando-se uma excelente leitura para programadores iniciantes e curiosos que desejam compreender melhor como algoritmos funcionam e como aplicá-los em suas próprias soluções de software.

### 5.3 Recursos Adicionais

- [Documentação Oficial do Python](https://docs.python.org/3/)
- [Prettier](https://prettier.io/)
- [ESLint](https://eslint.org/)
- [Sphinx](https://www.sphinx-doc.org/)


## Equipe
- **Riquelme Ferreira** 
- **Sara Vitória** 
- **Vitor Emanuel** 
- **Miguel Gastaldi** 
- **Ana Julia** 
- **Vinicius Rosário** 
