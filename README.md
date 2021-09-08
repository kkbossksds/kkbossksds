#include<iostream>
using namespace std;

void bubble_sort(int m[],int t){
	
	for(int i=1;i<=t-1;i++){
	  	
		for(int j=0;j <=t-i-1;j++){
			if(m[j] > m[j+1]){				
			    swap(m[j],m[j+1]);					
			}
		}
	}
}  			
int main(){
	int arr[] ={5,4,3,2,1};
	int n= sizeof(arr)/sizeof(int);
	bubble_sort(arr,n);
	
	for(auto x: arr){
		cout << x <<",";
	}
	
	return 0;
}
