# readability1

int l= 0; 
int w=1;  
int f=0;  
while(S[l]!='\0')
    {
        if(S[l]=='.' || S[l]=='\n'  || S[l]=='\0' || S[l]==' ')

        {
            w++;
            f++;
        }

        l++;
    
    }

 int grade = 0.0588 * (100 * l / w) - 0.296 * (100 * f / w) - 15.8;

    printf("Letters: %i\n Words: %i\n Sentences: %i\n", l, w, f);

 if (grade <= 1)
    {
        printf("Before Grade 1\n");
    }
    else if (grade < 16)
    {
        printf("Grade %i\n", grade);
    }
    else
    {
        printf("Grade 16+\n");
    }




}
