# Traps-Stats-menu

1. GOTO Dayz_Code/init/compiles.sqf and add

player_onPause = compile preprocessFileLineNumbers "FG\stats\player_onPause.sqf";

in the if (!isDedicated) then { section

Then add 
#include "FG\stats\defines.hpp" If you dont have the defines already....
#include "FG\stats\statdefines.hpp" at the bottom of description.ext
