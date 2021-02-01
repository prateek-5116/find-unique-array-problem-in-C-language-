int findUnique(int *arr, int size)
{
   for(int i=0;i<size;i++){
       bool unique=true;
       for(int k=0;k<size;k++){
           if(k==i){
               continue;
           }
           if(arr[i]==arr[k]){
               unique=false;
               break;
           }
          }
       if(unique)
           return arr[i];
     }    
 }
//we have to find an unique element present in the arrat
