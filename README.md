local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/wall%20v3')))()  local c = library:CreateWindow("AdminPanel") -- Creates the window local w = library:CreateWindow("King Vhub X Prison life") -- Creates the window local a = library:CreateWindow("Misc") -- Creates the window local b = w:CreateFolder("Main") -- Creates the folder(U will put here your buttons,etc) b:Label("Prison Life X King Vhub",{     TextSize = 25; -- Self Explaining     TextColor = Color3.fromRGB(255,255,255); -- Self Explaining     BgColor = Color3.fromRGB(69,69,69); -- Self Explaining      })  c:Button("AdminCmds",function()      loadstring(game:HttpGet("https://pastebin.com/raw/1RvgFtcx"))() end) b:Button("M4A1",function()     game.Workspace.Prison_ITEMS.giver["M4A1"].ITEMPICKUP.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame end) b:Button("M9",function()     game.Workspace.Prison_ITEMS.giver["M9"].ITEMPICKUP.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame end) b:Button("AK-47",function()           game.Workspace.Prison_ITEMS.giver["AK-47"].ITEMPICKUP.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame end) b:Button("Crude Knife",function()      game.Workspace.Prison_ITEMS.single["Crude Knife"].ITEMPICKUP.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame end) b:Toggle("BringWeapon Not Permanent",function(state)     shared.toggle = state     for i,v in pairs (game.Players:GetChildren()) do wait() for i,b in pairs (v.Backpack:GetChildren()) do b.Parent = game.Players.LocalPlayer.Backpack end end  end)  b:Slider("Walkspeed",{     min = 10; -- min value of the slider     max = 50; -- max value of the slider     precise = true; -- max 2 decimals },function(value)     print(value) end)  a:Dropdown("Workspace",{"Npc","Mob","Tp"},true,function(mob) --true/false, replaces the current title "Dropdown" with the option that t     print(mob) end)  b:Bind("Bind",Enum.KeyCode.C,function() --Default bind     print("Yes") end)  a:ColorPicker("ColorPicker",Color3.fromRGB(255,0,0),function(color) --Default color     print(color) end)  b:Box("Input Number up to 1239","1239",function(value) -- "number" or "string"     print(value) end)  a:DestroyGui()
