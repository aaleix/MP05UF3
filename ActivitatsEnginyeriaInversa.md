# Enginyeria inversa (Activitats per parelles)

De vegades ens tocarà copiar el comportament d'un programa només visualitzant-lo, això és el que s'anomena enginyeria inversa.

## Activitats 

### Calculadora

Tenim el següent codi:

```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Double operand1, operand2;
        int operacio;
        Calculadora calc = new Calculadora();
        while (true){
            try {
                System.out.println("Introdueix el primer número: ");
                operand1 = sc.nextDouble();
                System.out.println("Introdueix el segon número: ");
                operand2 = sc.nextDouble();
                System.out.println("Quina operació vols realitzar? ");
                System.out.println("1. suma");
                System.out.println("2. resta");
                System.out.println("3. multiplicació");
                System.out.println("4. divisió");
                operacio = sc.nextInt();
                switch (operacio) {
                    case 1:
                        System.out.println("El resultat és: " + calc.suma(operand1, operand2));
                        break;
                    case 2:
                        System.out.println("El resultat és: " + calc.resta(operand1, operand2));
                        break;
                    case 3:
                        System.out.println("El resultat és: " + calc.multiplicacio(operand1, operand2));
                        break;
                    case 4:
                        System.out.println("El resultat és: " + calc.divisio(operand1, operand2));
                        break;
                }
            }
            catch (Exception e){
                System.out.println("Error!\n");
                sc = new Scanner(System.in);
            }
        }
    }
}
```

Sense coneixer la classe Calculadora ens demanen fer un treball de documentació dels següents passos (link a un repositori públic de github on ho expliqueu):

1. Crear la classe Calculadora a Umbrello. ![image](https://user-images.githubusercontent.com/113586080/234492319-312f7bba-38cf-4b34-bba0-306ea54ee750.png)

2. A Umbrello afegir el codi de tots els mètodes de la classe Calculadora.

![image](https://user-images.githubusercontent.com/113586080/234495017-44bf3a17-1fc5-4a6c-8be2-7618de17f49c.png)

He fet el mateix amb els altres mètodes.

3. Importar a Umbrello la classe Main (mitjançant assistent d'importació).
4. Exportar el codi del projecte a JAVA i a Python.
5. Es pot utilitzar directament el codi generat a JAVA?
   
   Sí. 
   
   ![image](https://user-images.githubusercontent.com/113586080/234494739-9d8c4724-30ce-4efd-be37-24fe67990e15.png)


### Batalles 

Hem vist un joc que està fent l'alumnat de 2n de DAM amb les tecnologies Python + Flask.

És tracta d'un joc de batalles per torns on 2 personatges generats aleatòriament s'enfronten entre ells.

![image](https://user-images.githubusercontent.com/110727546/234293601-609310d0-8986-4d37-be2c-c96227eca9d2.png)

Per accedir al joc haureu d'escriure al navegador [192.168.204.100:5000](http://192.168.204.100:5000)

**Es demana:**

Utilitzeu el programa i penseu com deu funcionar.

Ens demanen fer un treball de documentació dels següents passos (link a un repositori públic de github on ho expliqueu):

1. Fer un diagrama de classes de la classe Personatge amb els seus atributs i mètodes a Umbrello.
2. Exportar el diagrama a codi Python des d'Umbrello.
3. Fer el diagrama de casos d'ús que penseu que tindria el joc (a Umbrello o Lucid).
4. Fer el diagrama de seqüència total o d'algun cas d'ús específic que penseu que tindria el joc (a Umbrello o Lucid).
