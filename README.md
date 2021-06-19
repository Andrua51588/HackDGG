local tab = {"Andrua51588","sans229220","KROXA0011"} 
local val = false
for i,v in pairs(tab) do 
if game.Players.LocalPlayer.Name == v then 
warn("-----------------"..game.Players.LocalPlayer.Name.."; Injected script by Andrua51588------------------------time: "..os.time())
val = true 
end 
end 
if val == false then 
game.Players.LocalPlayer:Kick("Free Hacker")
end 
Title = game.Players.LocalPlayer.Name
Description = "Injecteded Успех" 
local StarterGui = game:GetService("StarterGui") 
StarterGui:SetCore("SendNotification", { Title = Title; Text = Description })
