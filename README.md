# B.-Two-Buttons
<!-- codeforces questions -->
#include <bits/stdc++.h>
using namespace std;
typedef long long ll;
#define sof sizeof
typedef double ld;
#define all(v) v.begin(),v.end()
#define ms(dp,a) memset(dp,(ll)a,sof(dp))
#define sqr(x) (x)*(x)
#define pb push_back
#define mod 1000000007
const int N=1e5+10;
const int INF=1e9+10;
#define mkp make_pair
#define inf 1e18
#define minf -1e18
#define rep(i,n) for(ll i=0;i<n;++i)
// vector<ll> per(N);
// vector<ll> adj[N];
// vector<bool> vis(N,false);
// vector<ll> dist(51,0);
// ll bfs(ll s,ll t){
//       std::queue<ll> q;
//       q.push(s);
//       vis[s]=true;
//       dist[s]=1;
//       while(!q.empty()){
//             ll u=q.front();
//             q.pop();
//             // if(u==t) break;
//             for(auto v:adj[u]){
//                 if(vis[v]==false){
//                       q.push(v);
//                       vis[v]=true;
//                       dist[v]=dist[u]+1;
//                 } 
//             }
//       }
//       // (dist[t]==INF)?(return -1):(return dist[t]);
//       if(dist[t]==INF){
//             return -1;
//       }
//       else return dist[t];
      
// }
// bool isPal(string S)
// {
//     // Iterate over the range [0, N/2]
//     for (int i = 0; i < S.length() / 2; i++) {
 
//         // If S[i] is not equal to
//         // the S[N-i-1]
//         if (S[i] != S[S.length() - i - 1]) {
//             // Return No
//             return false;
//         }
//     }
//     // Return "Yes"
//     return true;;
// }
 
// int setBitNumber(int n)
// {
 
//     // To find the position
//     // of the most significant
//     // set bit
//     int k = (int)(log2(n));
 
//     // To return the the value
//     // of the number with set
//     // bit at k-th position
//     return 1 << k;
// }
// ll arr[N];
// bool cmp(const pair<int,int> &a,
//               const pair<int,int> &b)
// {
//     return (a.second > b.second);
// }
// vector<int> prefix_function(string s) {
//     int n = (int)s.length();
//     vector<int> pi(n);
//     for (int i = 1; i < n; i++) {
//         int j = pi[i-1];
//         while (j > 0 && s[i] != s[j])
//             j = pi[j-1];
//         if (s[i] == s[j])
//             j++;
//         pi[i] = j;
//     }
//     return pi;
// }
// Prefix function. Knuth–Morris–Pratt algorithm
// if ( std::equal(v.begin() + 1, v.end(), v.begin()) )
// {
//     //all equal
// }
 
// bool vis[51][51];
// void dfs(ll x,ll y){
//       if(x<0 or y<0 or x>=n or y>=n) return;
//       if(vis[x][y] or vs[x][y]=='1') return;
//       vis[x][y]=true;
      
// //       for(auto &[dx,dy] : dr)
// //     {
// //         dfs(x+dx,y+dy);
// //     }
//        dfs(x+1,y);
//        dfs(x-1,y);
//        dfs(x,y-1);
//        dfs(x,y+1);
// }
// int factorial(int n)
// {
//     // single line to find factorial
//     return (n == 1 || n == 0) ? 1 : n * factorial(n - 1);
// }
// ll m=1;
// long long binpow(long long a, long long b) {
//     long long res = 1;
//     while (b > 0) {
//         if (b & 1)
//             res = res * a;
//         a = a * a;
//         b >>= 1;
//     }
//     return res%mod;
// }
int main(){
        
         ios_base::sync_with_stdio(false);
         cin.tie(NULL);
         
         ll n,m;cin>>n>>m;
         ll s=m;
         ll d=n;
         ll op=0;
         while(s>d){
               if(s%2!=0){
                     op++;
                     s++;
               }
               else{
                     op++;
                     s/=2;
               }
         }
         if(s==d){
               cout<<op<<endl;
               return 0;
         }
         if(s<d){
               while(s<d){
                  op++;
                  s++;
                  if(s==d){
                        cout<<op<<endl;
                        break;
                  }
               }
         }
         
               
                  
         
       //     cout<<"Case #"<<m<<":"<<" "<<cn<<endl;
      //     m++;
         
 return 0;
}
// read the question correctly   
    
  
    
 
 
  
    
 
 
