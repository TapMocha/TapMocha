local RE = game.ReplicatedStorage.RE
local giveCash = script.Parent
local leaderstats = Instance.new("leaderstats")
local player = game.Players.LocalPlayer

Cash.Name = "Cash"
Cash.Value = 0
Cash = Instance.new("Cash")

game.OnServerEvent:Connect(function()
   RE:FireClient()
end)

gui.Parent.MouseButton1Click:Connect(function(clicked)
   for i = Cash.Value, 1000 do
      if player.clicked.gui then
         task.wait(3)
         i + 10
         if i == 1000 then
            break or stop
         end
      end
   end
end)
return
