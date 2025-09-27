# attendance-management-system
#include<stdio.h>
void main(){
    char name[50];
    float percentage,total_classes,attended;
    printf("enter the name of the student:");
    scanf("%s",name);
    printf("enter total number of classes conducted:");
    scanf("%f",&total_classes);
    printf("enter total number of classes attended:");
    scanf("%f",&attended);
    percentage=(attended/total_classes)*100;
    printf("name of the student: %s\n",name);
    printf("total number of classes conducted:%f\n",total_classes);
    printf("total number of classes attended:%f\n",attended);
    printf("attendance percentage:%f\n",percentage);
    if(percentage>=90){
        printf("status: excellent");
    }
    else if(percentage>=75){
        printf("status: satisfactory");
    }
    else if(percentage>=50){
        printf("status: low");
    }
    else{
        printf("status: critical");
    }
}
