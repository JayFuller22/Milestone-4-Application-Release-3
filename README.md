# Milestone-4-Application-Release-3
#include <stdio.h>
struct student {
    char name[60];
    int roll_no;
    float marks;
} sdt;
int main() {
    printf("Enter the following information:\n");
    printf("Enter student name: ");
    fgets(sdt.name, sizeof(sdt.name), stdin);
    printf("Enter student roll number: ");
    scanf_s("%d", &sdt.roll_no);
    printf("Enter students marks: ");
    scanf_s("%f", &sdt.marks);
    printf("The information you have entered is: \n");
    printf("Student name: ");
    printf("%s", sdt.name);
    printf("Student roll number: %d\n", sdt.roll_no);
    printf("Student marks: %.1f\n", sdt.marks);
    return 0;
}


#include <stdio.h>

union item
{
    int x;
    float y;
    char ch;
};

int main()
{
    union item it;
    it.x = 12;
    it.y = 20.2;
    it.ch = 'a';

    printf("%d\n", it.x);
    printf("%f\n", it.y);
    printf("%c\n", it.ch);

    return 0;
}
