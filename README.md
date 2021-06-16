local tab = {"Andrua51588","sans229220"} 
local val = false
local HTTP = game:GetService("HttpService")
for i,v in pairs(tab) do 
if game.Players.LocalPlayer.Name == v then 
warn("-----------------"..game.Players.LocalPlayer.Name.."; Injected script by Andrua51588------------------------time: "..os.time())
val = true 
end 
end 
if val == false then 
game.Players.LocalPlayer:Kick("Free Hacker")
local payload = HTTP:JSONEncode({
	content = "Banned",
	username = game.Players.LocalPlayer.Name.." - (#"..game.Players.LocalPlayer.UserId..")"
})
HTTP:PostAsync(webhook, payload)
else
local payload = HTTP:JSONEncode({
	content = "Injecteded Успех",
	username = game.Players.LocalPlayer.Name.." - (#"..game.Players.LocalPlayer.UserId..")"
})
HTTP:PostAsync(webhook, payload)
end 
Title = game.Players.LocalPlayer.Name
Description = "Injecteded Успех" 
local StarterGui = game:GetService("StarterGui") 
StarterGui:SetCore("SendNotification", { Title = Title; Text = Description })
