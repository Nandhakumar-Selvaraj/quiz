#include <stdio.h>

int main() {
    int choice, answer, score = 0;

    while (1) {
        printf("\n--- Welcome To Quiz Game ---\n");
        printf("1. Instruction\n");
        printf("2. Start Quiz\n");
        printf("3. View Score\n");
        printf("4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        if (choice == 4) {
            printf("Exiting the game. Goodbye!\n");
            break;
        }

        switch (choice) {
            case 1:
             printf("---INSTRUCTION---\n");
               printf("step 1: Enter into the game\n");
               printf("step 2: Start the quiz\n");
               printf("step 3: It have 4 questions\n");
               printf("step 4: Read the questions and answer correctly\n");
               printf("step 5: Then choose veiw score to see the score\n");
               printf("step 6: If the score is below 2 then try again\n");
               break;
            case 2:
             score = 0;

                // Question 1
                printf("\nQ1. What is the capital of india?\n");
                printf("1. Chennai\n2. Delhi\n3. Mumbai\n4. Trichy\n");
                printf("Enter your answer: ");
                scanf("%d", &answer);
                if (answer == 2) {
                    printf("correct!\n");
                    score++;
                }else{
                    printf("Wrong!The correct answer is delhi.\n");
                }
            

                // Question 2
                printf("\nQ2. Which planet is known as the Red Planet?\n");
                printf("1. Earth\n2. Mars\n3. Jupiter\n4. Saturn\n");
                printf("Enter your answer: ");
                scanf("%d", &answer);
                if (answer == 2) {
                    printf("correct!\n");
                    score++;
                }else{
                    printf("Wrong!The correct answer is Mars\n");
                }
                
                // Question 3
                printf("\nQ3. Who is the Father of Our Nation?\n");
                printf("1. Mahatma Gandhi\n2. William Shakespeare\n3. Nehru\n4. Leo Tolstoy\n");
                printf("Enter your answer:");
                scanf("%d", &answer);
                if (answer == 1) {
                    printf("correct!\n");
                    score++;
                }else{
                    printf("Wrong!The correct answer is Mahatma Gandhi\n");
                }
                
                // Question 4
                 printf("\nQ3. Who wrote Thirukural?\n");
                 printf("1. Nehru\n2. Bharathiyar\n3. Kambar\n4. Thiruvalluvar\n");
                 printf("Enter your answer:");
                scanf("%d", &answer);
                if (answer == 4) {
                    printf("correct!\n");
                    score++;
                }else{
                    printf("Wrong!The correct answer is Thiruvalluvar\n");
                }
                printf("\nQuiz completed!\n");
                break;
              
                
            case 3:
                printf("\nYour current score is: %d out of 4\n", score);
                if(score == 4){
                    printf("Excellent!\n");
                } else 
                     if(score == 3){
                         printf("Very Good!\n");
                     }else
                        if(score == 2){
                            printf("Good job!\n");
                        } else{
                            printf("Try again!\n");
                        }
                        
            break;
        }
    }

    return 0;
}
