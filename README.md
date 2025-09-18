# Test-repo-for-credentials
Bogatu Alexei Daw-241

I love HK amd Silk

#include <iostream>
using namespace std;

int main(){
    int n, i, j;
    cout << "Introduceti numarul n" << endl;
    do{
        cout << "n=";
        cin >> n;
        if(n<2 || n>23)  cout << "Introduceti alt numar n." << endl;
    }while(n<2 || n>23);
    int v[n][n]; 
    for(i=0; i<n; i++)
    for(j=0; j<n; j++){
        do{
            cout << "v[" << i << "][" << j << "]=";
            cin >> v[i][j];
            if(v[i][j]<-10000 || v[i][j]>10000) cout << "Introduceti alt numar pentru v[" << i << "][" << j << "]" << endl;
        }while(v[i][j]<-10000 || v[i][j]>10000);
    }
    cout << endl;
    for(i=0; i<n; i++){
        for(j=0; j<n; j++){
            cout << v[i][j] << " ";
        }
        cout << endl;
    }
    cout << endl;
    i=0;
    for(j=0; j<n; j++){
        cout << v[i][j] << " ";
    }
    j=n-1;
    for(i=1; i<n; i++){
        cout << v[i][j] << " ";
    }
    i=n-1;
    for(j=n-2; j>=0; j--){
        cout << v[i][j] << " ";
    }
    j=0;
    for(i=n-2; i>0; i--){
        cout << v[i][j] << " ";
    }
    
    return 0;
}
