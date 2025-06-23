# Problema 1 — ArrayDifferenza

Implemente o método:

```
public static int[] diff(int[] a, int[] b)
```

O método deve retornar um array contendo todos e somente os elementos do array `a` que não estão presentes no array `b`. Considere que o método sempre será chamado com argumentos diferentes de `null`.

---

# Problema 2 — ComparaSequenze

Implemente a classe `ComparaSequenze`, que deve realizar as seguintes operações:

- Ler da entrada padrão uma sequência **A** de números reais, inseridos um após o outro (a inserção termina quando o número 0 é inserido).
- Ler da entrada padrão uma sequência **B** de frações (instâncias da classe `Fraction`, que disponibiliza métodos como `isLesser()`, `isGreater()`, `getNumerator()`, `getDenominator()`, etc.), inseridas uma após a outra (a inserção termina quando uma fração menor que 0 é inserida).
- Imprimir na saída padrão as frações de **B** que sejam maiores que pelo menos a metade dos números reais presentes na sequência **A**.

Se ao menos uma das duas sequências estiver vazia, a execução deve ser interrompida e uma mensagem apropriada de erro deve ser impressa na saída padrão.

---

# Problema 3 — MatriceStringa

Considere a classe `MatriceStringa` com a seguinte estrutura:

```java
public class MatriceStringa {
    private String[][] m;
    // ...
}
```

- Implemente o construtor da classe com a seguinte assinatura:

  ```java
  public MatriceStringa(int r, int c, String val)
  ```

  O construtor deve inicializar o campo `m` com uma matriz de `r` linhas e `c` colunas, onde cada posição contém o valor `val`. O construtor deve lançar uma exceção do tipo `RuntimeException` se os valores de `r` e `c` não forem válidos (utilize o construtor sem argumentos da classe `RuntimeException`).

- Implemente o método da classe com a seguinte assinatura:

  ```java
  public void set(int r, int c, String val) throws MatriceException
  ```

  O método deve atribuir, na posição de linha `r` e coluna `c` da matriz `m`, o valor `val`. O método deve lançar a exceção não-verificada `MatriceException` se os valores de `r` e `c` estiverem fora dos limites válidos (utilize o construtor sem argumentos para criar a exceção).

- Implemente o método da classe com a seguinte assinatura:

  ```java
  public String rigaToString(int idx, String separatore) throws MatriceException
  ```

  Este método deve retornar uma string obtida pela concatenação das strings que aparecem na linha de índice `idx` da matriz `m`, separadas pela string fornecida como separador. O método lança a exceção não-verificada `MatriceException` se o índice `idx` não corresponder a uma linha válida da matriz ou se o separador for `null`.

---

# Problema 4 — Sorteador de Prêmios para Eventos

Você foi contratado para desenvolver um aplicativo de sorteios personalizados que será utilizado em festas e eventos para distribuir prêmios entre os convidados. O aplicativo precisa ser simples, intuitivo e funcional, com a possibilidade de ser reutilizado em diferentes ocasiões.

- Permitir o cadastro de ao menos dois prêmios que serão sorteados (ex.: "Camisa", "Caneca");
- Permitir o cadastro de ao menos cinco nomes de participantes que concorrerão ao sorteio;
- Realizar dois sorteios consecutivos:
  - O primeiro prêmio deve ser sorteado entre todos os participantes;
  - O segundo prêmio deve ser sorteado excluindo o ganhador do primeiro;
- Exibir na tela:
  - O nome do prêmio sorteado;
  - O nome do ganhador correspondente;
- Exibir uma imagem de logotipo (pode ser genérica);
- Apresentar um botão para iniciar o sorteio após o preenchimento dos dados;
- Implementar o sorteio utilizando algoritmo baseado em `Math.random()`, garantindo imparcialidade e aleatoriedade.

---

# Problema 5 (Versão Explicativa) — Sorteador de Prêmios para Eventos

Implemente uma função em Python responsável por simular um sorteador de prêmios utilizado em eventos. A função deve seguir os seguintes passos:

- Receber como entrada uma lista com ao menos dois prêmios, por exemplo: `["Camisa", "Caneca"]`;
- Receber como entrada uma lista com pelo menos cinco nomes de participantes;
- Sortear o primeiro prêmio aleatoriamente entre todos os participantes;
- Sortear o segundo prêmio, garantindo que o ganhador do primeiro prêmio seja excluído do segundo sorteio;
- Exibir para cada sorteio:
  - O nome do prêmio sorteado;
  - O nome do ganhador correspondente;
- Exibir um logotipo representado por texto (ex.: `[LOGO DO EVENTO]`), já que não há interface gráfica;
- A lógica de sorteio deve utilizar funções da biblioteca `random`, como `random.choice` ou `random.shuffle`, assegurando a aleatoriedade e imparcialidade da seleção.

A função deve ser clara, organizada em blocos funcionais e permitir fácil modificação das listas de entrada. O resultado deve ser exibido diretamente no console.

```python
def sortear_premios(premios: list[str], participantes: list[str]) -> None:
    # implementação aqui
```
