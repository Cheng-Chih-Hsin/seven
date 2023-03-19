#include<iostream>
using namespace std;

int main() {
    int n;
    cin >> n;//輸入數字後，就會儲存在之前創立好的n裡面
    while (n--)
    {
        int a1, a2, b1, b2;
        char w;
        cin >> w >> a1 >> a2 >> b1 >> b2;
        switch (w) { //變數名稱或運算式
        case '+': //符合數字或字元
        cout << a1 + b1 << " " << a2 + b2 << "\n";
        break;
        case '-':
        cout << a1 - b1 << " " << a2 - b2 << "\n";
        break;
        case '*':
        cout << a1 * b1 - a2 * b2 << " " << a2 * b1 + a1 * b2 << "\n"; break;
        case '/':
        cout << (a1 * b1 + a2 * b2) / (b1 * b1 + b2 * b2) << " " << (a2 * b1 - a1 * b2) / (b1 * b1 + b2 * b2) << "\n"; 
        break;//跳出迴圈
        }
    }

}
