#include <stdio.h>

int main()
{
    int n, i;
    int process[10], burstTime[10];

    printf("Enter the number of processes: ");
    scanf("%d", &n);

    // Input process IDs and burst times
    for(i = 0; i < n; i++)
    {
        process[i] = i + 1;
        printf("Enter Burst Time for Process P%d: ", process[i]);
        scanf("%d", &burstTime[i]);
    }

    printf("\nExecution Order:\n");

    // Simulate scheduler
    for(i = 0; i < n; i++)
    {
        printf("Executing Process P%d (Burst Time = %d)\n",
               process[i], burstTime[i]);
    }

    printf("\nAll processes executed successfully.\n");

    return 0;
}
