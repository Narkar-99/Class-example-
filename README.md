# Class-example-


#include<iostream>
using namespace std;
/// choose proper keywords to express the info 
class person {
private:
    int salary;
public:
    char gender;
    long mobile;

    void privateinfo(int salary1);
    void publicinfo()
    {
        cout <<"\nGender of employee:"<<gender;
        cout <<"\nMobile number of employee:"<<mobile;
        cout <<"\nSalary of the employee:"<<salary;
    }
};
void person:: privateinfo(int salary1)
{
    salary=salary1;

}



int main()
// change person name
    person fazal;

    fazal.gender='M';
    fazal.mobile=8999635381;
//private variable can be accessed through below function
    fazal.privateinfo(100000);
    fazal.publicinfo();


    return 0;
}
