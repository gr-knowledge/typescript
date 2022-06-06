# Classe

A ClasseA depende da ClasseB

```TS
class NomeClasse
{
private string atributoA;
public int atributoB;
private function metodo1(): string
{
//corpo do método
}
protected function metodo2(): int
{
//corpo do método
}
public static function metodo3(): void
{
//corpo do método
}
}
```
*Métodos estáticos podem ser invocados sem que exista um objeto da classe*

# Classe Abstrata

A ClasseA depende da ClasseB

```TS
abstract class NomeClasse
{
private string atributoA;
public int atributoB;
private function metodo1(): string
{
//corpo do método
}
protected function metodo2(): int
{
//corpo do método
}
public function metodo3(): void
{
//corpo do método
}
}

```

*Não pode ser instanciada*
*Não gera objetos*
*O nome da classe no diagrama fica em itálico*

# Interfaces

A ClasseA depende da ClasseB

```TS
interface NomeInterface
{
private function metodo1(): string;
protected function metodo2(): int;
public function metodo3(): void;
}
```

*As classes que implementam uma interface devem implementar todos os métodos definidos nela*

# Relacionamentos

![image](https://user-images.githubusercontent.com/10155481/172225916-43a2deb3-7cd6-4925-b07c-0a2efb21e997.png)

## Associação
![image](https://user-images.githubusercontent.com/10155481/172227803-795441a2-e0be-4cef-9511-66d7587ca5f4.png)

A ClasseA depende da ClasseB

```TS
class ClasseA
{
//Início do corpo da classe
...
variavel = new classeB();
...
//Fim do corpo da classe
}
```

*A ClasseA depende da ClasseB*

## Generalização
![image](https://user-images.githubusercontent.com/10155481/172227860-9b4efbd3-d6b3-4285-bdbe-2c1df5fcf893.png)

A ClasseA depende da ClasseB

```TS
class ClasseA
{
//Início do corpo da classe
...
variavel = new classeB();
...
//Fim do corpo da classe
}
```

*A ClasseA herda a ClasseB*
*A ClasseA é uma subclasse da ClasseB*

## Realização
![image](https://user-images.githubusercontent.com/10155481/172227885-65012b4c-acb4-4b2f-a8c2-fd8c36df9d50.png)

A ClasseA depende da ClasseB

```TS
class ClasseA
{
//Início do corpo da classe
...
variavel = new classeB();
...
//Fim do corpo da classe
}
```

*A ClasseA implementa a Interface*

## Agregação
![image](https://user-images.githubusercontent.com/10155481/172227936-8e532a3b-918b-4f38-b2db-fef0f677928f.png)

A ClasseA depende da ClasseB

```TS
class ClasseA
{
//Início do corpo da classe
...
variavel = new classeB();
...
//Fim do corpo da classe
}
```

*O objeto da ClasseB é utilizado/faz parte da ClasseA*
*A ClasseA não é fortemente ligada a ClasseB (podem existir separadamente)*

## Composição
![image](https://user-images.githubusercontent.com/10155481/172227969-9c898b2e-ae4f-4e47-8cc7-13d8b4848873.png)

A ClasseA depende da ClasseB

```TS
class ClasseA
{
//Início do corpo da classe
...
variavel = new classeB();
...
//Fim do corpo da classe
}
```

*O objeto da ClasseB é utilizado/faz parte da ClasseA*
*Quando a ClasseA deixar de existir a ClasseB também deixará de existir*
