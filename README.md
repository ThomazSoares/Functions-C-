# Functions-CPP

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
    
        return *vetor;
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
    
        return *vetor;
    }
}
