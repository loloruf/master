# master
playing around

#include <fstream>
#include <iostream>
#include <vector>
using namespace std;

#include <keepr.h>

int main() {
    keepr dontstop;
    vector<string> list;

    string word;
    ifstream wordfile("dic.dat");
    while (infile >> word) {
        list.push_back(word);
    }

    for (unsigned n=0; n<list.size(); ++n) {
        cout << list.at( n ) << " ";
    }
    return 0;
}
