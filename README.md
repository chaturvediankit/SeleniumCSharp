# SeleniumCSharp
Scanner sc=new Scanner(System.in);
        String s=sc.nextLine();
        String word[] = s.split(" ");
    for(int i=0; i<word.length;i++){

        for(int j=0; j<word[i].length();j++)
        {    int n=word[i].length();
            if(word[i].charAt(j)=='t'){
                if(n==1){
                    System.out.print(word[i]);
                    System.out.println();
                    break;
                }
                else if((n%2)==0){
                  for(int k=0; k<n;k++){
                      System.out.print(word[i].charAt(k+1));
                      System.out.print(word[i].charAt(k));
                      k=k+1;
                  } 
                  System.out.println();
                  break;
                }
                else if((n%2)==1){
                    for(int k=0; k<n;k++){
                      
                      if(k!=n-1){
                       System.out.print(word[i].charAt(k+1));
                       System.out.print(word[i].charAt(k));
                       k=k+1;
                      }
                      else{
                        System.out.print(word[i].charAt(k));  
                      }   
                  }
                    System.out.println();
                    break;
                }
                break;
               }
            else if(j==n-1&&i==word.length-1){
            	System.out.println("None");
                break;
            
                
            }
       
        }
        }
