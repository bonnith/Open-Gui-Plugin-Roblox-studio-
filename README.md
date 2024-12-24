This all for roblox studio, all write with lua code, for someone who too lazy to create open gui script this module and plugin will does great help to you, anyway this module still v0.1 can't do much thing

use Play to open ui with tween
use Back to close ui with tween
 	
 	create an frame, open plugin click {create Start} to set startposition
 	and then click {Set end} to set last position,size,rotation at last
 	and use reset to move ui to start
 	
 	:::script:::
 	local gui_tweener = require(game.ReplicatedStorage.GuiTweener)
 	
	local frame = bla bla bla
	local button = bla bla bla
	
	--to open
	button.MouseButton1Click:Connect(function()
		local stage = gui_tweener.GetStage(frame)
		if stage == "Close" then
			gui_tweener.Play(frame)
		elseif stage == "Open" then
			gui_tweener.Back(frame)
		end
	end)
	
	-- or
	tweener.Toggle(frame,button,
	function() --- when open function
		
	end,
	function() --- when close function
		
	end)


 
