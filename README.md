# include <iostream>
#include <vector>

using namespace std;

int main() {
    int n;
    cout << "Neçə ədəd daxil edəcəksiniz? ";
    cin >> n;

    if (n <= 0) {
        cout << "Ədədlərin sayı müsbət olmalıdır." << endl;
        return 1;
    }

    vector<double> ededler(n);
    double cemi = 0.0;

    cout << "Ədədləri daxil edin:" << endl;
    for (int i = 0; i < n; ++i) {
        cin >> ededler[i];
        cemi += ededler[i];
    }

    double ededi_orta = cemi / n;

    cout << "Ədədlərin ədədi ortası: " << ededi_orta << endl;

    return 0;
}
