# Projects
 #include<stdlib.h>
#include<stdio.h>
#include<time.h>
main ()
{
  int zar1, zar2, toplam = -1, a = -1;

  srand (time (NULL));
  while (toplam != 0)
    {
      toplam++;

      zar1 = (rand () % 6) + 1;
      zar2 = (rand () % 6) + 1;

      toplam = zar1 + zar2;

      if (toplam == 7 || toplam == 11)
	{
	  printf ("Tebrikler kazandiniz!!\n");
	  printf ("Toplam olarak atisiniz %d geldi", toplam);
	  break;
	}

      if (toplam == 2 || toplam == 3 || toplam == 12)
	{
	  printf ("Maalesefki kaybettiniz.\n");
	  printf ("Toplam olarak atisiniz %d geldi", toplam);
	  break;
	}

      if (toplam == 4 || toplam == 5 || toplam == 6 || toplam == 8
	  || toplam == 9 || toplam == 10)
	{
	  while (a == -1)
	    {
	      zar1 = 0;
	      zar2 = 0;
	      int toplam2 = 0;
	      zar1 = (rand () % 6) + 1;
	      zar2 = (rand () % 6) + 1;
	      toplam2 = zar1 + zar2;
	      if (toplam2 == 7)
		{
		  printf ("Maalesefki kaybettiniz.\n");
		  printf("Toplam olarak atisiniz %d geldi.",toplam2);
		  break;
		}
	      if (toplam2 == toplam)
		{
		  printf ("Tebrikler kazandiniz.\n");
		  printf("Toplam olarak atisiniz %d geldi.",toplam2);
		  break;
		}

	    }

	}
      break;
    }
}
