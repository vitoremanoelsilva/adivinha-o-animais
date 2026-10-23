#include <iostream>
#include <string>
#include <limits> 
using namespace std;

void limparTela() {
    cout << "\033[2J\033[H"; 
}

bool perguntar(const string& pergunta) {
    string resposta;
    cout << "\n----------------------------------------\n";
    cout << pergunta << " (sim/nao): ";
    cin >> resposta;

    cin.ignore(numeric_limits<streamsize>::max(), '\n');

    return (!resposta.empty() && (resposta[0] == 's' || resposta[0] == 'S'));
}

int main() {
    char jogarNovamente;

    do {
        limparTela();
        cout << "========================================\n";
        cout << "  JOGO DOS ANIMAIS - ADIVINHE O ANIMAL\n";
        cout << "========================================\n";
        cout << "Pense em um animal da lista:\n";
        cout << "Leao, Baleia, Tartaruga, Cavalo, Avestruz,\n";
        cout << "Crocodilo, Homem, Pinguim, Cobra, Macaco,\n";
        cout << "Pato, Iguana, Morcego, Aguia, Panda\n\n";
        cout << "Pressione ENTER para comecar...";
        cin.get(); // Espera o usuário apertar Enter

        string animal = "DESCONHECIDO";

        // perguntas
        
        limparTela();
        bool mamifero = perguntar("E mamifero?");

        limparTela();
        bool quadrupede = perguntar("E quadrupede?");

        limparTela();
        bool carnivoro = perguntar("E carnivoro?");

        limparTela();
        bool herbivoro = perguntar("E herbivoro?");

        limparTela();
        bool voador = perguntar("E voador?");

        limparTela();
        bool terrestre = perguntar("E terrestre?");

        // animais

        if (mamifero && quadrupede && carnivoro && !herbivoro && !voador && terrestre) {
            animal = "Leao";
        } 
        else if (mamifero && quadrupede && !carnivoro && herbivoro && !voador && terrestre) {
            animal = "Cavalo ou Panda";
        } 
        else if (mamifero && !quadrupede && !carnivoro && !herbivoro && !voador && terrestre) {
            animal = "Homem ou Macaco";
        } 
        else if (mamifero && !quadrupede && carnivoro && !herbivoro && voador && !terrestre) {
            animal = "Morcego";
        } 
        else if (mamifero && !quadrupede && carnivoro && !herbivoro && !voador && !terrestre) {
            animal = "Baleia";
        } 
        else if (!mamifero && quadrupede && !carnivoro && herbivoro && !voador && terrestre) {
            animal = "Tartaruga ou Iguana";
        } 
        else if (!mamifero && quadrupede && carnivoro && !herbivoro && !voador && terrestre) {
            animal = "Crocodilo";
        } 
        else if (!mamifero && !quadrupede && !carnivoro && herbivoro && !voador && terrestre) {
            animal = "Avestruz";
        } 
        else if (!mamifero && !quadrupede && !carnivoro && herbivoro && voador && !terrestre) {
            animal = "Pato";
        } 
        else if (!mamifero && !quadrupede && carnivoro && !herbivoro && voador && !terrestre) {
            animal = "Aguia";
        } 
        else if (!mamifero && !quadrupede && carnivoro && !herbivoro && !voador && terrestre) {
            animal = "Cobra";
        } 
        else if (!mamifero && !quadrupede && carnivoro && !herbivoro && !voador && !terrestre) {
            animal = "Pinguim";
        }

        // resultado
        limparTela();
        cout << "========================================\n";
        if (animal == "DESCONHECIDO")
            cout << " Nao consegui identificar o animal. :(\n";
        else if (animal.find("ou") != string::npos)
            cout << " O animal que voce pensou foi: " << animal << "!\n (As respostas empataram para esses dois)\n";
        else
            cout << " O animal que voce pensou foi: " << animal << "!\n";
        
        cout << "========================================\n";

        cout << "\nDeseja jogar novamente? (s/n): ";
        cin >> jogarNovamente;
        cin.ignore(numeric_limits<streamsize>::max(), '\n');

    } while (jogarNovamente == 's' || jogarNovamente == 'S');

    cout << "\nObrigado por jogar!\n";
    return 0;
}