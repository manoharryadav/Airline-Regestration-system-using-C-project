#include<iostream>
#include<fstream>
#include<iomanip>

using namespace std;

void mainMenu();

class Management
{
    public :
     Management()
     {
         mainMenu();

     }
};

class Details
{

    public:
       static string name, gender;
       int phoneNo;
       int age;
       string add;
       static int cId;
       char arr[100];

       void information()
       {
        cout<<"\nEnter the customer ID: ";
        cin>>cId;
        cout<<"\nEnter the Name: ";
        cin>>name;
        cout<<"\nEnter the age: ";
        cin>>age;
        cout<<"\nEnter the Address : ";
        cin>>add;
        cout<<"\nGender : ";
        cin>>gender;
        cout<<"  Your details are saved with us\n   "<<endl;
       }

};
int Details::cId;
string Details::name;
string Details::gender;

class registration
{
     public:
       static int choice;
       int choice1;
       int back;
       static float charges;

      void flights()
      {
        string flightN[]={"dubai","canada","UK","USA","Austrilia","Europe","India"};

        for(int a=0;a<7;a++)
        {
            cout<<(a+1)<<".flight to"<<flightN[a]<<endl;
        }
        cout<<"\n Welcome to the Airlines!!  "<<endl;
        cout<<"press the number to which country you want to book your flight:  ";
        cin>>choice;

        switch(choice)
        {
              case 1:
              {
                cout<<"________Welcome to dubai Emirates_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. DUB - 498 "<<endl;
                cout<<"\t08-11-2023 8:00AM 10hrs Rs.14000"<<endl;
                  cout<<"2. DUB - 698 "<<endl;
                cout<<"\t09-11-2023 10:00AM 15hrs Rs.9000"<<endl;
                  cout<<"3. DUB - 798 "<<endl;
                cout<<"\t10-11-2023 7:00PM 9hrs Rs.20000"<<endl;

                cout<<"\nSelect the flight you want to book : ";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=14000;
                  cout<<"\nYou successfully booked the flight  DUB-498 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                 else if (choice1==2)
                {
                  charges=9000;
                  cout<<"\nYou successfully booked the flight  DUB - 698 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                 else if (choice1==3)
                {
                  charges=20000;
                  cout<<"\nYou successfully booked the flight  DUB-798 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu :"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu :"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
                
              }
              case 2:
              {
                   cout<<"________Welcome to canadian airlines_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. CA - 498 "<<endl;
                cout<<"\t08-11-2023 8:00AM 10hrs Rs.25000 "<<endl;
                  cout<<"2. CA - 698 "<<endl;
                cout<<"\t09-11-2023 10:00AM 15hrs Rs.30000 "<<endl;
                  cout<<"3. CA - 798 "<<endl;
                cout<<"\t10-11-2023 7:00PM 9hrs Rs.35000 "<<endl;

                cout<<"\nSelect the flight you want to book : ";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=25000;
                  cout<<"\nYou successfully booked the flight  CA-498 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                 else if (choice1==2)
                {
                  charges=30000;
                  cout<<"\nYou successfully booked the flight  CA - 698 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                 else if (choice1==3)
                {
                  charges=35000;
                  cout<<"\nYou successfully booked the flight  CA-798 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket "<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu "<<endl;
                  flights();
                }
                cout<<"press any Number key to  go back to main menu "<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              case 3:
              {

                   cout<<"________Welcome to UK AIRWAYS_______\n "<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. UK- 498 "<<endl;
                cout<<"\t10-11-2023 8:00AM 15hrs Rs.44000 "<<endl;
                 

                cout<<"\nSelect the flight you want to book :";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=44000;
                  cout<<"\nYou successfully booked the flight  UK-498"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                
                else {
                  cout<< "invalid input ,shifting to previous menu"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              case 4:
              {
                cout<<"________Welcome to US AIRWAYS_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. US - 498 "<<endl;
                cout<<"\t15-11-2023 8:00AM 22hrs Rs.37000"<<endl;
                  cout<<"2. US2A - 698 "<<endl;
                cout<<"\t18-11-2023 10:00AM 25hrs Rs.39000"<<endl;
                  cout<<"3. US - 798 "<<endl;
                cout<<"\t20-11-2023 7:00PM 30hrs Rs.45000"<<endl;

                cout<<"\nSelect the flight you want to book :";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=37000;
                  cout<<"\nYou successfully booked the flight  US-498 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==2)
                {
                  charges=39000;
                  cout<<"\nYou successfully booked the flight  US2A - 698 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==3)
                {
                  charges=45000;
                  cout<<"\nYou successfully booked the flight  US-798 "<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              case 5:
              {
                cout<<"________Welcome to Austrialian flights_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. AUS - 498 "<<endl;
                cout<<"\t01-11-2023 8:00AM 18hrs Rs.24000"<<endl;
                  cout<<"2. AUS - 698 "<<endl;
                cout<<"\t03-11-2023 10:00AM 20hrs Rs.20000"<<endl;
                  cout<<"3. AUS - 798 "<<endl;
                cout<<"\t07-11-2023 7:00PM 24hrs Rs.16000"<<endl;

                cout<<"\nSelect the flight you want to book :";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=24000;
                  cout<<"\nYou successfully booked the flight  AUS-498"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==2)
                {
                  charges=20000;
                  cout<<"\nYou successfully booked the flight  AUS - 698"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==3)
                {
                  charges=16000;
                  cout<<"\nYou successfully booked the flight  AUS-798"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              case 6:
              {
                cout<<"________Welcome to EUROPIAN Emirates_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. EU- 498 "<<endl;
                cout<<"\t10-11-2023 8:00AM 30hrs Rs.14000"<<endl;
                  cout<<"2. EU - 698 "<<endl;
                cout<<"\t13-11-2023 10:00AM 25hrs Rs.15000"<<endl;
                  cout<<"3. EU - 798 "<<endl;
                cout<<"\t15-11-2023 7:00PM 19hrs Rs.20000"<<endl;

                cout<<"\nSelect the flight you want to book :";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=14000;
                  cout<<"\nYou successfully booked the flight  EU-498"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==2)
                {
                  charges=15000;
                  cout<<"\nYou successfully booked the flight  EU - 698"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==3)
                {
                  charges=20000;
                  cout<<"\nYou successfully booked the flight  EU-798"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              case 7:
              {
                cout<<"________Welcome to INDIAN AIRWAYS_______\n"<<endl;
                cout<<"Following  are the flights \n"<<endl;

                cout<<"1. IND - 498 "<<endl;
                cout<<"\t18-11-2023 8:00AM 10hrs Rs.14000"<<endl;
                  cout<<"2. IND - 698 "<<endl;
                cout<<"\t09-11-2023 10:00AM 15hrs Rs.9000"<<endl;
                  cout<<"3. IND - 798 "<<endl;
                cout<<"\t10-11-2023 7:00PM 9hrs Rs.20000"<<endl;

                cout<<"\nSelect the flight you want to book :";
                cin>>choice1;

                if (choice1==1)
                {
                  charges=14000;
                  cout<<"\nYou successfully booked the flight  IND-498"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==2)
                {
                  charges=9000;
                  cout<<"\nYou successfully booked the flight  IND - 698"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                 else if (choice1==3)
                {
                  charges=20000;
                  cout<<"\nYou successfully booked the flight  IND-798"<<endl;
                  cout<<" you can go back to main menu and collect the ticket"<<endl;
                }
                else {
                  cout<< "invalid input ,shifting to previous menu"<<endl;
                  flights();
                }
                cout<<"press any number key to go back to main menu"<<endl;
                cin>>back;
                if (back==1)
                {
                  mainMenu();
                }
                else
                {
                  mainMenu();
                }
              }
              default :
              {
                cout<<"invalid input, shifting to main menu....please try again!!!"<<endl;
                 mainMenu();
                 break;
              }
        }
      }
};
float registration::charges;
int registration::choice;

class ticket : public registration,Details
{
  public :
    void Bill()
    {
      string Destination="";
      ofstream outf("records.txt");
      {
        outf<<"___________________MANU Airlines______________"<<endl;
        outf<<"___________________Ticket____________________"<<endl;
        outf<<"_____________________________________________"<<endl;

        outf<<"customerID:"<<Details::cId<<endl;
        outf<<"customer Name:"<<Details::name<<endl;
        outf<<"customer gender:"<<Details::gender<<endl;
        outf<<"\tDescription"<<endl<<endl;

        if(registration::choice==1)
        {
          Destination="Dubai";
        }
         else if(registration::choice==2)
        {
          Destination="Canada";
        }
         else if(registration::choice==3)
        {
          Destination="UK";
        }
        else if(registration::choice==4)
        {
          Destination="USA";
        }
         else if(registration::choice==5)
        {
          Destination="Austrilia";
        }
         else if(registration::choice==6)
        {
          Destination="Europe";
        }
        else if(registration::choice==7)
        {
          Destination="India";
        }
       
       outf<<"Destination  \t\t"<<Destination<<endl;
       outf<<"Flight cost   :\t\t "<<registration::charges<<endl;

      }
      outf.close();
    }
    void dispBill()
    {
      ifstream ifs("records.txt");
      {
        if(!ifs)
        {
          cout<<"file error!!"<<endl;
        }
        while(!ifs.eof())
        {
          ifs.getline(arr,100);
          cout<<arr<<endl;
        }
      }
      ifs.close();
    }

};



void mainMenu()
{
    int lchoice;
    int schoice;
    int back;

    cout<<"\t       _______MANUU______ AIRLINES \n"<<endl;
    cout<<"\t       _______MAIN MENU___________ "<<endl;
    cout<<"\t________________________________________________________"<<endl;
    cout<<"\t|\t\t\t\t\t\t\t|"<<endl;
    cout<<"\t|\t press 1 to add the Customer Details            |"<<endl;
    cout<<"\t|\t press 2 for Flight Registration                |"<<endl;
    cout<<"\t|\t press 3 for Ticket and Charges                 |"<<endl;
    cout<<"\t|\t press 4 to  Exit                               |"<<endl;
    cout<<"\t|\t\t\t\t\t\t\t|"<<endl;
    cout<<"\t________________________________________________________"<<endl;

    cout<<"Enter the choice :  ";
    cin>>lchoice;

    Details d;
    registration r;
    ticket t;

     switch(lchoice)
     {
        case 1:
        {
            cout<<"______________Customers___________\n"<<endl;
            d.information();
            cout<<"press any  number key to go back to main menu";
            cin>>back;

            if(back==1)
            {
                 mainMenu();
                
            }
            else{
                mainMenu();

            }
            break;
        }
        case 2:{
            cout<<"________Book a flight using this system ________\n"<<endl;
            r.flights();
            break;
        }
          case 3:{
          cout<<"___________GET YOUR TICKET________\n"<<endl;
          t.Bill();

          cout<<"Your ticket is printed ,you can collect it \n "<<endl;
          cout<<"press 1 to display your ticket ";
          
          cin>>back;
              

               if (back==1)
               {
                t.dispBill();
                cout<<"press any number  key to go back to main menu:";
                cin>>back;
                if(back==1)
                {
                       mainMenu();
                }
                else{
                     mainMenu();
                }
               }
               else{
                    mainMenu();
               }
               break;
          }
               
               case 4:
               {
                cout<<"\n\n\t__________Thankyou__________"<<endl;
                break;
               }
               default :
               {
                cout<<"Invalid choice, please TRY Again!!\n"<<endl;
                mainMenu();
                break;
               }
     }
}


int main()
{
  Management Mobj;
  return 0;
}