#include<bits/stdc++.h>
using namespace std;


void conl(string& s){
    for(char& c:s){
        if(c=='1')c='0';
        else if(c=='0')c='1';
    }
}

int main() {
    int t,n;
    cin>>t>>n;
    while(t--){
        int i,j,r=-1,c=-1;
        char q,End;
        string s(n,'?');
        for(i=1,j=0;j<n/2;i+=2)
        {
            if(i>10 && i%10==1)
            {
                if(c!=-1)
                {
                    cout << c+1 << endl;
                    cin >> q;
                    if(s[c]!=q)
                        conl(s);
                }
                else
                {
                    cout << "1\n";
                    cin>>q;
                }
                if(r!=-1)
                {
                    cout << r+1 << endl;
                    cin >> q;
                    if(s[r]!=q)
                    reverse(s.begin(),s.end());
                }
                else 
                {
                    cout << "1\n";
                    cin>>q;
                }
            }
            else
            {
                cout << j+1 << endl;
                cin >> s[j];
                cout << n-j << endl;
                cin >> s[n-1-j];
                if(s[j]==s[n-1-j])c=j;
                else if(s[j]!=s[n-1-j])r=j;
                ++j;
            }
        }
        cout<<s<<endl;
        cin>>End;
        if(End=='N')return 0;
    }
}
