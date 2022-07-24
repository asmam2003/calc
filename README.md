#include <iostream>

using namespace std;
float a, b;
int c;
char d;

float addition (float a, float b)
{
    cout << "Enter your two numbers" << endl;
    cin >> a >> b;
    float answer = a + b;
    return answer;
}

float subtraction (float a, float b)
{
    cout << "Enter your two numbers" << endl;
    cin >> a >> b;
    float answer = a-b;
    return answer;
}

float division (float a, float b)
{
    cout << "Enter your two numbers" << endl;
    cin >> a >> b;
    float answer = a/b;
    return answer;
}

float multiplication (float a, float b)
{
    cout << "Enter your two numbers" << endl;
    cin >> a >> b;
    float answer = a*b;
    return answer;
}

int mod (int a, int b)
{
    cout << "Enter your two numbers" << endl;
    cin >> a >> b;
    int answer = a%b;
    return answer;
}

void calc () {
    cout << "what operation do you want" << endl;
    cin >> c;
    if (c==1) {
    cout << addition (a,b)<< endl;
    
        if (c==2)
        cout << subtraction (a,b) << endl;
        
        if (c==3)
        cout << division (a,b) << endl;
        
        if (c==4)
            cout << multiplication (a,b) << endl;
        
        if (c==5)
            cout << mod (a,b) << endl; }
    
        else {
            cout << "error" << endl;
        }
}


int main ()
{
     calc ();
    do {
    cout << "Do you want another operation" << endl;
        cin >> d;
        if (d=='y')
        calc ();
    } while (d=='y');
    
    return 0;

}
    
