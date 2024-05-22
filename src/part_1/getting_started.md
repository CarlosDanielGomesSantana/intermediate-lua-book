# Começando

## Primeiros Passos
Tradicionalmente, o programadores ao iniciar os estudos de uma nova linguagem. Criam um primeiro programa com a menssagem 'Olá Mundo!'

```Lua
print('Olá Mundo!')
```

Se você estiver usando o Interpretador Lua, é necessário chamá-lo para executar o seu primeiro programa em Lua. Salve o arquivo com o nome `hello.lua` e, em seguida, execute o seguinte comando:

```text
$ lua hello.lua
```

Mas, podemos se quisermos executar um código mais complexo como um programa que pega número passado pelo usuário e dar a posição do mesmo na [Sequência de Fibonacci](https://pt.wikipedia.org/wiki/Sequ%C3%AAncia_de_Fibonacci):

```Lua
-- Entrega um número da Sequência de Fibonacci 
function fibonacci(n)
    if n == 0 then
        return 0
    elseif n == 1 then
        return 1
    else
        return fibonacci(n - 1) + fibonacci(n - 2)
    end
end

print('Digite um número:')
numero = io.read("*n") -- lê um Número (Number)
print(fibonacci(numero))
```
