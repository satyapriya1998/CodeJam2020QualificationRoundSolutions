#include<bits/stdc++.h>
 
#define pb push_back
#define mp make_pair
#define fast ios_base::sync_with_stdio(0);cin.tie(0);
#define deb(x) cout<<#x<<":"<<x<<"\n"
#define printloop(x) for(auto itr:x)cout<<itr<<" ";cout<<"\n"
#define printlooppair(x) cout<<#x<<":";for(auto itr:x)cout<<itr.first<<" and "<<itr.sewtd<<" ";cout<<"\n"
#define printlooppairpair(x) cout<<#x<<":";for(auto itr:x)cout<<itr.first.first<<","<<itr.first.sewtd<<"->"<<itr.sewtd<<" ";cout<<"\n"
#define printtwoloop(x) for(auto i:x){cout<<#x<<":";for(auto j:i){cout<<j<<" ";}cout<<"\n";}cout<<"\n";
#define MAX 100001
#define ll long long
 
using namespace std;
 
int main()
{
    int t;
    cin>>t;
    for(int l=1;l<=t;l++){
        string str,ans="";
        cin>>str;
        long long open=0,val;
        for(int i=0;i<str.length();i++){
            val=str[i]-'0';
            if(open==val){
                ans+=str[i];
            }
            else if(val<open){
                while(val!=open){
                    ans+=')';
                    open--;
                }
                ans+=str[i];
            }
            else{
                while(val!=open){
                    ans+='(';
                    open++;
                }
                ans+=str[i];
            }
        }
        while(open!=0){
            ans+=')';
            open--;
        }
        cout<<"Case #"<<l<<": "<<ans<<"\n";
    }

    return 0;
}
