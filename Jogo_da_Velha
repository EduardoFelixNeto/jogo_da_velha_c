#include <stdio.h>
#include <stdlib.h>
#include <conio.h>
#include<stdbool.h>

     char jog[2] ;
     char velha [3][3] = {{' ', ' ', ' '} , {' ', ' ', ' '} , {' ', ' ', ' '}};
     int l , c  , n , venc , val_jogada , x = 0 ;   // val_jogada = valida jogada
     bool usuario = false;
     
  int menu()
  {

        int x = 0;
		printf("*--------------------------*\n");
        printf("|--- Jogo da Velha v1.0 ---|\n");
		printf("|--------------------------|\n");
		printf("|--------------------------|\n");
		printf("| Selecione o seu Oponente:|\n");
		printf("|-- 1:Você vs Amigo -------|\n");
		printf("|-- 2:Você vs Computador --|\n");
		printf("*--------------------------*\n");
        scanf("%d", &x );
        switch ( x )
        {
                 case 1:
                 return 1;
                 break;

                 case 2:
                 printf("\n*-----------------------------------*\n");
				 printf("|------- Jogo da Velha v1.0 --------|\n");
				 printf("|-----------------------------------|\n");
				 printf("|-----------------------------------|\n");
				 printf("| Selecione o nível do seu Oponente:|\n");
				 printf("|-- 1:Computador nível Fácil -------|\n");
				 printf("|-- 2:Computador nível Médio -------|\n");
				 printf("|-- 3:Computador nível Difícil -----|\n");
				 printf("*-----------------------------------*\n"); 
                 scanf("%d", &x);
                 printf("%d", x );
					 switch(x)
                    {
                        case 1:
                        return 3;
                        break;
                        
                        case 2:
                        return 4;
                        break;

                        case 3:
                        return 5;
                        break;
                        
                        default:
                        printf("entrada invalida");
                    }
                    
                 default:
                 printf("entrada invalida");
            }
    }


void escolha_simb(char *jog1 , char *jog2)
{

	*jog1 = 'X';
	*jog2 = 'O';
}


void inicializa_velha(){
	
	printf("*---------------------------*\n");
	printf("|--- Jogo da Velha v1.0 ----|\n");
	printf("|---------------------------|\n");
	printf("|---------------------------|\n");
	for( int l = 0 ; l<= 2 ; l++)
	{
	    printf("|");
		for( int c = 0 ; c<= 2 ; c++)
		{   
			printf("--- %c ---", velha[l][c]);
		}
		if(l!=2){
		    printf("|");
			printf("\n|---------------------------|\n");
		}
	}
	printf("|");
	printf("\n*---------------------------*\n");
}
    
    
int jogada_usuario(int lin , int col , char j ){   // funcao q faz a jogada do usuario 
	
	if(lin >= 3 || col >= 3 )
	{
		printf("\n*--------------------------*\n");
		printf("|----- Posição inválida ---|\n");
		printf("*--------------------------*\n");
		return 1 ;
	}
	else if (velha[lin][col] == ' ')
	{
		velha[lin][col] = j;
		return 0;
	}
	else 
	    printf("\n*---------------------------*\n");
		printf("|-- Posição Já Preenchida --|\n");
		printf("*---------------------------*\n");
		return 2 ;
}
	
	

void jogada()
{
		  printf("\nL ");
		  scanf("%d" , &l);
		  printf("C ");
		  scanf("%d" , &c);
}
int jogada_final( char j)	
{
	         if(velha[0][0] == j && velha[2][2] == j && velha[1][1] == ' ' )  {	velha[1][1] = j;   return 1;  }          //   00 | 01 | 02
     	else if(velha[0][2] == j && velha[2][0] == j && velha[1][1] == ' ')  {	velha[1][1] = j;   return 1;  }          //   10 | 11 | 12
     	else if(velha[1][0] == j && velha[1][1] == j && velha[1][2] == ' ')  {	velha[1][2] = j;   return 1;  }          //   20 | 21 | 22
       	else if(velha[0][0] == j && velha[0][1] == j && velha[0][2] == ' ')  {	velha[0][2] = j;   return 1;  }
       	else if(velha[0][1] == j && velha[0][2] == j && velha[0][0] == ' ')  {	velha[0][0] = j;   return 1;  }      	
       	else if(velha[1][1] == j && velha[1][2] == j && velha[1][0] == ' ')  {	velha[1][0] = j;   return 1;  }
       	else if(velha[2][0] == j && velha[2][1] == j && velha[2][2] == ' ')  {	velha[2][2] = j;   return 1;  }
       	else if(velha[2][1] == j && velha[2][2] == j && velha[2][0] == ' ')  {	velha[2][0] = j;   return 1;  }
       	else if(velha[0][0] == j && velha[1][0] == j && velha[2][0] == ' ')  {	velha[2][0] = j;   return 1;  }
       	else if(velha[1][0] == j && velha[2][0] == j && velha[0][0] == ' ')  {	velha[0][0] = j;   return 1;  }
       	else if(velha[0][1] == j && velha[1][1] == j && velha[2][1] == ' ')  {	velha[2][1] = j;   return 1;  }
       	else if(velha[1][1] == j && velha[2][1] == j && velha[0][1] == ' ')  {	velha[0][1] = j;   return 1;  }
       	else if(velha[0][2] == j && velha[1][2] == j && velha[2][2] == ' ')  {	velha[2][2] = j;   return 1;  }
       	else if(velha[1][2] == j && velha[2][2] == j && velha[0][2] == ' ')  {	velha[0][2] = j;   return 1;  }
       	else if(velha[0][0] == j && velha[0][2] == j && velha[0][1] == ' ')  {	velha[0][1] = j;   return 1;  }
       	else if(velha[0][0] == j && velha[2][0] == j && velha[1][0] == ' ')  {	velha[1][0] = j;   return 1;  }
       	else if(velha[2][0] == j && velha[2][2] == j && velha[2][1] == ' ')  {	velha[2][1] = j;   return 1;  }
       	else if(velha[0][2] == j && velha[2][2] == j && velha[1][2] == ' ')  {	velha[1][2] = j;   return 1;  }
	
}

void nivel2( char j)       // funcao dificuldade nivel 2
{
    int i = 0;

	x = jogada_final(j);   // antes de fazer uma jogada , essa funcao retorna uma possivel vitoria . caso retorna vitoria o jogo acaba
	if(x == 1)
	{
		return;
	}
	int auxl1 , auxc1;
		for (  ; i==0 ; )
		{
			
			auxl1 = rand() % 3 ;    // rand() % x  : � uma funcao q retorna um valor aleatorio , nesse caso foi escolhido valor entre 0 ate 2 q fica  assim = rand() % 3 ;
			auxc1 = rand() % 3 ;
		   if(velha[auxl1][auxc1] == ' ')
		   {
		         i=1;
		         velha[auxl1][auxc1] = j;
	       }
	    }
}
	
	
void nivel3(char j)     // funcao dificuldade nivel 3
{
	x = jogada_final(j);    // antes de fazer uma jogada , essa funcao retorna uma possivel vitoria . caso retorna vitoria o jogo acaba
	if(x == 1)
	{
		return;
	}
           	if(velha[1][1] == ' ' )	  {		velha[1][1] = j	;   }
        else if(velha[0][0] != j && velha[2][2] != j && velha[0][0] != ' ' && velha[2][2] != ' ' && velha[1][0] == ' ')  {	velha[1][0] = j;   }
     	else if(velha[0][2] != j && velha[2][0] != j && velha[0][2] != ' ' && velha[2][0] != ' ' && velha[2][1] == ' ')  {	velha[2][1] = j;   }
     	else if(velha[1][0] != j && velha[1][1] != j && velha[1][0] != ' ' && velha[1][1] != ' ' && velha[1][2] == ' ')  {	velha[1][2] = j;   }
       	else if(velha[0][0] != j && velha[0][1] != j && velha[0][0] != ' ' && velha[0][1] != ' ' && velha[0][2] == ' ')  {	velha[0][2] = j;   }
       	else if(velha[0][1] != j && velha[0][2] != j && velha[0][1] != ' ' && velha[0][2] != ' ' && velha[0][0] == ' ')  {	velha[0][0] = j;   }      	
       	else if(velha[1][1] != j && velha[1][2] != j && velha[1][1] != ' ' && velha[1][2] != ' ' && velha[1][0] == ' ')  {	velha[1][0] = j;   }
       	else if(velha[2][0] != j && velha[2][1] != j && velha[2][0] != ' ' && velha[2][1] != ' ' && velha[2][2] == ' ')  {	velha[2][2] = j;   }
       	else if(velha[2][1] != j && velha[2][2] != j && velha[2][1] != ' ' && velha[2][2] != ' ' && velha[2][0] == ' ')  {	velha[2][0] = j;   }
       	else if(velha[0][0] != j && velha[1][0] != j && velha[0][0] != ' ' && velha[1][0] != ' ' && velha[2][0] == ' ')  {	velha[2][0] = j;   }
       	else if(velha[1][0] != j && velha[2][0] != j && velha[1][0] != ' ' && velha[2][0] != ' ' && velha[0][0] == ' ')  {	velha[0][0] = j;   }
       	else if(velha[0][1] != j && velha[1][1] != j && velha[0][1] != ' ' && velha[1][1] != ' ' && velha[2][1] == ' ')  {	velha[2][1] = j;   }
       	else if(velha[1][1] != j && velha[2][1] != j && velha[1][1] != ' ' && velha[2][1] != ' ' && velha[0][1] == ' ')  {	velha[0][1] = j;   }
       	else if(velha[0][2] != j && velha[1][2] != j && velha[0][2] != ' ' && velha[1][2] != ' ' && velha[2][2] == ' ')  {	velha[2][2] = j;   }
       	else if(velha[1][2] != j && velha[2][2] != j && velha[1][2] != ' ' && velha[2][2] != ' ' && velha[0][2] == ' ')  {	velha[0][2] = j;   }
       	else if(velha[0][0] != j && velha[0][2] != j && velha[0][0] != ' ' && velha[0][2] != ' ' && velha[0][1] == ' ')  {	velha[0][1] = j;   }
       	else if(velha[0][0] != j && velha[2][0] != j && velha[0][0] != ' ' && velha[2][0] != ' ' && velha[1][0] == ' ')  {	velha[1][0] = j;   }
       	else if(velha[2][0] != j && velha[2][2] != j && velha[2][0] != ' ' && velha[2][2] != ' ' && velha[2][1] == ' ')  {	velha[2][1] = j;   }
       	else if(velha[0][2] != j && velha[2][2] != j && velha[0][2] != ' ' && velha[2][2] != ' ' && velha[1][2] == ' ')  {	velha[1][2] = j;   }
       	else  { nivel2(j); } 

    
			 	
}	

		
void jogada_computador(char j , int nivel)
{
	int lc , cc , x , i ;

	if ( nivel == 1){
    for( lc = 0 ; lc <= 2 ; lc++ )  //lc = linha computador
	{
	    for(  cc = 0 ; cc <= 2 ; cc++ )  // cc = coluna computador
	       {
		      if(velha[lc][cc] == ' ')
		      {
		      	velha[lc][cc] = j;
		      	return;
			  }
		
	       }		
	}
	}
	else if ( nivel == 2)
	{
        nivel2(j);
	}
   if ( nivel == 3)
   {
      	nivel3(j);
   }

}	





int verifica_ganhador( char j)  // caso algum jogador ganha vai retorna valor 1
{
	     if(velha[0][0] == j  && velha[0][1] ==  j  && velha[0][2] == j ){return 1;	}
	     if(velha[1][0] == j  && velha[1][1] ==  j  && velha[1][2] == j ){return 1;	}
	     if(velha[2][0] == j  && velha[2][1] ==  j  && velha[2][2] == j ){return 1;	}
	     if(velha[0][0] == j  && velha[1][0] ==  j  && velha[2][0] == j ){return 1;	}
	     if(velha[0][1] == j  && velha[1][1] ==  j  && velha[2][1] == j ){return 1;	}
	     if(velha[0][2] == j  && velha[1][2] ==  j  && velha[2][2] == j ){return 1;	}
	     if(velha[0][0] == j  && velha[1][1] ==  j  && velha[2][2] == j ){return 1;	}
	     if(velha[0][2] == j  && velha[1][1] ==  j  && velha[2][0] == j ){return 1;	}


}
	int main (){

         int i = 0;
         i = menu();
         if( i > 2)
             {
                 i -= 2 ;
                 switch(i)
                 {
                     case 1:
                     printf("\n*---------------------*\n");
					 printf("|-- Você selecionou:--|\n");
					 printf("|---- Nível Fácil ----|\n");
					 printf("*---------------------*\n");
                     n= 1;
                     break;

                     case 2:
                     printf("\n*---------------------*\n");
					 printf("|-- Você selecionou:--|\n");
					 printf("|---- Nível Médio ----|\n");
					 printf("*---------------------*\n");
                     n=2;
                     break;

                     case 3:
                     printf("\n*---------------------*\n");
					 printf("|-- Você selecionou:--|\n");
					 printf("|--- Nível Difícil ---|\n");
					 printf("*---------------------*\n");
                     n=3;
                     break;
                 }
            }
            else
			{	
                     printf("\n*---------------------*\n");
					 printf("|-- Você selecionou:--|\n");
					 printf("|--- Você vs Amigo ---|\n");
					 printf("*---------------------*\n");
                     usuario = true;
            }
        
		printf("\n*--------------------------*\n");
        printf("|--- Jogo da Velha v1.0 ---|\n");
		printf("|--------------------------|\n");
		printf("|--------------------------|\n");
		printf("|-- Escolha o seu símbolo: |\n");
		printf("|-- 1: X ------------------|\n");
		printf("|-- 2: O ------------------|\n");
		printf("*--------------------------*\n");
		scanf("%d" , &i);
		if(i == 1)
			escolha_simb(&jog[0] , &jog[1]);
		
        else
			escolha_simb(&jog[1] , &jog[0]);
		
		printf("\n*------------------------------------*\n");
		printf("*-- Você está com o %c --------------*\n", jog[0]);  
		printf("*-- O outro jogador está com o %c ---*\n", jog[1]);
		printf("*------------------------------------*\n");
		
		for( i = 0 ; i <= 8 ; i++)
		{
		  system("clear");
          inicializa_velha();
		  printf("\n*------------------------------------*\n");
          printf("*------- É a Vez do Jogador %c ------*\n",jog[i%2]);
		  printf("*------------------------------------*\n");
          if(i%2 == 0 || usuario == true )
          {
		  do
		  {
             jogada(); 
		     val_jogada = jogada_usuario(l-1 , c -1, jog[i%2]);
		      if(val_jogada != 0 )
		     {
				printf("\n*------------------------------------*\n");
		  	    printf("*----- Tente Novamente Jogador %c ---*\n" , jog[i%2]);
				printf("*------------------------------------*\n");

		     }
	          }while(val_jogada != 0);
	     }
	     else
	     {
	     	jogada_computador(jog[i%2] , n);
		 }
	     
	     venc = verifica_ganhador(jog[i%2]);

	     if( venc == 1 )
	     {
		 system("clear");
	     inicializa_velha();
		 printf("\n*------------------------------------*\n");
		 printf("|-------------- PARABÉNS --------------|\n");
		 printf("|---------- jogador %c Ganhou ---------|\n", jog[i%2]);
		 printf("*--------------------------------------*\n");
         i = 10;

	     }
		 
	    }
	    if( i == 8)
	    {
	    	printf("\nnao ouve nenhum ganhador ");
		}
		
}
