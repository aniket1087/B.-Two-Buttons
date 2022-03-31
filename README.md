# B.-Two-Buttons
<!-- codeforces questions -->

int main(){
        
         ios_base::sync_with_stdio(false);
         cin.tie(NULL);
         
         ll n,m;cin>>n>>m;//taking input
         ll s=m;
         ll d=n;
         ll op=0;//intialize with zero
         //The problem can be reversed as follows--> we should get the number n starting from m using the operations "add 1 to the number" and "divide the number by 2          if it is even".
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
    
  
    
 
 
  
    
 
 
