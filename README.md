#include <stdio.h>
#include <stdlib.h>

void nhapmang (int a[][10], int n, int m)
{
    int i,j;
    for (i=0; i < n; i++)
    {
        for (j=0; j<m; j++)
            {
                printf ("a[%d][%d]= ", i+1, j+1);
                scanf ("%d", &a[i][j]);
            }
    }
}

void xuatmang (int a[][10], int n, int m)
{
    int i,j;
    printf ("mang da nhap la:\n");
    for ( i=0; i<n; i++)
    {
        for ( j=0; j<m; j++)
            {
                printf ("%3d ", a[i][j]);
            }
        printf ("\n");
    }
}
int main()
{
    int m,n;
    int a[10][10];
    printf ("nhap so dong va so cot: ");
    scanf ("%d%d", &m, &n );
    nhapmang (a,m,n);
    xuatmang (a,m,n);
    return 0;
}
