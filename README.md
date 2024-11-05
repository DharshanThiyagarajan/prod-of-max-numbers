# prod-of-max-numbers # cpp
#include <iostream>
using namespace std;
int main()
{
    int a;
    cin>>a;
    int r[a];
    for (int i=0;i<a;i++)
    {
        cin>>r[i];
    }
    int max=r[0];
    int smax;
    for (int i=1;i<a;i++)
    {
        if (r[i]>max)
        {
            smax=max;
            max=r[i];
        }
    }
    cout<<max*smax;
    return 0;
}
