// bruteforce approach using xor time complexity O(n)
#include <bits/stdc++.h>
using namespace std;

int singleNonDuplicate(vector<int>& arr) {
    int n = arr.size(); //size of array.
    int ans = 0;
    // XOR all the elements:
    for (int i = 0; i < n; i++) {
        ans = ans ^ arr[i];
    }
    return ans;
}

int main()
{
    vector<int>array = {1, 1, 2, 2, 3, 3, 4, 5, 5, 6, 6};
    int ans = singleNonDuplicate(array);
    cout << "The single element is: " << ans << "\n";
    return 0;
}
// optimal approach using binary search time complexity-O(logn)
  int n = arr.size();
    int low = 0, high = n - 1, mid;

    // Do binary search
    while (low < high) {

        // Calculate mid
        mid = low + (high-low) / 2;

        // Update low and high
        if ((mid % 2 == 1 && arr[mid] == arr[mid - 1]) || (mid % 2 == 0 && arr[mid] == arr[mid + 1]))
        {
            low = mid + 1;
        }
        else
        {
            high = mid;
        }
    }

    return arr[low];


    }
};
