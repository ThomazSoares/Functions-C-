# Functions-CPP

**Note: for any"is_[...]" returns a boolean value**

{

    int decrescent(int *vetor, int vSize){
        int x;
      
        for (int i=0; i<vSize - 1; i++){
            for (int j=0; j<vSize - 1; j++){
                if (vetor[j] < vetor[j+1]){
                    x = vetor[j];
                    vetor[j] = vetor[j+1];
                    vetor[j+1] = x;
                }
            }
        }
    
        return (*vetor);
    }
}
{

    int crescent(int *vetor, int vSize){
        int x;
    
        for (int i=0; i<vSize - 1; i++){
            for (int j=0; j<vSize - 1; j++){
                if (vetor[j] > vetor[j+1]){
                    x = vetor[j];
                    vetor[j] = vetor[j+1];
                    vetor[j+1] = x;
                }
            }
        }
    
        return (*vetor);
    }
}
{

    int is_prime(int num){
        int cond = 1;
    
        if (num == 0 || num == 1 || (num != 2 && num % 2 == 0)){
            cond = 0;
        } else{
            for (int i=3; i<(num/2) + 1; i++){
                if (num % i == 0){
                    cond = 0;
                    break;
                }
            }
        }
    
        return (cond);
    }
}
