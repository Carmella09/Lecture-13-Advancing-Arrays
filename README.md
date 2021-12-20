# Lecture-13-Codes

//EXERCISES

Input/Output Array
Write a program that puts 5 integer values provided by the user into an array. Then output these values to the console.

        #include <iostream>
        #include <string>
        using namespace std;
        int main()
        {
            int courses[5];

            for (int i = 0; i < 5; i++) {
                cout << "\nEnter the " << i + 1 << " number: " ;
                cin >> courses[i];
                while (cin.fail()) {
                    cout << "\nInvalid Input" << endl;
                    cout << "Enter the number again: ";
                    cin.clear();
                    cin.ignore();
                    cin >> courses[i];
                }
            }
            cout << "\nOutput: \n\n";
            for (auto course : courses) {
                cout << course << endl;
            }
        }


Array Art

    #include <iostream>
    using namespace std;
    int main()
    {
      string snacks[5][5] = 
      {
      {"_"," ","_"," ","_"}, 
      {"_", "O", "_", "O", "_"}, 
      {"_", "@", "@", "@", "_"},
      {"_", "^", "^", "^", "_"}, 
      {"_", "V", "V", "V","_" } 
      };

      for (int i = 0; i < 5; i++)
      {
        cout << endl;
        for (int j = 0; j < 5; j++) 
        {
          cout << snacks[i][j];
        }
      }
      cout << endl;
    }

//NOT EXERCISE

Range Based for Loop

    #include <iostream>
    using namespace std;
    int main()
    {
    string courses[] = { "BSU CC", "BSU BA", "HNC CC", "HND" };

      for (int i = 0; i < 4; i++) {
        cout << courses[i] << endl;}

      for (auto course: courses) {
        cout << course << endl;
      }
    }


Auto Keyword
                          
    #include <iostream>
    using namespace std;
    int main()
    {
      char letters[] = { 'C', 'o', 'd', 'e', 'L', 'a', 'b' };
      for (auto letter : letters) {

        cout << letters << endl;}
    }


Multidimensional Arrays
  
2DArray 

2DArray Initialisation

      #include <iostream>
      using namespace std;
      int main()
      {
        string snacks[3][4] = {
        {"Galaxy silk", "Mars Bar", "Snickers","Bounty"},
        {"Flavoured Youghurt", "Oman chips","Oreo,Lays"},
        {"Apple", "Banana","Orange","Pear"}
        };
        cout << snacks[1][2] << endl;

      }


Accessing 2D Array Values

    #include <iostream>
    using namespace std;
    int main()
    {
        string snack[3][4] =
        {
          {"Galaxy silk", "Mars Bar", "Bounty"},
          {"Flavoured Youghurt", "Oman chips", "Oreo", "Lays"},
          {"Apple", "Banana", "Orange", "Pearl"}
        };

        for (int i = 0; i < 3; i++)
        {
          for (int j = 0; j < 4; j++)
          {
            cout << snack[i][j] << " ";
          }
          cout << endl;
        }

      }




 














