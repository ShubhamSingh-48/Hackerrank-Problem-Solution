# Hackerrank-Problem-Solution
Here you will got Hackerrank Problem Solution 

Array Revesal Problem. ![Screenshot (678)](https://user-images.githubusercontent.com/88249319/190874657-d11a6967-f9a9-4f9d-8263-c6763bb23953.png)



#include <iostream>
using namespace std;
int main()
{
    int n;
    int arr[1000];
    cout << "Enter size of array: ";
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> arr[i];
    }
    cout << "Our array is" << endl;
    for (int i = 0; i < n; i++)
    {
        cout << arr[i] << " ";
    }
    int start = 0;
    int end = n - 1;
    while (start <= end)
    {
        swap(arr[start], arr[end]);
        start++;
        end--;
    }
    cout << "Reversed array is" << endl;
    for (int i = 0; i < n; i++)
    {
        cout << arr[i] << " ";
    }
}
