#include <iostream>
#include <raylib.h>

using namespace std;

// blanco scherm maken
int main()
{
    cout<< "START GAME" << endl;
const int scherm_breedte = 1280;
const int schermm_hoogte = 800; 
    InitWindow(scherm_breedte, schermm_hoogte, "naam van onze game");
    SetTargetFPS(60);

    // game loop maken
    while(WindowShouldClose() == false)
     {
        BeginDrawing();

        //tekening maken
        Drawline(scherm_breedte/2, 0, scherm_breedte/2, schermm_hoogte, GREEN)
        DrawCircle(scherm_breedte/2, schermm_hoogte/2, 20, YELLOW); /*tekent een pingponh bal*/
        DrawRectangle(10, schermm_hoogte/2 - 60, 25, 120, RED); /* tekent van de rechter paddle en kleur aangeven*/
        DrawRectangle(scherm_breedte/2 - 35, schermm_hoogte/2 - 60, 25, 120, RED); /* tekent van de linker paddle en kleur aangeven*/
        EndDrawing();
    }

    CloseWindow()
    return 0;
}
