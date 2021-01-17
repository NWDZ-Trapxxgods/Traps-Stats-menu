# Traps-Stats-menu

1. GOTO Dayz_Code/init/compiles.sqf and add

player_onPause = compile preprocessFileLineNumbers "FG\stats\player_onPause.sqf";

in the if (!isDedicated) then { section

Then add 
#include "FG\stats\defines.hpp" If you dont have the defines already....
#include "FG\stats\statdefines.hpp" at the bottom of description.ext.

if you run KFC AH delete lines 208 and 209 and remove _escMidT from the top private[] section.

If you run Infistar remove 
					_btnRespawn = _display displayCtrl 1010;
					_btnRespawn ctrlShow true;
					_btnRespawn ctrlSetScale 0.9;
					if((canStand player) || (deathHandled))then
					{
						_btnRespawn ctrlEnable false;
						_btnRespawn ctrlSetText 'by infiSTAR.de';
					}
 from AH.sqf
