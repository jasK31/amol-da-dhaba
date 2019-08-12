# amol-da-dhaba
#include<iostream>
using namespace std;

 int main()

{
    float totaltax=0,total=0;
    
    int i,table,item,s,temptotal=0,d1=0,d2=0,d3=0,d4=0,d5=0,d6=0;
    cout<<"Enter the Table Number : ";
    cin>>table;
    cout<<"			  Paal Dhaba		  \n ";
    cout<<"            ************      \n\n";
    cout<<"~ Make your selsction from the menu below :\n\n";
    cout<<"	 1. Aloo prontha		          Rs  99\n";
    cout<<"	 2. Double stuffed prontha		  Rs 109\n";
    cout<<"	 3. Paneer sandwich				  Rs 149\n";
    cout<<"	 4. Thaal with Dal/sabjee		  Rs 279\n";
    cout<<"	 5. Special Lassi		 		  Rs  99\n";
    cout<<"	 6. Soft drink		        	  Rs  99\n\n";
    cout<<" *********************************************\n\n";
    cout<<"Enter the NO. of Item's You wanna Order : ";
    cin>>item;
    
    
    for(i=0;i<item;i++)
    {
    cout<<"Enter Your Choice : ";
        cin>>s;
    
    switch (s)
    {
        case 1:
            cout<<"You have ordered the Aloo prontha : Rs 99	\n";
            d1=99;
            break;
            
        case 2:
            cout<<"You have ordered the Double stuffed prontha : Rs 109 \n";
            d2=109;
            break;
            
        case 3:
            cout<<"You have ordered the Paneer sandwich : Rs149\n";
            d3=149;
            break;
            
        case 4:
            cout<<"You have ordered the Thaal with Dal/sabjee : Rs 279 \n";
            d4=279;
            break;
            
        case 5:
            cout<<"You have ordered the Special Lassi : Rs 99\n";
            d5=99;
            break;
            
        case 6:
            cout<<"You have ordered the Soft drink : Rs 99\n";
            d6=99;
            break;
        default:
            break;
            
    }
    }
        temptotal=d1+d2+d3+d4+d5+d6;
    totaltax=temptotal*.17;
    total=temptotal+totaltax;
    cout<<endl<<"  ****************************************"<<endl;
    cout<<endl<<endl<<"Table Number = "<<table<<endl;
    cout<<"Your Order "<<endl;
    cout<<"Total Number of Item Order = "<<item<<endl;
    cout<<"TAX = Rs "<<totaltax<<endl;
    cout<<"Total Bill : Rs "<<total<<endl;
    cout<<"Thank you for eating at Paal Dhaba!\n\n";
}
