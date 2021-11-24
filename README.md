# proyectodesemestre
#include <iostream> 
using namespace std;

int main() 
  {
  int saldo=500,clave=273,contador=1,deposito,retiro,respuesta=0;

  string usuario="Drake";
  cout<<"escribe usuario:";
  cin >>usuario;
  cout<< "escribe clave:";
  cin >> clave;


if(usuario=="Drake" and clave==273) 
{
  cout<< "bienvenido"<<"\n";
  while(respuesta!=4)
 
{
  cout << "1:=consulta tu saldo"<<endl;
  cout << "2:=ingresar saldo"<<endl; 
  cout << "3:=retirar saldo"<<endl;
  cout <<"4:=salir"<<endl;
  cin >> respuesta;
  
         if (respuesta==1)
         {
         cout <<"tu saldo actual es:"<<saldo<<"\n"; 
         }
             if (respuesta==2)
             {
             cout <<  "ingresa cantidad a depositar"<<"\n";
             cin>>deposito ;
             saldo=saldo+deposito;
             cout << "tu saldo actual es:"<<saldo<<"\n";
             }
                          
                   if (respuesta==3) 
                   {
                   cout <<  "ingresa cantidad a retirar"<<"\n";
                   cin>>retiro ;
                   if (retiro>saldo)
                   {
                   cout << "tu saldo es insuficiente, prueba de nuevo con una cantidad menor"<<"\n";
                   }
                   else
                   {
                   saldo=saldo-retiro;
                   cout << "tu saldo actual es:"<<saldo<<"\n";
                   }
                   }
                        }
}


 else
 {

     cout<< "denegado";
 }
 



  
  return 0;
}
