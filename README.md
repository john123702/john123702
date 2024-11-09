#include <bits/stdc++.h>
using namespace std;
long long uoc(long long n) {
    long long i;
    for ( i = n / 2; i >= 1; i--) {
        if (n % i == 0) {
            cout<<i;
            break;
        }
    }
    return i;
}
int tongcs(long long n) {
    int sum = 0;
    while (n > 0) {
        sum += n % 10;
        n /= 10;
    }
    return sum;
}
int main() {
    long long n;
    cin >> n;
    cout<<uoc(n)<<endl;
    cout<<tongcs(n);
    return 0;
}
