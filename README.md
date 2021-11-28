# Lecture-13-Codes


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



---

    #include <iostream>
    #include <array>
    using namespace std;
    int main()
    {
      array<string, 4> arr = { "Mars Bar", "Snickers", "Bounty", "Wispa"};
      cout << arr.at(1) << endl;
      cout << arr[1] << endl;

      cout << arr.front()<< endl;
      cout << arr.back()<< endl;

      for (int i = 0; i < arr.size(); i++) {
        cout << arr.at(i) << ", ";
      }
      cout << endl;
    }


---

    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      array<int, 5> numbers = { 33, 5, 7, 99, 83 };
      sort(numbers.begin(), numbers.end());
      for (int num : numbers) {
        cout << num << " ";
      }

    }


---
  
    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      array<int, 5> numbers = { 33, 5, 7, 99, 83 };
      sort(numbers.begin(), numbers.end());
      reverse(numbers.begin(), numbers.end());
      for (int num : numbers) {
        cout << num << " ";
      }

    }

  
rand function
  
    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      int randomArray[10];
      for (int i = 0; i < 10; i++) 
      {
        randomArray[i] = rand() % 50;
        cout << randomArray[i] << endl;
      }

    }
    
    
Exercise (1)

    #include <iostream>
    #include<array>
    #include <algorithm>
    using namespace std;
    int main()
    {
      int randomArray[1000];
      int counter = 0;
      for (int i = 0; i < 1000; i++) 
      {
        randomArray[i] = rand() % 100;
        cout << randomArray[i] << endl;

        if (randomArray[i] == 6)
        {
          counter++;
        }
      }
      cout << "6 appeared " << counter << "x" << endl;

    }



Exercise (2)



Exercise (3)


















