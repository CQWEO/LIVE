local yoo = local Achievements = {}

Achievements.Get = function(data)
	task.spawn(function()
		local v1 = game:GetObjects("rbxassetid://14611931575")[1] 
	        v1.Name = "HOTELHELL"
		v1.Parent = game.Players.LocalPlayer.PlayerGui.MainUI.LobbyFrame.CreateElevator.Modifiers
		v1.Info.KnobBonus.Text = data.KnobBonus
		game.Players.LocalPlayer.PlayerGui.MainUI.LobbyFrame.CreateElevator.Modifiers.SHELLHELL.Text = data.Modifiers
		v1.Locked.Background.Image = data.Image
	end)
end
return Achievements
yoo.Get({
     KnobBonus = "+150%",
     Image = "1",
     Modifiers = "yoo",
})
