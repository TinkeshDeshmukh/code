import java.util.*;
class Main
{
  public static void main(String args[])
  {
    //Try out your code here
    Scanner sc=new Scanner(System.in);
    int size=sc.nextInt();
    int [][]matrix=new int[size][size];
    for(int i=0;i<size;i++){
      for(int j=0;j<size;j++){
    	matrix[i][j]=sc.nextInt();    
      }
    }
    boolean isUTM=true;
      for(int i=0;i<size;i++){
      for(int j=0;j<i;j++){
    	if(matrix[i][j]!=0){
          isUTM=false;
          break;
        }
      }
    }
    if(isUTM){
     System.out.println("Upper triangular matrix"); 
    }else{
           System.out.println("Not an Upper triangular matrix"); 

    }
  }
}
