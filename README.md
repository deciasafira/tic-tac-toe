# tic-tac-toe
source code

#include <stdio.h>
#include <stdlib.h>

void board();
void petunjukpermainan1();
void petunjukpermainan2();
void mainmenu();
char square[10] = {'o','1','2','3','4','5','6','7','8','9'};

//Variabel Global
int modepermainan;

int main (){
	printf ("\n\nHallo, Selamat Datang!\nKetik apa saja dan tekan enter untuk melanjutkan ke Main Menu");

	mainmenu();
	
	if (modepermainan == 1){
//		int player = 1,i,choice;
//		int menang;
//    	char mark;
    	
		board();
	}
	else if (modepermainan == 2){
		
	}
	else if (modepermainan == 3){
		
	}
	else{
		
	}
	
	return 0;
}

void mainmenu() {
	printf ("\n\n[[MAIN MENU]]\nPilih mode permainan");
	printf ("\n\nKetik 1 untuk mode permainan VS FRIEND\nKetik 2 untuk mode permainan VS COMPUTER");
	printf ("\nKetik 3 untuk keluar dari permainan\n\n");
	scanf ("%d", &modepermainan);
}

void board(){
    system("cls");
    printf("\n\n\tTic Tac Toe\n\n");

    printf("Player 1 (X)  -  Player 2 (O)\n\n");

    printf("     |     |     \n");
    printf("  %s  |  %s  |  %s  \n", square[1],square[2],square[3]);
    printf("_____|_____|_____\n");
    printf("     |     |     \n");
    printf("  %s  |  %s  |  %s  \n", square[4],square[5],square[6]);
    printf("_____|_____|_____\n");
    printf("     |     |     \n");
    printf("  %s  |  %s  |  %s  \n", square[7],square[8],square[9]);
    printf("     |     |     \n");
}
