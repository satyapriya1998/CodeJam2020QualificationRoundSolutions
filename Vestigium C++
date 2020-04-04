#include<bits/stdc++.h>
 
#define pb push_back
#define mp make_pair
#define fast ios_base::sync_with_stdio(0);cin.tie(0);
#define deb(x) cout<<#x<<":"<<x<<"\n"
#define printloop(x) cout<<#x<<":";for(auto itr:x)cout<<itr<<" ";cout<<"\n"
#define printlooppair(x) cout<<#x<<":";for(auto itr:x)cout<<itr.first<<" and "<<itr.second<<" ";cout<<"\n"
#define printlooppairpair(x) cout<<#x<<":";for(auto itr:x)cout<<itr.first.first<<","<<itr.first.second<<"->"<<itr.second<<" ";cout<<"\n"
#define printtwoloop(x) cout<<#x<<endl;for(auto i:x){for(auto j:i){cout<<j.first<<","<<j.second<<" ";}cout<<"\n";}
#define MAX 1000000007
#define ll long long
 
using namespace std;

int main(){
    fast;
    int t;
    cin>>t;
    for(int l=1;l<=t;l++){
        int n;
        cin>>n;
        int arr[n+1];
        long long sum=0;
        int rows=0,cols=0;
        int mat[n][n],val;
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                cin>>val;
                if(i==j) sum+=val;
                mat[i][j]=val;
            }
        }
        for(int i=0;i<n;i++){
            memset(arr,0,sizeof(arr));
            for(int j=0;j<n;j++){
                if(arr[mat[i][j]]==1){
                    rows++;
                    break;
                }
                arr[mat[i][j]]++;
            }
        }
        for(int j=0;j<n;j++){
            memset(arr,0,sizeof(arr));
            for(int i=0;i<n;i++){
                if(arr[mat[i][j]]==1){
                    cols++;
                    break;
                } 
                arr[mat[i][j]]++;
            }
        }
        cout<<"Case #"<<l<<": "<<sum<<" "<<rows<<" "<<cols<<"\n";
    }
    return 0;
}
