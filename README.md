int main(int argc, char const *argv[])
{
    float peso, altura, imc; 

    printf("Digite seu peso %f", peso);
    scanf("%f", &peso);

    printf("Digite sua altura %f", altura);
    scanf("%f", &altura);

    imc = peso / (altura * altura);

    printf("seu IMC e: %2.f\n", imc);


    if (imc <18.5) {
        printf("classificado abaixo do peso\n");
    } else if (imc >= 18.5 && imc < 24.9){
        printf("classificado peso normal\n");
    } else if (imc >= 25 && imc < 29.9){
        printf("classificado: Sobrepeso\n");
    } else if (imc >= 30 && imc < 34.9) {
        printf("classificado: Obesidade grau I\n");
    } else if (imc >= 35 && imc < 39.9) {
        printf("classificado: Obesidade grau II\n");
    } else {
        printf("classificado: Obesidade grau III (mórbida)\n");
    }
      
    
      return 0;
      
}