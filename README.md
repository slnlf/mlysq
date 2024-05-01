
-- First create a part and call it "Button"
-- MAKE SURE TO CHANGE THE NAME IF YOUR PART IS CALLED OTHER THAN "Button" !!


local  Button = game.Workspace.Button
Button.Touched:Connect(function(otherPart)  -- connect the button to the otherpart which could be the player/player's part
 
local humanoid = otherPart.Parent:FindFirstChild("Humanoid")  -- the humanoid variable is the player/player's parts
 
	if humanoid then   -- " if it's player's part"
		humanoid.Health = 0  -- "kill the player"
	end
end)
 
-- @mlysq on yt
