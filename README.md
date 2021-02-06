# studing-c


    #include <stdio.h>

    int main(void)
    {
        int column,line,n,i;

        printf("%3s", "");
        printf("%3s", "｜");
        for(column = 1; column <= 9; column++){
            printf("%3d", column);
        }
        putchar('\n');

        printf("%s", "---");
        printf("%3s", "＋");
        for(line = 1; line <= 9; line++){
            printf("%s", "---");
        }

        putchar('\n');

        for(i = 1; i <= 9; i ++){
            //"|"にも空白つけたい(文字制限つけると空白できるやつ)
            printf("%3d%3s", i, "｜");
            for (n = 1; n <= 9; n++)
            {
                printf("%3d", i * n);
            }
            putchar('\n');
        }

        return 0;
    }
