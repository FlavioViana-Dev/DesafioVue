# Calculadora de números de dados

Você receberá três valores diferentes como parâmetros, cada valor representa um único número de dados. Seu objetivo é calcular o resultado final para este jogo de dados.

Se receber três dados com o mesmo número, deve devolver o número multiplicado por 3. Se o resultado for dois números iguais, deve devolver o número multiplicado por 2. Se não houver números iguais, deve devolver o maior deles .

### Entrada e saída

Com base na explicação acima, você receberá entradas como os exemplos abaixo:

```
Exemplo 1:
- Dados 1: 1
- Dados 2: 2
- Dados 3: 3

Exemplo 2:
- Dados 1: 4
- Dados 2: 1
- Dados 3: 4

Exemplo 3:
- Dados 1: 3
- Dados 2: 3
- Dados 3: 3
```

Com base nos exemplos acima, você deve retornar o valor que representa o valor numérico correto.

```
Exemplo 1: 3
Exemplo 2: 8
Exemplo 3: 9
```

O exemplo 1 retornará 3 porque não há números iguais e 3 é o maior valor. No exemplo 2 retornará 8, pois são dois dados iguais. E o último exemplo retornará 9, porque são três dados iguais.

Nota: Deve-se ter cuidado com os números fora de um intervalo de dados (que é de 1 a 6).
