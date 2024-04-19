# BASICS
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
### Subscriptions
```cpp
INPUT
3
1 100
12 250
16 135
OUTPUT
100
500
405
#include <bits/stdc++.h>
#include <cmath>
using namespace std;

int totalCost(int n, int x) {
    float total = 0;
    if(n%6==0) {
        total = (n/6)*x;
    }else {
        total = ceil(n/6+1)*x;
    }
    return total;
    
}
int main() {
	// your code goes here
    int size, n, x;
    float total = 0;
    cin >> size;
    for(int i=0; i<size; i++) {
        cin >> n >> x;
        total = totalCost(n,x);
        cout << total << "\n";
    }
    
}
```
### Janmansh and Assignments
```cpp
Input
2
7
9
Output
Yes
No
#include <bits/stdc++.h>
using namespace std;

string checkAssignments(int n) {
    int x = 3;
    x+=n;
    if(x <= 10) {
        return "YES";
    }else {
        return "NO";
    }
}
int main() {
	// your code goes here
    int n,x;
    cin >> n;
    for(int i=0; i<n; i++) {
        cin >> x;
        cout << checkAssignments(x) << "\n";
    }
}

```
### Exams
```cpp
INPUT
4
2 10 12
2 10 3
1 5 3
3 6 9
OUTPUT
YES
NO
YES
NO
#include <bits/stdc++.h>
using namespace std;

string checkPassed(int x,int y, int z) {
    if(z>x*y/2) {
        return "YES";      
    }else {
        return "NO";
    }
}
int main() {
	// your code goes here
    int size, n,x,y,z;
    cin >> size;
    for(int i=0; i<size; i++) {
        cin >> x >> y >> z;
        cout << checkPassed(x,y,z) << "\n";
    }
}

```
