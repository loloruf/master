# master
playing around

#include<iostream>
#include<vector>
#include<algorithm>
using namespace std;

vector<int> vec; 

void print()
{
    //for(int i=0; i<vec.size(); i++)
    //    cout << vec[i] << " ";
    for(vector<int>::iterator it = vec.begin(); it != vec.end(); it++)
        cout << *it << "\t";
    cout << endl;
}

int main()
{

    for(int i = 1; i < 5 ; i++) { 
        vec.push_back(i); 
        cout << vec[i-1] << "\t";
    }

    cout << endl;

    while(next_permutation(vec.begin(), vec.end()) ){
        print();
        // do some processing on vec
    }

    return 0;
}
