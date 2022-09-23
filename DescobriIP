#include <stdio.h>
#include <netdb.h>
#include <arpa/inet.h>

int main(int argc, char *argv[])
{
  if (argc == 1){
    printf("\nModo De uso: ./CDNS -hst google.com");
    printf("\n\nopções:\n\n");
    printf("\n\n\t-hst: para expecifica o host");
  }
  if (argc > 1){
    struct hostent *alvo = gethostbyname(argv[2]);
    printf("\nHost => %s\tIP ===> %s\n", argv[2],  inet_ntoa(*((struct in_addr *)alvo->h_addr)));
  }
  return 0;
}
