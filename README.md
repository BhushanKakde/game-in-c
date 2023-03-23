# game-in-c
the game is going to fun how can we guess no,
#include<stdio.h>
#include<stdlib.h>
#include<time.h>
int main(){
    int number,guess,nguesses=1;
    srand(time(0));
    number=rand()%100+1;
    do{
        printf("guess the number between 1 to 100 \n");
        scanf("%d",&guess);
        if(guess>number){
            printf("lowe number plz\n");

        }

        else if(guess<number){
            printf("bigger number plz\n");
        }
        else{
            printf("your guessed it in %d attempts\n",nguesses);

        }
        nguesses++;

    } while (guess!=number);
    return 0;
    


}
