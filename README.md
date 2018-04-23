#include <iostream>
#include <bits/stdc++.h>
#include <cstring>
#define kol 20
#define bar 20

using namespace std;
int main(){
	int n,test,temu,PanjangKata;
	temu=0;
	char word[100];
	char kata[15][15]={ {'t','g','b','w','w','i','n','t','e','r','w','s','e','s','n'},
						{'a','a','u','n','t','t','m','m','h','f','o','o','d','n','b'},
						{'j','l','w','c','q','l','d','z','m','p','m','v','d','m','r'},
						{'a','s','a','g','m','q','u','w','v','v','b','s','o','h','i'},
						{'b','w','p','l','o','t','a','n','a','d','t','p','g','n','c'},
						{'r','e','w','n','g','o','d','j','c','p','n','a','t','n','k'},
						{'e','e','o','t','w','o','s','b','q','h','a','r','r','s','a'},
						{'a','z','c','g','e','s','w','e','w','n','a','k','n','p','b'},
						{'d','i','n','n','e','r','q','o','d','l','w','d','c','a','r'},
						{'o','n','o','p','k','w','m','p','a','r','k','t','z','c','c'},
						{'q','b','f','r','o','g','m','a','m','w','p','w','e','e','y'},
						{'l','q','z','q','n','n','m','r','z','j','j','s','c','l','g'},
						{'m','o','s','g','z','c','z','e','t','d','b','o','o','t','o'},
						{'p','d','c','r','z','m','s','n','g','r','d','n','r','p','z'},
						{'o','h','n','k','z','w','a','t','e','r','j','g','t','r','a'}
						};
						
						
				
	for(int i=0;i<15;i++){
		for (int j=0;j<15;j++){
			cout<<kata[i][j]<<" ";
		}
		cout<<endl;
	}
	cout<<endl;
	cout<<"Berapa Kata yang Ingin dicari : "; cin>>n;
	for (int i=0; i<3; i++){
	}
	for(int i=0;i<n;i++){
		cout<<"Input Kata yang ingin dicari : ";cin>>word;
	PanjangKata=strlen(word);
}

	for (int i=0;i<15;i++){
		for (int j=0;j<15;j++){
			if (word[0]==kata[i][j]){
				for (int a=0;a<PanjangKata;a++){
					if (word[a]==kata[i][j+a]){
						test=a;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i][j-k]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i+k][j]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i-k][j]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i-k][j-k]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i-k][j+k]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i+k][j-k]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;
				for (int k=0;k<PanjangKata;k++){
					if (word[k]==kata[i+k][j+k]){
						test=k;
					}
					else{
						break;
					}
				}
				if (test==PanjangKata-1){
					temu+=1;
				}
				else{
					temu+=0;
				}
				test=0;	
			}}	}
				cout<<"================================== "<<endl;
	for (int i=0; i<n; i++){
	if(word[i]==1){
		cout<<i+1<<"Kata "<<word<<" Ada di dalam tabel ";
	}
	else {
		cout<<i+1<<"kata "<<word<<" Tidak ada di dalam tabel ";
	}
	}
	}

