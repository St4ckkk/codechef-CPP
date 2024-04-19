#BASICS
### Greater Average

```cpp
INPUT
5
5 9 6
5 8 6
5 7 6
4 9 8
3 7 2
OUTPUT
YES
YES
NO
NO
YES
#include <bits/stdc++.h>
#include <string>
using namespace std;

string checkGreaterthanC(float a, float b, float c) {
    
    float avg = (a+b)/2;                                                                                                                    
    if(avg > c) {                    
        return "YES";
    }else {
        return "NO";
    }
}

int main() {
	// your code goes here
    int size;
    float a,b,c;
    string check;
    cin >> size;
    for(int i = 0; i<size; i++) {
        cin >> a >> b >> c;
        check = checkGreaterthanC(a,b,c);
        cout << check << "\n";
    }
}


```