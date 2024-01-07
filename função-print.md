# Função print, type e help
Nesta aula, o professor abordou a instalação do Python 3 e a função print. Ele explicou como utilizar a função `help()`para obter informações sobre outras funções, como a função print. A função print é utilizada para imprimir mensagens na tela e pode receber três valores: ***value, sep e end***. O professor mostrou exemplos de como utilizar a função print com diferentes valores para ***value, sep e end***. Em seguida, ele introduziu o conceito de variáveis e mostrou como definir e utilizar variáveis no lugar dos valores antigos na função print. Ele também explicou que o tipo de uma variável depende do valor que é atribuído a ela e utilizou a função `type()` para verificar o tipo das variáveis. No próximo vídeo, será abordado com mais detalhes sobre os tipos de variáveis.

## Exemplo ( print() )
```python
print("Olá mundo")
```
resultado: Olá mundo

## Exemplo ( type() )
``` python
pais = "Brasil"
quantidade = 4

type(pais)
type(quantidade)
```

resultado:
```python
 <class 'str'>
<class 'int' >
```

# Exemplo ( help() )
```python
help()

 um novo console aparece:
help>

Agora, como queremos saber mais sobre a função print, vamos digitá-la:
help(print)

resultado:
print(*args, sep=' ', end='\n', file=None, flush=False)
    Prints the values to a stream, or to sys.stdout by default.

    sep
      string inserted between values, default a space.
    end
      string appended after the last value, default a newline.
    file
      a file-like object (stream); defaults to the current sys.stdout.
    flush
      whether to forcibly flush the stream.
```

Inicialmente, o que nos importa são os três primeiros valores que a função print pode receber:

***value*** é o valor que queremos imprimir, as reticências indicam que a função pode receber mais de um valor, basta separá-los por vírgula.
***sep*** é o separador entre os valores, por padrão o separador é um espaço em branco.
***end*** é o que acontecerá ao final da função, por padrão há uma quebra de linha, uma nova linha (\n).


