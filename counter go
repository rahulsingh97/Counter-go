
--[[
CS:GO No-Recoil

- For Logitech Game Software:		TO DO
400 DPI 
1000 HZ

- For Windows:						TO DO
Sensitivity: 6
Pointer Precision: OFF

- For CS:GO:						TO DO
Aspect Ratio: 16:9
Sensitivity: 3.09
Raw Input: ON
Mouse Acceleration: OFF

Weapon Supported: AK47/M4A1-S
--]]
local Activation_Key = 9 -- this is the activation key with 3 modes 1-"T:AK47" 2-"CT:M4A1-S" 3-"OFF"
OutputLogMessage("WELCOME press the \"%d\" key on mouse to shuffel through T, CT & OFF\n",Activation_Key);

local AK47_Pattern = { 
   { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 5 }, { x = 0, y = 6 }, { x = 0, y = 7 }, { x = 0, y = 7 }, { x = 0, y = 8 }, { x = 0, y = 7 }, { x = 0, y = 6 }, { x = 0, y = 7 }, { x = 0, y = 8 }, { x = -2, y = 8 }, { x = 1, y = 7 }, { x = 3, y = 7 }, { x = 6, y = 7 }, { x = 6, y = 7 }, { x = 6, y = 7 }, { x = 0, y = 7 }, { x = 1, y = 7 }, { x = 2, y = 7 }, { x = 2, y = 8 }, { x = 2, y = 8 }, { x = 2, y = 9 }, { x = -3, y = -4 }, { x = -8, y = -1 }, { x = -15, y = -1 }, { x = -15, y = -1 }, { x = -5, y = 0 }, { x = -5, y = 0 }, { x = -5, y = 0 }, { x = -5, y = 0 }, { x = -1, y = 1 }, { x = 4, y = 2 }, { x = 4, y = 2 }, { x = 5, y = 1 }, { x = -5, y = 1 }, { x = -5, y = 1 }, { x = -10, y = 1 }, { x = -10, y = 0 }, { x = -5, y = 0 }, { x = -3, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 1 }, { x = 0, y = 1 }, { x = -2, y = 1 }, { x = 6, y = 1 }, { x = 8, y = 2 }, { x = 14, y = 2 }, { x = 15, y = 2 }, { x = 1, y = 2 }, { x = 1, y = 2 }, { x = 1, y = 1 }, { x = 1, y = 1 }, { x = 5, y = 1 }, { x = 6, y = 1 }, { x = 6, y = 1 }, { x = 6, y = 1 }, { x = 6, y = -1 }, { x = 10, y = -1 }, { x = 10, y = -2 }, { x = 10, y = -3 }, { x = 0, y = -5 }, { x = 0, y = 0 }, { x = -5, y = 0 }, { x = -5, y = 0 }, { x = -5, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 1 }, { x = 0, y = 2 }, { x = 0, y = 1 }, { x = 0, y = 1 }, { x = 0, y = 2 }, { x = 0, y = 2 }, { x = 0, y = 1 }, { x = 0, y = 1 }, { x = 3, y = 1 }, { x = 3, y = -1 }, { x = 3, y = -1 }, { x = 0, y = 0 }, { x = -3, y = 0 }, { x = -4, y = 0 }, { x = -4, y = 0 }, { x = -4, y = 0 }, { x = -4, y = 0 }, { x = -4, y = 0 }, { x = -7, y = 0 }, { x = -7, y = 0 }, { x = -8, y = 0 }, { x = -8, y = -2 }, { x = -15, y = -3 }, { x = -16, y = -5 }, { x = -18, y = -7 }, { x = 0, y = 0 }, { x = 0, y = 0 },}
local MAC10_Pattern = { 
   { x = 0, y = 1 }, { x = 0, y = 2 }, { x = 0, y = 2 }, { x = 0, y = 2 }, { x = 0, y = 2 }, { x = 0, y = 2 }, { x = 0, y = 3 }, { x = 2, y = 5 }, { x = 3, y = 6 }, { x = 4, y = 6 }, { x = 4, y = 6 }, { x = 4, y = 6 }, { x = 4, y = 6 }, { x = 4, y = 6 }, { x = 0, y = 6 }, { x = 0, y = 6 }, { x = -2, y = 6 }, { x = -2, y = 6 }, { x = 1, y = 5 }, { x = 3, y = 5 }, { x = 3, y = 5 }, { x = 3, y = 4 }, { x = 1, y = 2 }, { x = 1, y = 1 }, { x = -2, y = 2 }, { x = -2, y = 2 }, { x = -2, y = 2 }, { x = -2, y = 1 }, { x = -1, y = 1 }, { x = -1, y = 1 }, { x = -1, y = 0 }, { x = -1, y = 1 }, { x = -3, y = 1 }, { x = -5, y = -1 }, { x = -5, y = -1 }, { x = -6, y = -1 }, { x = -7, y = 2 }, { x = -8, y = 2 }, { x = -2, y = 2 }, { x = -2, y = 0 }, { x = -2, y = 0 }, { x = -1, y = 0 }, { x = -1, y = 0 }, { x = -1, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = -3, y = 0 }, { x = -5, y = 0 }, { x = -8, y = 0 }, { x = -4, y = 0 }, { x = 0, y = 0 }, { x = 3, y = 0 }, { x = 6, y = 0 }, { x = 6, y = 0 }, { x = 6, y = 0 }, { x = 6, y = 0 }, { x = 3, y = 0 }, { x = 2, y = 0 }, { x = 3, y = 0 }, { x = 5, y = 0 }, { x = 4, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 }, { x = 0, y = 0 },}
local function OutputLogs(act)
   if act == 1 then
      OutputLogMessage("T: AK47\n");
   elseif act == 2 then
      OutputLogMessage("CT: M4A1-S\n");
   else
      OutputLogMessage("OFF\n");
   end
end
local Spray_Randomize = math.random(29,31)
local Recoil_Activator = 0
EnablePrimaryMouseButtonEvents(true);
function OnEvent(event, arg)
--OutputLogMessage("Button  = %d\n", arg)    --uncomment me to see the button presed in outputlog
   if (event == "MOUSE_BUTTON_PRESSED" and arg == Activation_Key) then
      if Recoil_Activator >= 3 then Recoil_Activator = 0 end
      Recoil_Activator = Recoil_Activator + 1
	  OutputLogs(Recoil_Activator)
   end
   if Recoil_Activator == 1 then
      if IsMouseButtonPressed(1) then
         for i = 1, #AK47_Pattern do
            if IsMouseButtonPressed(1) then
               Sleep(Spray_Randomize)
               MoveMouseRelative( AK47_Pattern[i].x, AK47_Pattern[i].y )
OutputLogMessage("X = %d", AK47_Pattern[i].x);
OutputLogMessage("Y = %d\n", AK47_Pattern[i].y );
            end
         end
      end
   elseif Recoil_Activator == 2 then
      if IsMouseButtonPressed(1) then
         for i = 1, #MAC10_Pattern do
            if IsMouseButtonPressed(1) then
               Sleep(Spray_Randomize)
               MoveMouseRelative( MAC10_Pattern[i].x, MAC10_Pattern[i].y )
OutputLogMessage("X = %d", MAC10_Pattern[i].x);
OutputLogMessage("Y = %d\n", MAC10_Pattern[i].y );
            end
         end
      end
   else
   end
end
