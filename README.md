# algo2
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
        
        <li><a href="#TP2">TP2</a></li>

       
  </ol>
</details>

```c++
void saisirComplexe(Complexe *t){
 	
 	printf("entrez le re:\n");
 	scanf("%f",&t->re);
 	
 	printf("entrez le img:\n");

 	scanf("%f",&t->img);
 	
 	
 }
 
 //afficher
 void afficher (Complexe *f){
 	
 	printf("vuillez afficher les elemnts svp:\n");
 	
 	printf("le re est: %f\n",f->re);
 	 	printf("le img est: %f\n",f->img);

 }
  
  
  ```c++
void creerListe(Liste *t,int N){
	
	t->lmax=N;
	t->taille=0;
	t->tab=malloc(sizeof(Liste));
	
	
	
}
  ```
  
  
  ```c++
void insererDebutListe(Liste *l,float v){
int i=0;
	if(l->taille==l->lmax){
		l->lmax*=2;
		l->tab=(float *)realloc(l->tab,l->lmax);
	}
	
	for(i=l->taille-1;i>=0;i--){
		
		l->tab[i+1]=l->tab[i];
		l->tab[0]=v;
		l->taille++;
	}
}
  ```
  
  
  ```c++
void saisirliste(Liste *l){
printf("veuillez saisir les elements de la liste\n");
printf("entrez la taille :\n");
scanf("%d",&l->taille);
printf("entrez lmax:\n");
scanf("%d",&l->lmax);
printf("entrer les elemnts de la complexe:\n");
printf("entrez  le re:\n");
scanf("%f",&l->tab->re)


printf("entrez le img:\n");
scanf("%f",&l->tab->img);	

	
}
void afficherListe(Liste *m){

printf("veuillez afficher les elements de la liste\n");	

printf("la taille est: %d",m->taille);
printf("lmax est :%d",m->lmax);

int i=0;
for(i=0;i<m->taille;i++){
	printf("%f",m->tab[i]);
}	
}

  ```
  
  
  ```c++
void programme(Complexe *l,float v){
	// nouvelle liste
Complexe *nouvelleliste=malloc(sizeof(Complexe));
	
	saisirComplexe(l);
	insererDebutListe(l,v);
	afficherListe(l);
	
}	
  ```
  
  ```c++
int i=0;
  	
  	for (i=position+1;i>0;i--){
  		
  		l->tab[i-1]=l->tab[i];
  		l->taille--;
	  }
  }
void supprimerOcculiste(Liste *l,float v){
	
	int i=0;
	
	for(i=0;i<l->taille;i++){
		
		if(l->tab[i]==v){
			
			// on fait l'appel de la fonction
			supprimerelemntliste(l,v);
			i--;
			
		}
	}
}	
  ```
  
  ```c++

  ```
  
  ```c++
   void  clonerListe(Liste liste1,Liste *liste2){
  	
  	int i;
  	creerliste(liste1,liste2,lmax);
  	
  	for (int i=0;i<liste1->taille;i++){
  		
  		liste1->tab[i]=liste2->tab[i];
  		liste1->taille=liste2->taille;
	  }
  }
  

  ```
  12
  
  ```c++
  //a 
 LISTE *L1,L2; 
//b 
 L1=(LISTE*)malloc(sizeof(LISTE)); 
 creerListe(L1,10); 
 creerListe(&L2,20); 
//c 
 COMPLEXE *c1= (COMPLEXE *)malloc(4*sizeof(COMPLEXE)); 
 for(i=0;i<4;i++){ 
 saisirComplexe(&c1[i]); 
 insererDebutListe(L1,c1[i]); 
 } 
  
 COMPLEXE *c2= (COMPLEXE *)malloc(3*sizeof(COMPLEXE)); 
 for(i=0;i<3;i++){ 
 saisirComplexe(&c2[i]); 
 insererDebutListe(&L2,c2[i]); 
 } 
 //d 
 trierListe(L1); 
 trierListe(&L2); 
 //e 
 L2=*L1; 
 printf("L adresse de L1: %p et de L2: %p",L1,&L2); 
 clonerListe(*L1,&L2); 
 printf("L adresse de L1: %p et de L2: %p",L1,&L2); 
 //f 
 afficherListe(L2); 
 //g 
 COMPLEXE co; 
 co.re=8; 
 co.img=5; 
 insererDebutListe(L1,co); 
 //h 
 afficherListe(L2); 
return 0;

  ```


Our Team -[DARBAL nour-elhouda](https://github.com/teamkhaoulanour)

Project Link: [Algorithme](https://https:/https://github.com/Darbal-Nour-elhouda/algo1)

Encadré par : [Mr.Ahmed ](https://)


<p align="right">(<a href="#top">back to top</a>)</p>

