# include <stdio.h>
# include <stdlib.h>
# include <time.h>

int main()
{
int numbers_needed;
int max_range;
int bonus_ans;
int again_ans;
int bonus_range;
int lottery_numbers[100];
int bonus_number[100];
int i;
int j=0;
int temp;
int random_1;
int random_2;
srand(time(NULL));

printf("****************************************************\n");
printf("*$$$$$$$$$$$$$$$$$$$ THE AMAZING $$$$$$$$$$$$$$$$$$*\n");
printf("*$$$$$$$$$$$$$$$$$ LOTTERY NUMBER $$$$$$$$$$$$$$$$$*\n");
printf("*$$$$$$$$$$$$$$$$$$$ GENERATOR $$$$$$$$$$$$$$$$$$$$*\n");
printf("****************************************************\n");
printf("     How Many Numbers do you need to choose?:");
scanf("                      %d", &numbers_needed);
printf("           What is the range? 1 to ");
scanf("                      %d", &max_range);
printf("  Is there a bonus number drawn? 1 for YES, 2 for NO : ");
scanf("                      %d", &bonus_ans);

if (bonus_ans==1)
{
printf("         What is the range for the bonus#? 1 to ");
scanf("                       %d", &bonus_range);
}

while (j==0){
for (i=1; i<=max_range; i++)
{
lottery_numbers[i]=i;
}

for (i=1; i<=max_range*2; i++)
{ 
random_1= 1+ rand () % (max_range);
random_2= 1+ rand () % (max_range);   
temp=lottery_numbers[random_1];   
lottery_numbers[random_1]=lottery_numbers[random_2];   
lottery_numbers[random_2]=temp;
}

printf("Your lottery Numbers are: ");

for (i=1; i<=numbers_needed; i++)
{  
printf("%d ", lottery_numbers[i]);
}

printf("\n");

if (bonus_ans==1)
{    
  for (i=1; i<=bonus_range; i++)
  {    
  bonus_number[i]=i;
  }
  for (i=1; i<=bonus_range*2; i++)
  {    
  random_1=1+ rand () % (bonus_range);    
  random_2=1+ rand () % (bonus_range);   
  temp=bonus_number[random_1];    
  bonus_number[random_1]=bonus_number[random_2];   
  bonus_number[random_2]=temp;
  }    
  printf("Your Bonus number is: %d \n", bonus_number[3]);
  }
 
printf("Are you okay with these numbers? 0 for Yes, 1 for NO: ");
scanf("%d", &again_ans);

if (again_ans==0)
{
j++;
}
} 
printf("Good Luck");     
return 0;
}
