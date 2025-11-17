# employee-database
medical camp

#include <stdio.h>
struct employee{
    int ID;
    int age;
    int workyear;
    
};
int main() {
    int i, ID, workyear;
    struct employee emp[3];
    for (int i=1; i<4; i++){
        printf(" enter ID:");
        scanf("%d", &emp[i].ID);
        printf("enter age:");
        scanf("%d",&emp[i].age);
        printf("enter workyear:");
        scanf("%d",&emp[i].workyear);
        }
    for(i=1; i<4; i++){
        if(emp[i].age==27 && emp[i].workyear>=1){
            printf("ID %d selected for medical camp\n",emp[i].ID);
        }
        else{
            printf("ID %d not selected for medical camp\n", emp[i].ID);
        }
    }

    return 0;
}
