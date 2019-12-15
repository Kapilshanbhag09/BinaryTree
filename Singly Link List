#include <stdio.h>
#include <stdlib.h>
struct node{
    int data;
    struct node *link;
};
int count;
struct node *first;
void insertb();
void inserte();
void display();
void deleteb();
void deletee();

int main(){
    int ch;
    printf("The menus are \n1.Insert At the beggining\n2.Insert at the end \n3.Display\n4.Delete at beginning\n5.Delete at end\n6.Exit\n");
    for(;;){
        printf("\nEnter the choice : ");
        scanf("%d",&ch);
        switch(ch){
            case 1:insertb();
                    break;
            case 2:inserte();
                    break;
            case 3:display();
                    break;
            case 4:deleteb();
                    break;
            case 5:deletee();
                    break;
            case 6:exit(0);
        }
    }
}
void insertb(){
    int ele;
    struct node *t;
    t=(struct node *)malloc(sizeof(struct node));
    printf("Enter the element to be inserted : ");
    scanf("%d",&ele);
    t->data=ele;
    t->link=NULL;
    if(first==NULL){
        first=t;
    }
    else{
        t->link=first;
        first=t;
    }
    count++;
}
void display(){
    struct node *t;
    printf("\nThere are %d elements they  are",count);
    t=first;
    while(t->link!=NULL){
        printf("\n%d",t->data);
        t=t->link;
    }
     printf("\n%d",t->data);
}
void inserte(){
    int ele;
    count++;
    struct node *t,*u;

    t=(struct node *)malloc(sizeof(struct node));
     printf("Enter the element to be inserted : ");

    scanf("%d",&ele);
    t->data=ele;
    t->link=NULL;
    if(first==NULL){
        first=t;
    }
    else{
        u=first;
        while(u->link!=NULL){
            u=u->link;
        }
        u->link=t;}

}


void deleteb(){
struct node *t;
   count--;
if(first==NULL){
    printf("The list is empty");
    }
    else{
        printf("\nThe deleted element is %d",first->data);
        t=first->link;
        free(first);
        first=t;


    }
}


void deletee(){
    struct node *t,*u;
    t=first;

if(t==NULL){
    printf("The list is empty");
    }
    else{

        while(t->link!=NULL){
            t=t->link;
            }
        u=t->link;
        t->link=NULL;
        printf("The deleted element is %d",u->data);




}
}
