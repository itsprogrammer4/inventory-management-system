# inventory-management-system

#include <iostream>

using namespace std;

int main()
{
    char lab_ID('o');
    cout<<"press p to execute pre lab"<<endl;
    cout<<"press i to execute in lab"<<endl;
    cin>>lab_ID;
    switch(lab_ID)
    {
        case 'P':
        case 'p':
             int task_choice;
            cout<<"Enter 1 to Task 1 of pre lab"<<endl;
            cout<<"Enter 2 to Task 2 of pre lab"<<endl;
            cout<<"Enter 3 to Task 3 of pre lab"<<endl;
            cout<<"Enter 4 to Task 4 of pre lab"<<endl;
            cout<<"Enter 5 to Task 5 of pre lab"<<endl;
            cout<<"Enter 6 to Task 6 of pre lab"<<endl;
            cout<<"Enter 7 to Task 7 of pre lab"<<endl;
            cin>>task_choice;

            switch (task_choice)
            {
                case 1:
                {
                    cout<<"Task 1"<<endl;
                    for (int i = 1; i <= 10; i++)
                {
                    for (int j=1; j<=10; j++)

                    {
                            cout<< i <<"*"<< j <<"="<< i * j <<endl;
                    }
                }
                }
                break;

                case 2:
                {
                    cout<<"Task 2"<<endl;
                    for (int i = 0 ; i <= 2 ; i++)
                {
                    for (int j = 0 ; j <= 5 ; j++)
                    {
                            cout<<"x";
                    }
                            cout<<endl;
                }
                }
                break;

                case 3:
                {
                    cout<<"Task 3"<<endl;
                    for (int i=0; i<=3; i++)
                    {
                    for (int j=0; j<=5; j++)
                    {
                            cout<<"#";
                            j++;
                            cout<<"?";
                    }
                            cout<<endl;
                    }
                }
                break;

                case 4:
                {
                    cout<<"Task 4"<<endl;
                    for (int i=0; i<=3; i++)
                    {
                    for (int j=0; j<=3; j++)
                    {
                            cout<<"#";
                            cout<<"?";
                    }
                    }
                }
                break;

                case 5:
                    {
                    cout<<"Task 5"<<endl;
                    for (int i = 0 ; i <= 5 ; i++)
                    {
                    for(int j=0 ; j<= i ; j++)
                    {
                            cout<<"*";
                    }
                            cout<<endl;
                    }
                    }
                break;
                case 6:
                    {
                    cout<<"Task 6"<<endl;
                    int rows = 5;
                    for (int i = 0 ; i <= rows ; i++)
                    {
                    for(int j=0 ; j <= rows ; j++)
                    {
                            if (i + j < rows){cout<<"*";}
                            else{cout<<" ";}
                    }
                             cout<<endl;
                    }
                    }
                break;
                case 7:
                    {
                    cout<<"Task 7"<<endl;
                    for (int i = 0 ; i <= 5 ; i++)
                    {
                    for(int j=0 ; j<= i ; j++)
                    {
                            if(i + j > 3)
                    {
                            cout<<"*";
                    }
                    }
                    cout<<endl;
                    }
                 default :
                   {
                    cout<<"invalid input"<<endl;
                   }

                    }
                    }
                break;

                case 'i':
                case 'I':
                    int task_choice1;
             cout<<"Enter 1 for in lab task 1"<<endl;
             cout<<"Enter 2 for in lab task 2"<<endl;
             cout<<"Enter 3 for in lab task 3"<<endl;
             cout<<"Enter 4 for in lab task 4"<<endl;
             cout<<"Enter 5 for in lab task 5"<<endl;
             cout<<"Enter 6 for in lab task 6"<<endl;
             cout<<"Enter 7 for in lab task 7"<<endl;
             cout<<"Enter 8 for in lab task 8"<<endl;
             cin>>task_choice1;

             switch(task_choice1)
             {
                case 1 :
                int i,j,rows;
                    cout<<"Please enter the number of rows"<<endl;
                    cin>>rows;
                    for(i=1; i<=rows; i++)
                    {
                    for(j=i; j<=rows; j++)
                    {
                   cout<<"*";
                    }

                   for(j=1; j<=(2*i-2); j++)
                    {
                   cout<<" ";
                    }
                   for(j=i; j<=rows; j++){
                   cout<<"*";
                    }
                   cout<<"\n";
                    }

                   for(i=1; i<=rows; i++){
                   for(j=1; j<=i; j++)
                   {
                   cout<<"*";
                   }

                   for(j=(2*i-2); j<(2*rows-2); j++)
                   {
                   cout<<" ";
                   }
                   for(j=1; j<=i; j++)
                    {
                   cout<<"*";
                    }
                   cout<<endl;
                }

                break;
                case 2:
                    {
                    int n, i , j;
                    cout << "Enter number of rows: ";
                    cin >> n;
                   for(i = 1; i <= n; i++)
                   {
                   for(j = 1; j <= i; j++)
                   {
                   cout<< "*";
                   }
                   cout<<"\n";
                   }
                   for(i = n; i >= 1; i--)
                   {
                   for(j = 1; j <= i; j++)
                   {
                   cout << "*" ;
                   }

                   cout<<"\n";

                   }

                   }
                   break;

                case 3:
                    {
                        int n, i, j;
                    cout << "Enter number of rows: ";
                    cin >> n;
                   for(i = 1; i <= n; i++)
                    {
                   for(j = i; j < n; j++)
                    {
                     cout << " ";
                    }
                   for(j = 1; j <= i; j++)
                    {
                    cout << "*";
                    }
                    cout << "\n";
                    }
                   for(i = n; i >= 1; i--)
                    {
                   for(j = i; j <= n; j++)
                    {
                    cout << " ";
                    }
                   for(j = 1; j < i; j++)
                    {
                   cout<<"*";
                    }
                   cout<<"\n";
                    }

                    }
                case 4:
                    {
                        int r, i, j, s;
                    cout << "Enter number of rows: ";
                    cin >> r;
                for(i = 1; i <= r; i++)
                {
                for (s = i; s < r; s++)
                cout << " ";
                for(j = 1; j <= (2 * r - 1); j++)
                {
                if(i == r || j == 1 || j == 2*i - 1)
                cout << "*";
                else
                cout << " ";
                }

                 cout << "\n";
                }

}
}
}
return 0;
}
