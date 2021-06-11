#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main()
{
    srand((unsigned)time(0));
    int x;
    int numarRandom = (rand() % 10);
    cin >> x;

    if (numarRandom == x){
        cout << "Bravo!!! \n"; return 0;}

    if (x + 1 / 2 * x <= numarRandom){
        cout << "Aproape, prea putin \n\n";}
    if (x - 1 / 2 * x >= numarRandom){
        cout << "Aproape, prea mult \n\n";}


/*    if ((numarRandom - 3 / 10 * numarRandom <= x) || (numarRandom + 3 / 10 * numarRandom >= x)){
        cout << "Aproape \n";}

    if (((x - 1 / 2 * x <= numarRandom) && (x - 3 / 10 * x >= numarRandom)) || ((x + 3 / 10 * x <= numarRandom) && (x + 1 / 2 * x >= numarRandom))){
        cout << "Departe \n";}
*/

    cout << "Numarul era: \n" << numarRandom << endl;


    return 0;
}
