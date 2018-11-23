//
//  main.c
//  CProgramming
//
//  Created by Levi on 11/22/18.
//  Copyright © 2018 Levi. All rights reserved.
//

#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>
#include <string.h>
#include <math.h>

int main(int argc, char *argv[]) {
    
    int end;
    char guess;
    int roll1, roll2, roll3, roll4, sum;
    char enter1;
    char enter2;
    char enter3;

    do {
        puts("Press 1 to start the game or 0 to end");
        scanf("%d", &end);
        
        if(end != 0) {
            puts("Rolling 1");
            roll1 = (rand()%6+1);
            puts("1/3 rolled\nPress 1 to continue");
//            printf("%d\n",roll1);
            scanf(" %s", &enter1);
            
            puts("Rolling 2;");
            roll2 = (rand()%6+1);
            puts("2/3 rolled\nPress 1 to continue");
//            printf("%d\n",roll2);
            scanf(" %s", &enter2);
            
            puts("Rolling 3;");
            roll3 = (rand()%6+1);
            puts("3/3 rolled\nPress 1 to continue");
//            printf("%d\n",roll3);
            scanf(" %s", &enter3);
            
            sum = roll1 + roll2 + roll3;
           
            //Test the sum
//            printf("The sum of all three rolls is: %d\n",sum);
            
            puts("Time to guess: Would the next roll be higher or a lower than your sum?\n[type 'h' if higher or 'l' if lower]");
            scanf(" %c0",&guess);
            
            puts("Here you go! Final roll!");
            
            roll4 = (rand()%6+1);
            
            if((roll4 > sum) && (guess == 'h')) {
                printf("Yes!! You win!\nThe sum of the first three rolls is %d, and your guess is higher [%d] than the sum\n", sum, roll4);
                
            }
            else if((roll4 < sum) && (guess == 'h')) {
                
                printf("No, try again. The sum of the first three rolls is %d, and your guess is lower [%d] than the sum\n", sum, roll4);
            }
            else if((roll4 < sum) && (guess == 'l')) {
                
                printf("Yes!! You win!\nThe sum of the first three rolls is %d, and your guess is lower [%d] than the sum\n", sum, roll4);
            }
            else if((roll4 > sum) && (guess == 'l')) {
                
                printf("No, try again. The sum of the first three rolls is %d, and your guess is higher [%d] than the sum\n", sum, roll4);
            }
            
        }
        else {
            break;
        }
       
        
    }
    while(end!=0);
    
    puts("Thank you for playing the game");
    
}



        
