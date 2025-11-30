# Prova

Hoje é o nosso ultimo dia de aula, e faremos hoje nossa prova.

# Pontuação

No total a prova vale 30 Pontos 

#### 15 dedicadas a codigos
#### 15 para perguntas de multipla escolha
#### 5 Pontos Extras, para questões de multipla escolha

## Atenção!

--------------------------------------------------------------------------------

Por conta de como o Forms é organizado, Na parte superior aparece Que o valor total é de 24 pontos.
A pontuação será da seguinte forma:

* Da 1° até a 5° Pergunta, cada uma vale 1 ponto
* A 6° e 7° pergunta, cada uma vale 2 pontos
* A 8° pergunta, cada resposta correta vale 0,5 pontos (totalizando 6 pontos totais disponiveis)
* 9° e 10 ° Pergunta (perguntas que valem os pontos extras), cada uma vale 2,5 pontos

* No total teremos 15 Pontos e 5 Pontos Extras Para perguntas de multiplas escolhas

------------------------------------------------------------------------

  A respeito das questões de código

  Teremos o total de 2 codigos, Ao final do questionario do forms, terão dois campos onde deverão ser escritos os dois ultimos códigos.


  ## Questão 1

  Temos Um Aplicativo de calculadora Capaz de fazer as seguinte Operações, Adição, Subtração, Multiplicação, Divisão, Elevevar um numero a outro, fazer a raiz quadrada desse número.

  Além disso, ele é capaz de fazer calculos de formas geiometricas, e retornar o perimetro e área dessa figura. Das figuras Geométricas em especifico, nós temos:

  * Retangulo/Quadrados
  * Circulos
  * Triangulos (assumindo um triangulo retangulo, aquele que possui um angulo de 90°)

O Cósigo atualmente se encontra totalmente modularizado, Porem, a lógica e os calculos estão inacabados.

Além disso, precisamos verificar se alguns números são válidos para determinadas operações, já que em determinados calculos como divisão de algum numero por 0, e calculo de formas gemoetricas não podem ter valores iguais ou abaixo de 0.

#### O que devemos fazer?

Complete todos os Metodos faltantes, de acordo com o que o Exercício pede.

#### ALgumas regras

Na divisão, o divisor não pode ser igual a 0. Na radiciação e nas figuras geometricas, nenhum valo pode ser menor ou igual a 0

---------------------------------------------------------------------------

#### Comandos e calculos importantes

 * comandos especificos
   
Math.Pow(x,y) - Faz o numero x elevado ao numero y


Math.Sqrt(x) - faz a raiz quadrada de x


Math.PI - Representa o numero PI 

* Formulas matemáticas:

Perimetro do retangulo/quadrado = (2 * comprimentos ) + (2 * altura)  (obs: como o quadrado possui lados iguais, seria 4 * lado)


Aréa do retangulo/quadrado = ( comprimento * altura ) (obs: como o quadrado possui lados iguais, seria lado * lado)


Perimetro do circulo = 2 * PI * Raio da circunferencia


Area do circulo = PI * Raio elevado a 2


Perimetro de um triangulo retangulo = base + altura +  diagonal. (para encontrar essa diagonal devemos usar o teorema de pitagoras, condierando base = b, altura = a e diagonal = g, a formula ficará assim: g elevado a 2 = b elevado a 2 + a elevado a 2. Após isso, para encontrar a diagonal, basta fazer a raiz de g elevado a 2)

Area do triangulo = (base 8 altura) / 2

Codigo: 

    using System;
    class program
    {
        
        public static void main()

        {
            double option = 0, resposta;
            do
            {
                Console.WriteLine("Escreva qual operação deseja fazer");
                Console.WriteLine("1 = Adição de dois numeros");
                Console.WriteLine("2 = Subtração de dois numeros");
                Console.WriteLine("3 = Multiplicação de dois numeros");
                Console.WriteLine("4 = Divisão de dois numeros");
                Console.WriteLine("5 = Primeiro numero elevado ao segundo");
                Console.WriteLine("6 = Raiz quadrada de um número");
                Console.WriteLine("7 = Perimetro e Area de um quadrado/retangulo");
                Console.WriteLine("8 = Perimetro e Area de um Circulo");
                Console.WriteLine("9 = Perimetro e Area de um Triangulo retangulo");
                Console.WriteLine("10 = Sair\n");
    
                option = double.Parse(Console.ReadLine());
    
    
                switch (option)
                {
                    case 1:
                        resposta = Adicao();
                        Console.WriteLine("A Soma final é de " + resposta);
                        break;
                    case 2:
                        resposta = Subratao();
                        Console.WriteLine("A Subtração final é de " + resposta);
                        break;
                    case 3:
                        resposta = Multiplicacao();
                        Console.WriteLine("A Multiplicação final é de " + resposta);
                        break;
                      case 4:
                        Divisao();
                        break;
                    case 5:
                        resposta = Potenciacao();
                        Console.WriteLine("A Potenciação final é de " + resposta);
                        break;
                    case 6:
                        Radiciacao();
                        break;
                    case 7:
                        retangulo();
                        break;
                    case 8:
                        Circulo();
                        break;
                    case 9:
                        Triangulo();
                        break;
                    case 10:
                        Console.WriteLine("Muito obrigado por sua atenção!");
                        break;
                    default:
                        Console.WriteLine("Escreva um número válido");
                        break;
                }


            } while (option != 10);
        }

        public double Adicao()
        {
            double x, y;
            Console.WriteLine("Escreva o primeiro numero");
            x = double.Parse(Console.ReadLine());
            Console.WriteLine("Escreva o segundo numero");
            y = double.Parse(Console.ReadLine());

            return/*Resposta*/;
        }
        public double Subratao()
        {
        double x, y;
        Console.WriteLine("Escreva o primeiro numero");
        x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva o segundo numero");
        y = double.Parse(Console.ReadLine());

        return/*Resposta*/;
        }
         public double Multiplicacao()
        {
        double x, y;
        Console.WriteLine("Escreva o primeiro numero");
        x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva o segundo numero");
        y = double.Parse(Console.ReadLine());

        return/*Resposta*/;
        }

        public static void Divisao()
        {
        double x, y;
        Console.WriteLine("Escreva o primeiro numero");
        x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva o segundo numero");
        y = double.Parse(Console.ReadLine());

        double resposta = /*resposta*/;



        if (/*Qual condição deve ser verdadeira?*/)
        {
            Console.WriteLine("A Divisão final é de" + resposta);
        }
        else
        {
            Console.WriteLine("Não é possivel dividir {0} por 0", x);
        }
        }

        public double Potenciacao()
        {
            double x, y;
        Console.WriteLine("Escreva o primeiro numero");
        x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva o segundo numero");
        y = double.Parse(Console.ReadLine());

            return/*Resposta*/;
        }

        public static void Radiciacao()
        {
        double x, y;
        Console.WriteLine("Escreva Um numero");
        x = double.Parse(Console.ReadLine());

        double resposta = /*Resposta*/;

        if (/*Qual condição deve ser verdadeira?*/)
        {
            Console.WriteLine("A Radiciacao final é de" + resposta);
        }
        else
        {
            Console.WriteLine("Não é possivel fazer a raiz de numeros menores ou igual a 0", x);
        }
        }

        public static void retangulo()
        {
        Console.WriteLine("Escreva o comprimento do retangulo");
        double x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva a altura do retangulo");
        double y = double.Parse(Console.ReadLine());

        if (/*Qual condição para que não seja correta?*/||/*Qual condição para que não seja correta?*/)
        {
            Console.WriteLine("Nem o comprimento nem a largura podem ser menor ou igual a 0");
        }
        else
        {
            Console.WriteLine("O perimetro do retangulo é " +/*Resposta*/);
            Console.WriteLine("A area do retangulo é " +/*Resposta*/);
        }
        }

        public static void Circulo()
        {
        Console.WriteLine("Escreva o Raio da circunferencia");
        double x = double.Parse(Console.ReadLine());


        if (/*Qual condição para que não seja correta?*/)
        {
            Console.WriteLine("O Raio da circunferencia pode ser menor ou igual a 0");
        }
        else
        {
            Console.WriteLine("O perimetro da circunferencia é " +/*Resposta*/);
            Console.WriteLine("A area da circunferencia é " +/*Resposta*/);
        }
        }

        public static void Triangulo()
        {
        Console.WriteLine("Escreva a base do triangulo");
        double x = double.Parse(Console.ReadLine());
        Console.WriteLine("Escreva a altura do triangulo");
        double y = double.Parse(Console.ReadLine());



        if (/*Qual condição para que não seja correta?*/||/*Qual condição para que não seja correta?*/)
        {
            Console.WriteLine("Nem a base nem a altura pode ser menor ou igual a 0");
        }
        else
        {
            double diagonal = /*resposta*/
            Console.WriteLine("O perimetro do triangulo é " +/*Resposta*/);
            Console.WriteLine("A area do triangulo é " +/*Resposta*/);
            }
        }
        }

  ## Questão 2

  




