# #include <iostream>
using namespace std; 

int main() {
    int n, i; //定義整數變數 n 和 i
    cin >> n; //從標準輸入讀入一個整數，存入變數 n
    for (i = 2; i < n; i++) { //從 2 到 n-1 開始迭代
        if (n % i == 0) { //如果 n 整除 i
            break; //跳出迴圈
        }
    }
    if (i == n) { //如果最後的 i 等於 n，代表 n 是質數
        cout << "YES" << endl; //輸出 "YES"，並換行
    }
    else { //否則 n 不是質數
        cout << "NO" << endl; //輸出 "NO"，並換行
    }
    return 0;
}
