// ok so, what i learnt new thing is about vectors

/*Vectors are resizable arrays, and is a data structure and we can add and eliminate an element from its
end, vectors are first included as a library like #include <vector

to add an element we can use push_back() function*/

#include <vector>
#include <iostream>
using namespace std;

class Solution {
public:
    vector<vector<int>> countFrequencies(vector<int>& nums) {
        //making an hash arrays
        int hash[13]={0}; //here all the values of this hash are considered to be zero
        
        for (int q: nums){
            hash[q]++; //here we r incrementing the values of this hash whenvr the nums element occurs
        }
        
        vector<vector<int>> result;
        
        for (int i=0;i<13;i++){
            if(hash[i]>0){
                result.push_back({i,hash[i]}); //here we will push te elements as lists with num ele, frequency
            }
        }
        
        return result;
    }
};

int main(){
    vector<int> q={1,2,2,1,3};
    
    Solution s1;
    vector<vector<int>> nm = s1.countFrequencies(q);
    for (auto &row : nm) {
        cout << row[0] << " -> " << row[1] << endl;
    }
}
