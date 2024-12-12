--discord.gg/boronide, code generated using luamin.js™




local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Iamkhnah/a__TDT_script/refs/heads/main/NewLibraryUi.lua"))()

local ScreenGui = Instance.new("ScreenGui")
local ImageLabel = Instance.new("ImageButton")
local UICorner = Instance.new("UICorner")

-- Properties

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ImageLabel.Parent = ScreenGui
ImageLabel.BackgroundColor3 = Color3.new(1, 1, 1)
ImageLabel.BorderColor3 = Color3.new(0, 0, 0)
ImageLabel.BorderSizePixel = 0
ImageLabel.Position = UDim2.new(0.394522578, 0, 0.336561739, 0)
ImageLabel.Size = UDim2.new(0, 70, 0, 70)
ImageLabel.Image = "http://www.roblox.com/asset/?id=137105861382234"
ImageLabel.Draggable = true
ImageLabel.MouseButton1Down:Connect(function()
	library:ToggleUi()
end)


UICorner.Parent = ImageLabel
UICorner.CornerRadius = UDim.new(1, 0)

--Create Tabs
local Win = library:Evil()
local Tab8 = Win:Tab("Status Server", 14477673361)
local Tab = Win:Tab("Main", 14477284625)
local Tab2 = Win:Tab("Others Farm", 14477543197)
local Tab3 = Win:Tab("Players - Travel", 14477517268)
local Tab4 = Win:Tab("Fruits - Raids", 14537413902)
local Tab5 = Win:Tab("Race V4", 14477598542)
local Tab6 = Win:Tab("Sea Events", 14477621526)
local Tab7 = Win:Tab("Shops - Miscs", 14477663692)
-------------------------------------------------------------------------------------------------------------------------------------------
--Status
local Sta = Tab8:CraftPage(1)
local Sta2 = Tab8:CraftPage(2)
--Main
local Main = Tab:CraftPage(1)
local Setting = Tab:CraftPage(2)
--Others Farm
local Farm = Tab2:CraftPage(1)
local Farm2 = Tab2:CraftPage(2)
--Players - Teleport
local Player = Tab3:CraftPage(1)
local Teleport = Tab3:CraftPage(2)
--Fruits - Raids
local Fruit = Tab4:CraftPage(1)
local Raid = Tab4:CraftPage(2)
--Race V4
local Race = Tab5:CraftPage(1)
local Race2 = Tab5:CraftPage(2)
--Sea Events
local Sea = Tab6:CraftPage(1)
local Sea2 = Tab6:CraftPage(2)
--Shops - Miscs
local S = Tab7:CraftPage(1)
local M = Tab7:CraftPage(2)
-------------------------------------------------------------------------------------------------------------------------------------------
--Musics
pcall(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.Sound:Destroy()
end)
local ContentProvider = Game:GetService("ContentProvider")
local sound = Instance.new("Sound")
sound.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
while (ContentProvider.RequestQueueSize > 0) do
	wait()
end
if game.Players.LocalPlayer.Character.Humanoid.Health <= 0 then
	game.Players.LocalPlayer.Character.HumanoidRootPart.Sound:Destroy()
	wait(5)
	local ContentProvider = Game:GetService("ContentProvider")
	local sound = Instance.new("Sound")
	sound.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
	while (ContentProvider.RequestQueueSize > 0) do
		wait()
	end
end
local plr = game.Players.LocalPlayer
local RadientPaid = {}
local UserInputService = game:GetService("UserInputService")
local TweenService = game:GetService("TweenService")
local RunService = game:GetService("RunService")
local LocalPlayer = game:GetService("Players").LocalPlayer
local Mouse = LocalPlayer:GetMouse()
local HttpService = game:GetService("HttpService")
local pfp
local userww
local tag
local userinfo = {}
pcall(function()
	userinfo = HttpService:JSONDecode(readfile("Radient.txt"));
end)
pfp = userinfo["pfp"] or "https://www.roblox.com/headshot-thumbnail/image?userId=" .. game.Players.LocalPlayer.UserId .. "&width=420&height=420&format=png"
user =  userinfo["user"] or game.Players.LocalPlayer.Name
tag = userinfo["tag"] or tostring(math.random(1, 10))
local function SaveInfo()
	userinfo["pfp"] = pfp
	userinfo["user"] = user
	userinfo["tag"] = tag
	writefile("Radient.txt", HttpService:JSONEncode(userinfo));
end
--Part
spawn(function()
	while wait() do
		pcall(function()
			if game.Players.LocalPlayer.Character.Humanoid.Health <= 0 or not plr.Character:FindFirstChild("HumanoidRootPart") then
				if game.Players.LocalPlayer.Character:FindFirstChild("PartTele") then
					game.Players.LocalPlayer.Character:FindFirstChild("PartTele"):Destroy()
				end
			end
		end)
	end
end)
spawn(function()
	while wait() do
		pcall(function()
			if game.Players.LocalPlayer.Character:FindFirstChild("PartTele") then
				if (plr.Character.HumanoidRootPart.Position - plr.Character:FindFirstChild("PartTele").Position).Magnitude >= 100 then
					game.Players.LocalPlayer.Character:FindFirstChild("PartTele"):Destroy()
				end
			end
		end)
	end
end)
--Check World
local placeId = game.PlaceId
if placeId == 2753915549 then
	First_Sea = true
elseif placeId == 4442272183 then
	Second_Sea = true
elseif placeId == 7449423635 then
	Third_Sea = true
else
	game.Players.LocalPlayer:Kick("Support only Blox Fruits")
end
--CheckQuest
function CheckLevel()
	local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
	if First_Sea then
		if Lv == 1 or Lv <= 9 or SelectMonster == "Bandit" or SelectArea == '' then -- Bandit
			Ms = "Bandit"
			NameQuest = "BanditQuest1"
			QuestLv = 1
			NameMon = "Bandit"
			CFrameQ = CFrame.new(1060.9383544922, 16.455066680908, 1547.7841796875)
			CFrameMon = CFrame.new(1038.5533447266, 41.296249389648, 1576.5098876953)
		elseif Lv == 10 or Lv <= 14 or SelectMonster == "Monkey" or SelectArea == 'Jungle' then -- Monkey
			Ms = "Monkey"
			NameQuest = "JungleQuest"
			QuestLv = 1
			NameMon = "Monkey"
			CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
			CFrameMon = CFrame.new(-1448.1446533203, 50.851993560791, 63.60718536377)
		elseif Lv == 15 or Lv <= 29 or SelectMonster == "Gorilla" or SelectArea == 'Jungle' then -- Gorilla
			Ms = "Gorilla"
			NameQuest = "JungleQuest"
			QuestLv = 2
			NameMon = "Gorilla"
			CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
			CFrameMon = CFrame.new(-1142.6488037109, 40.462348937988, -515.39227294922)
		elseif Lv == 30 or Lv <= 39 or SelectMonster == "Pirate" or SelectArea == 'Buggy' then -- Pirate
			Ms = "Pirate"
			NameQuest = "BuggyQuest1"
			QuestLv = 1
			NameMon = "Pirate"
			CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
			CFrameMon = CFrame.new(-1201.0881347656, 40.628940582275, 3857.5966796875)
		elseif Lv == 40 or Lv <= 59 or SelectMonster == "Brute" or SelectArea == 'Buggy' then -- Brute
			Ms = "Brute"
			NameQuest = "BuggyQuest1"
			QuestLv = 2
			NameMon = "Brute"
			CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
			CFrameMon = CFrame.new(-1387.5324707031, 24.592035293579, 4100.9575195313)
		elseif Lv == 60 or Lv <= 74 or SelectMonster == "Desert Bandit" or SelectArea == 'Desert' then -- Desert Bandit
			Ms = "Desert Bandit"
			NameQuest = "DesertQuest"
			QuestLv = 1
			NameMon = "Desert Bandit"
			CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
			CFrameMon = CFrame.new(984.99896240234, 16.109552383423, 4417.91015625)
		elseif Lv == 75 or Lv <= 89 or SelectMonster == "Desert Officer" or SelectArea == 'Desert' then -- Desert Officer
			Ms = "Desert Officer"
			NameQuest = "DesertQuest"
			QuestLv = 2
			NameMon = "Desert Officer"
			CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
			CFrameMon = CFrame.new(1547.1510009766, 14.452038764954, 4381.8002929688)
		elseif Lv == 90 or Lv <= 99 or SelectMonster == "Snow Bandit" or SelectArea == 'Snow' then -- Snow Bandit
			Ms = "Snow Bandit"
			NameQuest = "SnowQuest"
			QuestLv = 1
			NameMon = "Snow Bandit"
			CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
			CFrameMon = CFrame.new(1356.3028564453, 105.76865386963, -1328.2418212891)
		elseif Lv == 100 or Lv <= 119 or SelectMonster == "Snowman" or SelectArea == 'Snow' then -- Snowman
			Ms = "Snowman"
			NameQuest = "SnowQuest"
			QuestLv = 2
			NameMon = "Snowman"
			CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
			CFrameMon = CFrame.new(1218.7956542969, 138.01184082031, -1488.0262451172)
		elseif Lv == 120 or Lv <= 149 or SelectMonster == "Chief Petty Officer" or SelectArea == 'Marine' then -- Chief Petty Officer
			Ms = "Chief Petty Officer"
			NameQuest = "MarineQuest2"
			QuestLv = 1
			NameMon = "Chief Petty Officer"
			CFrameQ = CFrame.new(-5035.49609375, 28.677835464478, 4324.1840820313)
			CFrameMon = CFrame.new(-4931.1552734375, 65.793113708496, 4121.8393554688)
		elseif Lv == 150 or Lv <= 174 or SelectMonster == "Sky Bandit" or SelectArea == 'Sky' then -- Sky Bandit
			Ms = "Sky Bandit"
			NameQuest = "SkyQuest"
			QuestLv = 1
			NameMon = "Sky Bandit"
			CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
			CFrameMon = CFrame.new(-4955.6411132813, 365.46365356445, -2908.1865234375)
		elseif Lv == 175 or Lv <= 189 or SelectMonster == "Dark Master" or SelectArea == 'Sky' then -- Dark Master
			Ms = "Dark Master"
			NameQuest = "SkyQuest"
			QuestLv = 2
			NameMon = "Dark Master"
			CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
			CFrameMon = CFrame.new(-5148.1650390625, 439.04571533203, -2332.9611816406)
		elseif Lv == 190 or Lv <= 209 or SelectMonster == "Prisoner" or SelectArea == 'Prison' then -- Prisoner
			Ms = "Prisoner"
			NameQuest = "PrisonerQuest"
			QuestLv = 1
			NameMon = "Prisoner"
			CFrameQ = CFrame.new(5310.60547, 0.350014925, 474.946594, 0.0175017118, 0, 0.999846935, 0, 1, 0, -0.999846935, 0, 0.0175017118)
			CFrameMon = CFrame.new(4937.31885, 0.332031399, 649.574524, 0.694649816, 0, -0.719348073, 0, 1, 0, 0.719348073, 0, 0.694649816)
		elseif Lv == 210 or Lv <= 249 or SelectMonster == "Dangerous Prisoner" or SelectArea == 'Prison' then -- Dangerous Prisoner
			Ms = "Dangerous Prisoner"
			NameQuest = "PrisonerQuest"
			QuestLv = 2
			NameMon = "Dangerous Prisoner"
			CFrameQ = CFrame.new(5310.60547, 0.350014925, 474.946594, 0.0175017118, 0, 0.999846935, 0, 1, 0, -0.999846935, 0, 0.0175017118)
			CFrameMon = CFrame.new(5099.6626, 0.351562679, 1055.7583, 0.898906827, 0, -0.438139856, 0, 1, 0, 0.438139856, 0, 0.898906827)
		elseif Lv == 250 or Lv <= 274 or SelectMonster == "Toga Warrior" or SelectArea == 'Colosseum' then -- Toga Warrior
			Ms = "Toga Warrior"
			NameQuest = "ColosseumQuest"
			QuestLv = 1
			NameMon = "Toga Warrior"
			CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
			CFrameMon = CFrame.new(-1872.5166015625, 49.080215454102, -2913.810546875)
		elseif Lv == 275 or Lv <= 299 or SelectMonster == "Gladiator" or SelectArea == 'Colosseum' then -- Gladiator
			Ms = "Gladiator"
			NameQuest = "ColosseumQuest"
			QuestLv = 2
			NameMon = "Gladiator"
			CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
			CFrameMon = CFrame.new(-1521.3740234375, 81.203170776367, -3066.3139648438)
		elseif Lv == 300 or Lv <= 324 or SelectMonster == "Military Soldier" or SelectArea == 'Magma' then -- Military Soldier
			Ms = "Military Soldier"
			NameQuest = "MagmaQuest"
			QuestLv = 1
			NameMon = "Military Soldier"
			CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
			CFrameMon = CFrame.new(-5369.0004882813, 61.24352645874, 8556.4921875)
		elseif Lv == 325 or Lv <= 374 or SelectMonster == "Military Spy" or SelectArea == 'Magma' then -- Military Spy
			Ms = "Military Spy"
			NameQuest = "MagmaQuest"
			QuestLv = 2
			NameMon = "Military Spy"
			CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
			CFrameMon = CFrame.new(-5787.00293, 75.8262634, 8651.69922, 0.838590562, 0, -0.544762194, 0, 1, 0, 0.544762194, 0, 0.838590562)
		elseif Lv == 375 or Lv <= 399 or SelectMonster == "Fishman Warrior" or SelectArea == 'Fishman' then -- Fishman Warrior
			Ms = "Fishman Warrior"
			NameQuest = "FishmanQuest"
			QuestLv = 1
			NameMon = "Fishman Warrior"
			CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
			CFrameMon = CFrame.new(60844.10546875, 98.462875366211, 1298.3985595703)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2500 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
			end
		elseif Lv == 400 or Lv <= 449 or SelectMonster == "Fishman Commando" or SelectArea == 'Fishman' then -- Fishman Commando
			Ms = "Fishman Commando"
			NameQuest = "FishmanQuest"
			QuestLv = 2
			NameMon = "Fishman Commando"
			CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
			CFrameMon = CFrame.new(61738.3984375, 64.207321166992, 1433.8375244141)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2500 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
			end
		elseif Lv == 10 or Lv <= 474 or SelectMonster == "God's Guard" or SelectArea == 'Sky Island' then -- God's Guard
			Ms = "God's Guard"
			NameQuest = "SkyExp1Quest"
			QuestLv = 1
			NameMon = "God's Guard"
			CFrameQ = CFrame.new(-4721.8603515625, 845.30297851563, -1953.8489990234)
			CFrameMon = CFrame.new(-4628.0498046875, 866.92877197266, -1931.2352294922)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2500 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.82275, 872.54248, -1667.55688))
			end
		elseif Lv == 475 or Lv <= 524 or SelectMonster == "Shanda" or SelectArea == 'Sky Island' then -- Shanda
			Ms = "Shanda"
			NameQuest = "SkyExp1Quest"
			QuestLv = 2
			NameMon = "Shanda"
			CFrameQ = CFrame.new(-7863.1596679688, 5545.5190429688, -378.42266845703)
			CFrameMon = CFrame.new(-7685.1474609375, 5601.0751953125, -441.38876342773)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 2500 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
			end
		elseif Lv == 525 or Lv <= 549 or SelectMonster == "Royal Squad" or SelectArea == 'Sky Island' then -- Royal Squad
			Ms = "Royal Squad"
			NameQuest = "SkyExp2Quest"
			QuestLv = 1
			NameMon = "Royal Squad"
			CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
			CFrameMon = CFrame.new(-7654.2514648438, 5637.1079101563, -1407.7550048828)
		elseif Lv == 550 or Lv <= 624 or SelectMonster == "Royal Soldier" or SelectArea == 'Sky Island' then -- Royal Soldier
			Ms = "Royal Soldier"
			NameQuest = "SkyExp2Quest"
			QuestLv = 2
			NameMon = "Royal Soldier"
			CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
			CFrameMon = CFrame.new(-7760.4106445313, 5679.9077148438, -1884.8112792969)
		elseif Lv == 625 or Lv <= 649 or SelectMonster == "Galley Pirate" or SelectArea == 'Fountain' then -- Galley Pirate
			Ms = "Galley Pirate"
			NameQuest = "FountainQuest"
			QuestLv = 1
			NameMon = "Galley Pirate"
			CFrameQ = CFrame.new(5258.2788085938, 38.526931762695, 4050.044921875)
			CFrameMon = CFrame.new(5557.1684570313, 152.32717895508, 3998.7758789063)
		elseif Lv >= 650 or SelectMonster == "Galley Captain" or SelectArea == 'Fountain' then -- Galley Captain
			Ms = "Galley Captain"
			NameQuest = "FountainQuest"
			QuestLv = 2
			NameMon = "Galley Captain"
			CFrameQ = CFrame.new(5258.2788085938, 38.526931762695, 4050.044921875)
			CFrameMon = CFrame.new(5677.6772460938, 92.786109924316, 4966.6323242188)
		end
	end
	if Second_Sea then
		if Lv == 700 or Lv <= 724 or SelectMonster == "Raider" or SelectArea == 'Area 1' then -- Raider
			Ms = "Raider"
			NameQuest = "Area1Quest"
			QuestLv = 1
			NameMon = "Raider"
			CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
			CFrameMon = CFrame.new(68.874565124512, 93.635643005371, 2429.6752929688)
		elseif Lv == 725 or Lv <= 774 or SelectMonster == "Mercenary" or SelectArea == 'Area 1' then -- Mercenary
			Ms = "Mercenary"
			NameQuest = "Area1Quest"
			QuestLv = 2
			NameMon = "Mercenary"
			CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
			CFrameMon = CFrame.new(-864.85009765625, 122.47104644775, 1453.1505126953)
		elseif Lv == 775 or Lv <= 799 or SelectMonster == "Swan Pirate" or SelectArea == 'Area 2' then -- Swan Pirate
			Ms = "Swan Pirate"
			NameQuest = "Area2Quest"
			QuestLv = 1
			NameMon = "Swan Pirate"
			CFrameQ = CFrame.new(635.61151123047, 73.096351623535, 917.81298828125)
			CFrameMon = CFrame.new(1065.3669433594, 137.64012145996, 1324.3798828125)
		elseif Lv == 800 or Lv <= 874 or SelectMonster == "Factory Staff" or SelectArea == 'Area 2' then -- Factory Staff
			Ms = "Factory Staff"
			NameQuest = "Area2Quest"
			QuestLv = 2
			NameMon = "Factory Staff"
			CFrameQ = CFrame.new(635.61151123047, 73.096351623535, 917.81298828125)
			CFrameMon = CFrame.new(533.22045898438, 128.46876525879, 355.62615966797)
		elseif Lv == 875 or Lv <= 899 or SelectMonster == "Marine Lieutenan" or SelectArea == 'Marine' then -- Marine Lieutenant
			Ms = "Marine Lieutenant"
			NameQuest = "MarineQuest3"
			QuestLv = 1
			NameMon = "Marine Lieutenant"
			CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
			CFrameMon = CFrame.new(-2489.2622070313, 84.613594055176, -3151.8830566406)
		elseif Lv == 900 or Lv <= 949 or SelectMonster == "Marine Captain" or SelectArea == 'Marine' then -- Marine Captain
			Ms = "Marine Captain"
			NameQuest = "MarineQuest3"
			QuestLv = 2
			NameMon = "Marine Captain"
			CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
			CFrameMon = CFrame.new(-2335.2026367188, 79.786659240723, -3245.8674316406)
		elseif Lv == 950 or Lv <= 974 or SelectMonster == "Zombie" or SelectArea == 'Zombie' then -- Zombie
			Ms = "Zombie"
			NameQuest = "ZombieQuest"
			QuestLv = 1
			NameMon = "Zombie"
			CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
			CFrameMon = CFrame.new(-5536.4970703125, 101.08577728271, -835.59075927734)
		elseif Lv == 975 or Lv <= 999 or SelectMonster == "Vampire" or SelectArea == 'Zombie' then -- Vampire
			Ms = "Vampire"
			NameQuest = "ZombieQuest"
			QuestLv = 2
			NameMon = "Vampire"
			CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
			CFrameMon = CFrame.new(-5806.1098632813, 16.722528457642, -1164.4384765625)
		elseif Lv == 1000 or Lv <= 1049 or SelectMonster == "Snow Trooper" or SelectArea == 'Snow Mountain' then -- Snow Trooper
			Ms = "Snow Trooper"
			NameQuest = "SnowMountainQuest"
			QuestLv = 1
			NameMon = "Snow Trooper"
			CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
			CFrameMon = CFrame.new(535.21051025391, 432.74209594727, -5484.9165039063)
		elseif Lv == 1050 or Lv <= 1099 or SelectMonster == "Winter Warrior" or SelectArea == 'Snow Mountain' then -- Winter Warrior
			Ms = "Winter Warrior"
			NameQuest = "SnowMountainQuest"
			QuestLv = 2
			NameMon = "Winter Warrior"
			CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
			CFrameMon = CFrame.new(1234.4449462891, 456.95419311523, -5174.130859375)
		elseif Lv == 1100 or Lv <= 1124 or SelectMonster == "Lab Subordinate" or SelectArea == 'Ice Fire' then -- Lab Subordinate
			Ms = "Lab Subordinate"
			NameQuest = "IceSideQuest"
			QuestLv = 1
			NameMon = "Lab Subordinate"
			CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
			CFrameMon = CFrame.new(-5720.5576171875, 63.309471130371, -4784.6103515625)
		elseif Lv == 1125 or Lv <= 1174 or SelectMonster == "Horned Warrior" or SelectArea == 'Ice Fire' then -- Horned Warrior
			Ms = "Horned Warrior"
			NameQuest = "IceSideQuest"
			QuestLv = 2
			NameMon = "Horned Warrior"
			CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
			CFrameMon = CFrame.new(-6292.751953125, 91.181983947754, -5502.6499023438)
		elseif Lv == 1175 or Lv <= 1199 or SelectMonster == "Magma Ninja" or SelectArea == 'Ice Fire' then -- Magma Ninja
			Ms = "Magma Ninja"
			NameQuest = "FireSideQuest"
			QuestLv = 1
			NameMon = "Magma Ninja"
			CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
			CFrameMon = CFrame.new(-5461.8388671875, 130.36347961426, -5836.4702148438)
		elseif Lv == 1200 or Lv <= 1249 or SelectMonster == "Lava Pirate" or SelectArea == 'Ice Fire' then -- Lava Pirate
			Ms = "Lava Pirate"
			NameQuest = "FireSideQuest"
			QuestLv = 2
			NameMon = "Lava Pirate"
			CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
			CFrameMon = CFrame.new(-5251.1889648438, 55.164535522461, -4774.4096679688)
		elseif Lv == 1250 or Lv <= 1274 or SelectMonster == "Ship Deckhand" or SelectArea == 'Ship' then -- Ship Deckhand
			Ms = "Ship Deckhand"
			NameQuest = "ShipQuest1"
			QuestLv = 1
			NameMon = "Ship Deckhand"
			CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
			CFrameMon = CFrame.new(921.12365722656, 125.9839553833, 33088.328125)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
			end
		elseif Lv == 1275 or Lv <= 1299 or SelectMonster == "Ship Engineer" or SelectArea == 'Ship' then -- Ship Engineer
			Ms = "Ship Engineer"
			NameQuest = "ShipQuest1"
			QuestLv = 2
			NameMon = "Ship Engineer"
			CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
			CFrameMon = CFrame.new(886.28179931641, 40.47790145874, 32800.83203125)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
			end
		elseif Lv == 1300 or Lv <= 1324 or SelectMonster == "Ship Steward" or SelectArea == 'Ship' then -- Ship Steward
			Ms = "Ship Steward"
			NameQuest = "ShipQuest2"
			QuestLv = 1
			NameMon = "Ship Steward"
			CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
			CFrameMon = CFrame.new(943.85504150391, 129.58183288574, 33444.3671875)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
			end
		elseif Lv == 1325 or Lv <= 1349 or SelectMonster == "Ship Officer" or SelectArea == 'Ship' then -- Ship Officer
			Ms = "Ship Officer"
			NameQuest = "ShipQuest2"
			QuestLv = 2
			NameMon = "Ship Officer"
			CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
			CFrameMon = CFrame.new(955.38458251953, 181.08335876465, 33331.890625)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
			end
		elseif Lv == 1350 or Lv <= 1374 or SelectMonster == "Arctic Warrior" or SelectArea == 'Frost' then -- Arctic Warrior
			Ms = "Arctic Warrior"
			NameQuest = "FrostQuest"
			QuestLv = 1
			NameMon = "Arctic Warrior"
			CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
			CFrameMon = CFrame.new(5935.4541015625, 77.26016998291, -6472.7568359375)
			if getgenv().AutoLevel and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-6508.5581054688, 89.034996032715, -132.83953857422))
			end
		elseif Lv == 1375 or Lv <= 1424 or SelectMonster == "Snow Lurker" or SelectArea == 'Frost' then -- Snow Lurker
			Ms = "Snow Lurker"
			NameQuest = "FrostQuest"
			QuestLv = 2
			NameMon = "Snow Lurker"
			CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
			CFrameMon = CFrame.new(5628.482421875, 57.574996948242, -6618.3481445313)
		elseif Lv == 1425 or Lv <= 1449 or SelectMonster == "Sea Soldier" or SelectArea == 'Forgotten' then -- Sea Soldier
			Ms = "Sea Soldier"
			NameQuest = "ForgottenQuest"
			QuestLv = 1
			NameMon = "Sea Soldier"
			CFrameQ = CFrame.new(-3054.5827636719, 236.87213134766, -10147.790039063)
			CFrameMon = CFrame.new(-3185.0153808594, 58.789089202881, -9663.6064453125)
		elseif Lv >= 1450 or SelectMonster == "Water Fighter" or SelectArea == 'Forgotten' then -- Water Fighter
			Ms = "Water Fighter"
			NameQuest = "ForgottenQuest"
			QuestLv = 2
			NameMon = "Water Fighter"
			CFrameQ = CFrame.new(-3054.5827636719, 236.87213134766, -10147.790039063)
			CFrameMon = CFrame.new(-3262.9301757813, 298.69036865234, -10552.529296875)
		end
	end
	if Third_Sea then
		if Lv == 1500 or Lv <= 1524 or SelectMonster == "Pirate Millionaire" or SelectArea == 'Pirate Port' then -- Pirate Millionaire
			Ms = "Pirate Millionaire"
			NameQuest = "PiratePortQuest"
			QuestLv = 1
			NameMon = "Pirate Millionaire"
			CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
			CFrameMon = CFrame.new(-435.68109130859, 189.69866943359, 5551.0756835938)
		elseif Lv == 1525 or Lv <= 1574 or SelectMonster == "Pistol Billionaire" or SelectArea == 'Pirate Port' then -- Pistol Billoonaire
			Ms = "Pistol Billionaire"
			NameQuest = "PiratePortQuest"
			QuestLv = 2
			NameMon = "Pistol Billionaire"
			CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
			CFrameMon = CFrame.new(-236.53652954102, 217.46676635742, 6006.0883789063)
		elseif Lv == 1575 or Lv <= 1599 or SelectMonster == "Dragon Crew Warrior" or SelectArea == 'Amazon' then -- Dragon Crew Warrior
			Ms = "Dragon Crew Warrior"
			NameQuest = "AmazonQuest"
			QuestLv = 1
			NameMon = "Dragon Crew Warrior"
			CFrameQ = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
			CFrameMon = CFrame.new(6301.9975585938, 104.77153015137, -1082.6075439453)
		elseif Lv == 1600 or Lv <= 1624 or SelectMonster == "Dragon Crew Archer" or SelectArea == 'Amazon' then -- Dragon Crew Archer
			Ms = "Dragon Crew Archer"
			NameQuest = "AmazonQuest"
			QuestLv = 2
			NameMon = "Dragon Crew Archer"
			CFrameQ = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
			CFrameMon = CFrame.new(6831.1171875, 441.76708984375, 446.58615112305)
		elseif Lv == 1625 or Lv <= 1649 or SelectMonster == "Female Islander" or SelectArea == 'Amazon' then -- Female Islander
			Ms = "Female Islander"
			NameQuest = "AmazonQuest2"
			QuestLv = 1
			NameMon = "Female Islander"
			CFrameQ = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
			CFrameMon = CFrame.new(5792.5166015625, 848.14392089844, 1084.1818847656)
		elseif Lv == 1650 or Lv <= 1699 or SelectMonster == "Giant Islander" or SelectArea == 'Amazon' then -- Giant Islander
			Ms = "Giant Islander"
			NameQuest = "AmazonQuest2"
			QuestLv = 2
			NameMon = "Giant Islander"
			CFrameQ = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
			CFrameMon = CFrame.new(5009.5068359375, 664.11071777344, -40.960144042969)
		elseif Lv == 1700 or Lv <= 1724 or SelectMonster == "Marine Commodore" or SelectArea == 'Marine Tree' then -- Marine Commodore
			Ms = "Marine Commodore"
			NameQuest = "MarineTreeIsland"
			QuestLv = 1
			NameMon = "Marine Commodore"
			CFrameQ = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
			CFrameMon = CFrame.new(2198.0063476563, 128.71075439453, -7109.5043945313)
		elseif Lv == 1725 or Lv <= 1774 or SelectMonster == "Marine Rear Admiral" or SelectArea == 'Marine Tree' then -- Marine Rear Admiral
			Ms = "Marine Rear Admiral"
			NameQuest = "MarineTreeIsland"
			QuestLv = 2
			NameMon = "Marine Rear Admiral"
			CFrameQ = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
			CFrameMon = CFrame.new(3294.3142089844, 385.41125488281, -7048.6342773438)
		elseif Lv == 1775 or Lv <= 1799 or SelectMonster == "Fishman Raider" or SelectArea == 'Deep Forest' then -- Fishman Raide
			Ms = "Fishman Raider"
			NameQuest = "DeepForestIsland3"
			QuestLv = 1
			NameMon = "Fishman Raider"
			CFrameQ = CFrame.new(-10582.759765625, 331.78845214844, -8757.666015625)
			CFrameMon = CFrame.new(-10553.268554688, 521.38439941406, -8176.9458007813)
		elseif Lv == 1800 or Lv <= 1824 or SelectMonster == "Fishman Captain" or SelectArea == 'Deep Forest' then -- Fishman Captain
			Ms = "Fishman Captain"
			NameQuest = "DeepForestIsland3"
			QuestLv = 2
			NameMon = "Fishman Captain"
			CFrameQ = CFrame.new(-10583.099609375, 331.78845214844, -8759.4638671875)
			CFrameMon = CFrame.new(-10789.401367188, 427.18637084961, -9131.4423828125)
		elseif Lv == 1825 or Lv <= 1849 or SelectMonster == "Forest Pirate" or SelectArea == 'Deep Forest' then -- Forest Pirate
			Ms = "Forest Pirate"
			NameQuest = "DeepForestIsland"
			QuestLv = 1
			NameMon = "Forest Pirate"
			CFrameQ = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
			CFrameMon = CFrame.new(-13489.397460938, 400.30349731445, -7770.251953125)
		elseif Lv == 1850 or Lv <= 1899 or SelectMonster == "Mythological Pirate" or SelectArea == 'Deep Forest' then -- Mythological Pirate
			Ms = "Mythological Pirate"
			NameQuest = "DeepForestIsland"
			QuestLv = 2
			NameMon = "Mythological Pirate"
			CFrameQ = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
			CFrameMon = CFrame.new(-13508.616210938, 582.46228027344, -6985.3037109375)
		elseif Lv == 1900 or Lv <= 1924 or SelectMonster == "Jungle Pirate" or SelectArea == 'Deep Forest' then -- Jungle Pirate
			Ms = "Jungle Pirate"
			NameQuest = "DeepForestIsland2"
			QuestLv = 1
			NameMon = "Jungle Pirate"
			CFrameQ = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
			CFrameMon = CFrame.new(-12267.103515625, 459.75262451172, -10277.200195313)
		elseif Lv == 1925 or Lv <= 1974 or SelectMonster == "Musketeer Pirate" or SelectArea == 'Deep Forest' then -- Musketeer Pirate
			Ms = "Musketeer Pirate"
			NameQuest = "DeepForestIsland2"
			QuestLv = 2
			NameMon = "Musketeer Pirate"
			CFrameQ = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
			CFrameMon = CFrame.new(-13291.5078125, 520.47338867188, -9904.638671875)
		elseif Lv == 1975 or Lv <= 1999 or SelectMonster == "Reborn Skeleton" or SelectArea == 'Haunted Castle' then
			Ms = "Reborn Skeleton"
			NameQuest = "HauntedQuest1"
			QuestLv = 1
			NameMon = "Reborn Skeleton"
			CFrameQ = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
			CFrameMon = CFrame.new(-8761.77148, 183.431747, 6168.33301, 0.978073597, -1.3950732e-05, -0.208259016, -1.08073925e-06, 1, -7.20630269e-05, 0.208259016, 7.07080399e-05, 0.978073597)
		elseif Lv == 2000 or Lv <= 2024 or SelectMonster == "Living Zombie" or SelectArea == 'Haunted Castle' then
			Ms = "Living Zombie"
			NameQuest = "HauntedQuest1"
			QuestLv = 2
			NameMon = "Living Zombie"
			CFrameQ = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
			CFrameMon = CFrame.new(-10103.7529, 238.565979, 6179.75977, 0.999474227, 2.77547141e-08, 0.0324240364, -2.58006327e-08, 1, -6.06848474e-08, -0.0324240364, 5.98163865e-08, 0.999474227)
		elseif Lv == 2025 or Lv <= 2049 or SelectMonster == "Demonic Soul" or SelectArea == 'Haunted Castle' then
			Ms = "Demonic Soul"
			NameQuest = "HauntedQuest2"
			QuestLv = 1
			NameMon = "Demonic Soul"
			CFrameQ = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
			CFrameMon = CFrame.new(-9712.03125, 204.69589233398, 6193.322265625)
		elseif Lv == 2050 or Lv <= 2074 or SelectMonster == "Posessed Mummy" or SelectArea == 'Haunted Castle' then
			Ms = "Posessed Mummy"
			NameQuest = "HauntedQuest2"
			QuestLv = 2
			NameMon = "Posessed Mummy"
			CFrameQ = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
			CFrameMon = CFrame.new(-9545.7763671875, 69.619895935059, 6339.5615234375)
		elseif Lv == 2075 or Lv <= 2099 or SelectMonster == "Peanut Scout" or SelectArea == 'Nut Island' then
			Ms = "Peanut Scout"
			NameQuest = "NutsIslandQuest"
			QuestLv = 1
			NameMon = "Peanut Scout"
			CFrameQ = CFrame.new(-2105.53198, 37.2495995, -10195.5088, -0.766061664, 0, -0.642767608, 0, 1, 0, 0.642767608, 0, -0.766061664)
			CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
		elseif Lv == 2100 or Lv <= 2124 or SelectMonster == "Peanut President" or SelectArea == 'Nut Island' then
			Ms = "Peanut President"
			NameQuest = "NutsIslandQuest"
			QuestLv = 2
			NameMon = "Peanut President"
			CFrameQ = CFrame.new(-2105.53198, 37.2495995, -10195.5088, -0.766061664, 0, -0.642767608, 0, 1, 0, 0.642767608, 0, -0.766061664)
			CFrameMon = CFrame.new(-2150.587890625, 122.49767303467, -10358.994140625)
		elseif Lv == 2125 or Lv <= 2149 or SelectMonster == "Ice Cream Chef" or SelectArea == 'Ice Cream Island' then
			Ms = "Ice Cream Chef"
			NameQuest = "IceCreamIslandQuest"
			QuestLv = 1
			NameMon = "Ice Cream Chef"
			CFrameQ = CFrame.new(-819.376709, 64.9259796, -10967.2832, -0.766061664, 0, 0.642767608, 0, 1, 0, -0.642767608, 0, -0.766061664)
			CFrameMon = CFrame.new(-789.941528, 209.382889, -11009.9805, -0.0703101531, -0, -0.997525156, -0, 1.00000012, -0, 0.997525275, 0, -0.0703101456)
		elseif Lv == 2150 or Lv <= 2199 or SelectMonster == "Ice Cream Commander" or SelectArea == 'Ice Cream Island' then
			Ms = "Ice Cream Commander"
			NameQuest = "IceCreamIslandQuest"
			QuestLv = 2
			NameMon = "Ice Cream Commander"
			CFrameQ = CFrame.new(-819.376709, 64.9259796, -10967.2832, -0.766061664, 0, 0.642767608, 0, 1, 0, -0.642767608, 0, -0.766061664)
			CFrameMon = CFrame.new(-789.941528, 209.382889, -11009.9805, -0.0703101531, -0, -0.997525156, -0, 1.00000012, -0, 0.997525275, 0, -0.0703101456)
		elseif Lv == 2200 or Lv <= 2224 or SelectMonster == "Cookie Crafter" or SelectArea == 'Cake Island' then
			Ms = "Cookie Crafter"
			NameQuest = "CakeQuest1"
			QuestLv = 1
			NameMon = "Cookie Crafter"
			CFrameQ = CFrame.new(-2022.29858, 36.9275894, -12030.9766, -0.961273909, 0, -0.275594592, 0, 1, 0, 0.275594592, 0, -0.961273909)
			CFrameMon = CFrame.new(-2321.71216, 36.699482, -12216.7871, -0.780074954, 0, 0.625686109, 0, 1, 0, -0.625686109, 0, -0.780074954)
		elseif Lv == 2225 or Lv <= 2249 or SelectMonster == "Cake Guard" or SelectArea == 'Cake Island' then
			Ms = "Cake Guard"
			NameQuest = "CakeQuest1"
			QuestLv = 2
			NameMon = "Cake Guard"
			CFrameQ = CFrame.new(-2022.29858, 36.9275894, -12030.9766, -0.961273909, 0, -0.275594592, 0, 1, 0, 0.275594592, 0, -0.961273909)
			CFrameMon = CFrame.new(-1418.11011, 36.6718941, -12255.7324, 0.0677844882, 0, 0.997700036, 0, 1, 0, -0.997700036, 0, 0.0677844882)
		elseif Lv == 2250 or Lv <= 2274 or SelectMonster == "Baking Staff" or SelectArea == 'Cake Island' then
			Ms = "Baking Staff"
			NameQuest = "CakeQuest2"
			QuestLv = 1
			NameMon = "Baking Staff"
			CFrameQ = CFrame.new(-1928.31763, 37.7296638, -12840.626, 0.951068401, -0, -0.308980465, 0, 1, -0, 0.308980465, 0, 0.951068401)
			CFrameMon = CFrame.new(-1980.43848, 36.6716766, -12983.8418, -0.254443765, 0, -0.967087567, 0, 1, 0, 0.967087567, 0, -0.254443765)
		elseif Lv == 2275 or Lv <= 2299 or SelectMonster == "Head Baker" or SelectArea == 'Cake Island' then
			Ms = "Head Baker"
			NameQuest = "CakeQuest2"
			QuestLv = 2
			NameMon = "Head Baker"
			CFrameQ = CFrame.new(-1928.31763, 37.7296638, -12840.626, 0.951068401, -0, -0.308980465, 0, 1, -0, 0.308980465, 0, 0.951068401)
			CFrameMon = CFrame.new(-2251.5791, 52.2714615, -13033.3965, -0.991971016, 0, -0.126466095, 0, 1, 0, 0.126466095, 0, -0.991971016)
		elseif Lv == 2300 or Lv <= 2324 or SelectMonster == "Cocoa Warrior" or SelectArea == 'Choco Island' then
			Ms = "Cocoa Warrior"
			NameQuest = "ChocQuest1"
			QuestLv = 1
			NameMon = "Cocoa Warrior"
			CFrameQ = CFrame.new(231.75, 23.9003029, -12200.292, -1, 0, 0, 0, 1, 0, 0, 0, -1)
			CFrameMon = CFrame.new(167.978516, 26.2254658, -12238.874, -0.939700961, 0, 0.341998369, 0, 1, 0, -0.341998369, 0, -0.939700961)
		elseif Lv == 2325 or Lv <= 2349 or SelectMonster == "Chocolate Bar Battler" or SelectArea == 'Choco Island' then
			Ms = "Chocolate Bar Battler"
			NameQuest = "ChocQuest1"
			QuestLv = 2
			NameMon = "Chocolate Bar Battler"
			CFrameQ = CFrame.new(231.75, 23.9003029, -12200.292, -1, 0, 0, 0, 1, 0, 0, 0, -1)
			CFrameMon = CFrame.new(701.312073, 25.5824986, -12708.2148, -0.342042685, 0, -0.939684391, 0, 1, 0, 0.939684391, 0, -0.342042685)
		elseif Lv == 2350 or Lv <= 2374 or SelectMonster == "Sweet Thief" or SelectArea == 'Choco Island' then
			Ms = "Sweet Thief"
			NameQuest = "ChocQuest2"
			QuestLv = 1
			NameMon = "Sweet Thief"
			CFrameQ = CFrame.new(151.198242, 23.8907146, -12774.6172, 0.422592998, 0, 0.906319618, 0, 1, 0, -0.906319618, 0, 0.422592998)
			CFrameMon = CFrame.new(-140.258301, 25.5824986, -12652.3115, 0.173624337, -0, -0.984811902, 0, 1, -0, 0.984811902, 0, 0.173624337)
		elseif Lv == 2375 or Lv <= 2400 or SelectMonster == "Candy Rebel" or SelectArea == 'Choco Island' then
			Ms = "Candy Rebel"
			NameQuest = "ChocQuest2"
			QuestLv = 2
			NameMon = "Candy Rebel"
			CFrameQ = CFrame.new(151.198242, 23.8907146, -12774.6172, 0.422592998, 0, 0.906319618, 0, 1, 0, -0.906319618, 0, 0.422592998)
			CFrameMon = CFrame.new(47.9231453, 25.5824986, -13029.2402, -0.819156051, 0, -0.573571265, 0, 1, 0, 0.573571265, 0, -0.819156051)
		elseif Lv == 2400 or Lv <= 2424 or SelectMonster == "Candy Pirate" or SelectArea == 'Candy Island' then
			Ms = "Candy Pirate"
			NameQuest = "CandyQuest1"
			QuestLv = 1
			NameMon = "Candy Pirate"
			CFrameQ = CFrame.new(-1149.328, 13.5759039, -14445.6143, -0.156446099, 0, -0.987686574, 0, 1, 0, 0.987686574, 0, -0.156446099)
			CFrameMon = CFrame.new(-1437.56348, 17.1481285, -14385.6934, 0.173624337, -0, -0.984811902, 0, 1, -0, 0.984811902, 0, 0.173624337)
		elseif Lv == 2425 or Lv <= 2449 or SelectMonster == "Snow Demon" or SelectArea == 'Candy Island' then
			Ms = "Snow Demon"
			NameQuest = "CandyQuest1"
			QuestLv = 2
			NameMon = "Snow Demon"
			CFrameQ = CFrame.new(-1149.328, 13.5759039, -14445.6143, -0.156446099, 0, -0.987686574, 0, 1, 0, 0.987686574, 0, -0.156446099)
			CFrameMon = CFrame.new(-916.222656, 17.1481285, -14638.8125, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
		elseif Lv == 2450 or Lv <= 2474 or SelectMonster == "Isle Outlaw" or SelectArea == 'Tiki Outpost' then
			Ms = "Isle Outlaw"
			NameQuest = "TikiQuest1"
			QuestLv = 1
			NameMon = "Isle Outlaw"
			CFrameQ = CFrame.new(-16549.890625, 55.68635559082031, -179.91360473632812)
			CFrameMon = CFrame.new(-16162.8193359375, 11.6863374710083, -96.45481872558594)
		elseif Lv == 2475 or Lv <= 2499 or SelectMonster == "Island Boy" or SelectArea == 'Tiki Outpost' then
			Ms = "Island Boy"
			NameQuest = "TikiQuest1"
			QuestLv = 2
			NameMon = "Island Boy"
			CFrameQ = CFrame.new(-16549.890625, 55.68635559082031, -179.91360473632812)
			CFrameMon = CFrame.new(-16912.130859375, 11.787443161010742, -133.0850830078125)
		elseif Lv == 2500 or Lv <= 2424 then
			Ms = "Sun-kissed Warrior"
			QuestLv = 1
			NameQuest = "TikiQuest2"
			NameMon = "kissed"
			CFrameQ = CFrame.new(-16539.078125, 55.68632888793945, 1051.5738525390625)
			CFrameMon = CFrame.new(-16349.8779296875, 92.0808334350586, 1123.4169921875)
		elseif Lv >= 2525 or SelectMonster == "Isle Champion" or SelectArea == 'Tiki Outpost' then
			Ms = "Isle Champion"
			NameQuest = "TikiQuest2"
			QuestLv = 2
			NameMon = "Isle Champion"
			CFrameQ = CFrame.new(-16542.447265625, 55.68632888793945, 1044.41650390625)
			CFrameMon = CFrame.new(-16848.94140625, 21.68633460998535, 1041.4490966796875)
		end
	end
end
--Check Materials
function MaterialMon()
	if getgenv().SelectMaterial == "Radioactive Material" then
		MMon = "Factory Staff"
		MPos = CFrame.new(295, 73, -56)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Mystic Droplet" then
		MMon = "Water Fighter"
		MPos = CFrame.new(-3385, 239, -10542)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Magma Ore" then
		if First_Sea then
			MMon = "Military Spy"
			MPos = CFrame.new(-5815, 84, 8820)
			SP = "Default"
		elseif Second_Sea then
			MMon = "Magma Ninja"
			MPos = CFrame.new(-5428, 78, -5959)
			SP = "Default"
		end
	elseif getgenv().SelectMaterial == "Angel Wings" then
		MMon = "God's Guard"
		MPos = CFrame.new(-4698, 845, -1912)
		SP = "Default"
		if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-7859.09814, 5544.19043, -381.476196)).Magnitude >= 5000 then
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7859.09814, 5544.19043, -381.476196))
		end
	elseif getgenv().SelectMaterial == "Leather" then
		if First_Sea then
			MMon = "Brute"
			MPos = CFrame.new(-1145, 15, 4350)
			SP = "Default"
		elseif Second_Sea then
			MMon = "Marine Captain"
			MPos = CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375)
			SP = "Default"
		elseif Third_Sea then
			MMon = "Jungle Pirate"
			MPos = CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375)
			SP = "Default"
		end
	elseif getgenv().SelectMaterial == "Scrap Metal" then
		if First_Sea then
			MMon = "Brute"
			MPos = CFrame.new(-1145, 15, 4350)
			SP = "Default"
		elseif Second_Sea then
			MMon = "Swan Pirate"
			MPos = CFrame.new(878, 122, 1235)
			SP = "Default"
		elseif Third_Sea then
			MMon = "Jungle Pirate"
			MPos = CFrame.new(-12107, 332, -10549)
			SP = "Default"
		end
	elseif getgenv().SelectMaterial == "Fish Tail" then
		if Third_Sea then
			MMon = "Fishman Raider"
			MPos = CFrame.new(-10993, 332, -8940)
			SP = "Default"
		elseif First_Sea then
			MMon = "Fishman Warrior"
			MPos = CFrame.new(61123, 19, 1569)
			SP = "Default"
			if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(61163.8515625, 5.342342376708984, 1819.7841796875)).Magnitude >= 17000 then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(61163.8515625, 5.342342376708984, 1819.7841796875))
			end
		end
	elseif getgenv().SelectMaterial == "Demonic Wisp" then
		MMon = "Demonic Soul"
		MPos = CFrame.new(-9507, 172, 6158)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Vampire Fang" then
		MMon = "Vampire"
		MPos = CFrame.new(-6033, 7, -1317)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Conjured Cocoa" then
		MMon = "Chocolate Bar Battler"
		MPos = CFrame.new(620.6344604492188, 78.93644714355469, -12581.369140625)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Dragon Scale" then
		MMon = "Dragon Crew Archer"
		MPos = CFrame.new(6594, 383, 139)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Gunpowder" then
		MMon = "Pistol Billionaire"
		MPos = CFrame.new(-469, 74, 5904)
		SP = "Default"
	elseif getgenv().SelectMaterial == "Mini Tusk" then
		MMon = "Mythological Pirate"
		MPos = CFrame.new(-13545, 470, -6917)
		SP = "Default"
	end
end
--WaitBBC
function GetDistance(target)
	return math.floor((target.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude)
end
function BTP(p)
	pcall(function()
		if (p.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude >= 1500 and not Auto_Raid and game.Players.LocalPlayer.Character.Humanoid.Health > 0 then
			repeat
				wait()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
				wait(0.5)
				game.Players.LocalPlayer.Character.Head:Destroy()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
			until (p.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 1500 and game.Players.LocalPlayer.Character.Humanoid.Health > 0
		end
	end)
end
function TP(Pos)
	Distance = (Pos.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
	if Distance < 300 then
		Speed = 300
	elseif Distance >= 1000 then
		Speed = 300
	end
	game:GetService("TweenService"):Create(
            game:GetService("Players").LocalPlayer.Character.HumanoidRootPart,
            TweenInfo.new(Distance / Speed, Enum.EasingStyle.Linear),
            {
		CFrame = Pos
	}
        ):Play()
	_G.Clip = true
	wait(Distance / Speed)
	_G.Clip = false
end

function CheckNearestTeleporter(aI)
	local MyLevel = game.Players.LocalPlayer.Data.Level.Value
	vcspos = aI.Position
	min = math.huge
	min2 = math.huge
	local y = game.PlaceId
	if y == 2753915549 then
		OldWorld = true
	elseif y == 4442272183 then
		NewWorld = true
	elseif y == 7449423635 then
		ThreeWorld = true
	end
	if Atsea3 then
		TableLocations = {
			["Caslte On The Sea"] = Vector3.new(-5058.77490234375, 314.5155029296875, -3155.88330078125),
			["Hydra"] = Vector3.new(5756.83740234375, 610.4240112304688, -253.9253692626953),
			["Mansion"] = Vector3.new(-12463.8740234375, 374.9144592285156, -7523.77392578125),
			["Great Tree"] = Vector3.new(28282.5703125, 14896.8505859375, 105.1042709350586),
			["Ngu1"] = Vector3.new(-11993.580078125, 334.7812805175781, -8844.1826171875),
			["ngu2"] = Vector3.new(5314.58203125, 25.419387817382812, -125.94227600097656)
		}
	elseif Atsea2 then
		TableLocations = {
			["Mansion"] = Vector3.new(-288.46246337890625, 306.130615234375, 597.9988403320312),
			["Flamingo"] = Vector3.new(2284.912109375, 15.152046203613281, 905.48291015625),
			["122"] = Vector3.new(923.21252441406, 126.9760055542, 32852.83203125),
			["3032"] = Vector3.new(-6508.5581054688, 89.034996032715, -132.83953857422)
		}
	elseif Atsea1 then
		TableLocations = {
			["1"] = Vector3.new(-7894.6201171875, 5545.49169921875, -380.2467346191406),
			["2"] = Vector3.new(-4607.82275390625, 872.5422973632812, -1667.556884765625),
			["3"] = Vector3.new(61163.8515625, 11.759522438049316, 1819.7841796875),
			["4"] = Vector3.new(3876.280517578125, 35.10614013671875, -1939.3201904296875)
		}
	end
	TableLocations2 = {}
	for r, v in pairs(TableLocations) do
		TableLocations2[r] = (v - vcspos).Magnitude
	end
	for r, v in pairs(TableLocations2) do
		if v < min then
			min = v
			min2 = v
		end
	end
	for r, v in pairs(TableLocations2) do
		if v < min then
			min = v
			min2 = v
		end
	end
	for r, v in pairs(TableLocations2) do
		if v <= min then
			choose = TableLocations[r]
		end
	end
	min3 = (vcspos - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
	if min2 <= min3 then
		return choose
	end
	return
end
function requestEntrance(aJ)
	args = {
		"requestEntrance",
		aJ
	}
	game.ReplicatedStorage.Remotes.CommF_:InvokeServer(unpack(args))
	oldcframe = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
	char = game.Players.LocalPlayer.Character.HumanoidRootPart
	char.CFrame = CFrame.new(oldcframe.X, oldcframe.Y + 50, oldcframe.Z)
	task.wait(0.5)
end
function AntiLowHealth(aK)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame =
            CFrame.new(
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X,
            aK,
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z
        )
	wait()
end
function conc(v)
	return math.abs(v - game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Y)
end

function GetNearstEntrance(v3)
    if not TableLocations then return end
    local v1, v2 = math.huge
    for i, v in pairs(TableLocations) do
        if (v - v3.Position).Magnitude < v1 then
            v1, v2 = TableLocations(v), v
            ahihi = i
        end
    end
    if (v2 - v3.Position).Magnitude < GetDistance(v3) then
    print("lol")
        return v2, ahihi
    end
    return
end
TweenSpeed = 300
topos = function(v)
	local realtarget
	if typeof(v) == "CFrame" then
		realtarget = v
	elseif typeof(v) == "Vector3" then
		realtarget = CFrame.new(v)
	end
	su, er = pcall(function()
		if game:GetService("Players").LocalPlayer and game:GetService("Players").LocalPlayer.Character and game:GetService("Players").LocalPlayer.Character:FindFirstChild("Humanoid") and game:GetService("Players").LocalPlayer.Character:FindFirstChild("HumanoidRootPart") and game:GetService("Players").LocalPlayer.Character.Humanoid.Health > 0 and game:GetService("Players").LocalPlayer.Character.HumanoidRootPart then
			if not TweenSpeed then
				TweenSpeed = 320
			end
			local DefualtY = realtarget.Y
			local Distance = GetDistance(realtarget)
			if Distance < 300 then
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = realtarget
			end
			local nearestT = CheckNearestTeleporter(realtarget)
			if nearestT then
				pcall(function()
                    tween:Cancel()
                end)
                requestEntrance(nearestT)
			end
			local _v2 = CFrame.new(realtarget.X, DefualtY, realtarget.Z)
			local _v1 = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X, DefualtY, game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
			if IngoreY and conc(DefualtY) < 1000 and conc(DefualtY) > 3 then
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = _v1
			end
			local TweenService = game:GetService("TweenService")
			local Info = TweenInfo.new(GetDistance(realtarget) / TweenSpeed, Enum.EasingStyle.Linear)
			tween = TweenService:Create(game:GetService("Players").LocalPlayer.Character["HumanoidRootPart"], Info, {
				CFrame = realtarget
			})
			tween:Play()
		end
	end)
    if not su then
        print(er)
    end
end

--toTarget Tween
function toTarget(...)
	local RealtargetPos = {
		...
	}
	local targetPos = RealtargetPos[1]
	local RealTarget
	if type(targetPos) == "vector" then
		RealTarget = CFrame.new(targetPos)
	elseif type(targetPos) == "userdata" then
		RealTarget = targetPos
	elseif type(targetPos) == "number" then
		RealTarget = CFrame.new(unpack(RealtargetPos))
	end
	if game.Players.LocalPlayer.Character:WaitForChild("Humanoid").Health == 0 then
		if tween then
			tween:Cancel()
		end
		repeat
			wait(0.2)
		until game.Players.LocalPlayer.Character:WaitForChild("Humanoid").Health > 0;
		wait(0.2)
	end
	local tweenfunc = {}
	local Distance = (RealTarget.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position)
        .Magnitude
	if Distance < 1000 then
		Speed = 315
	elseif Distance >= 1000 then
		Speed = 300
	end
	if getgenv().BypassTp then
		if Distance > 2500 and not getgenv().AutoNextIsland and not (game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip") or game.Players.LocalPlayer.Backpack:FindFirstChild("God's Chalice") or game.Players.LocalPlayer.Character:FindFirstChild("God's Chalice") or game.Players.LocalPlayer.Backpack:FindFirstChild("Hallow Essence") or game.Players.LocalPlayer.Character:FindFirstChild("Hallow Essence") or game.Players.LocalPlayer.Character:FindFirstChild("Sweet Chalice") or game.Players.LocalPlayer.Backpack:FindFirstChild("Sweet Chalice")) and not (Name == "Fishman Commando" or Name == "Fishman Warrior") then
			pcall(function()
				tween:Cancel()
				fkwarp = false
				if game:GetService("Players")["LocalPlayer"].Data:FindFirstChild("SpawnPoint").Value == tostring(GetIsLand(RealTarget)) then
					wait(.1)
					Com("F_", "TeleportToSpawn")
				elseif game:GetService("Players")["LocalPlayer"].Data:FindFirstChild("LastSpawnPoint").Value == tostring(GetIsLand(RealTarget)) then
					game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid"):ChangeState(15)
					wait(0.1)
					repeat
						wait(.1)
					until game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid").Health > 0
				else
					if game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid").Health > 0 then
						if fkwarp == false then
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = RealTarget
						end
						fkwarp = true
					end
					wait(.08)
					game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid"):ChangeState(15)
					repeat
						wait(getgenv().Fast_Delay)
					until game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid").Health > 0
					wait(.1)
					Com("F_", "SetSpawnPoint")
				end
				wait(0.2)
				return
			end)
		end
	end
	local tween_s = game:service "TweenService"
	local info = TweenInfo.new(
        (RealTarget.Position - game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart").Position)
        .Magnitude / Speed, Enum.EasingStyle.Linear)
	local tweenw, err = pcall(function()
		tween = tween_s:Create(game.Players.LocalPlayer.Character["HumanoidRootPart"], info, {
			CFrame = RealTarget
		})
		tween:Play()
	end)
	function tweenfunc:Stop()
		tween:Cancel()
	end
	function tweenfunc:Wait()
		tween.Completed:Wait()
	end
	return tweenfunc
end
--Get Island
function GetIsLand(...)
	local RealtargetPos = {
		...
	}
	local targetPos = RealtargetPos[1]
	local RealTarget
	if type(targetPos) == "vector" then
		RealTarget = targetPos
	elseif type(targetPos) == "userdata" then
		RealTarget = targetPos.Position
	elseif type(targetPos) == "number" then
		RealTarget = CFrame.new(unpack(RealtargetPos))
		RealTarget = RealTarget.p
	end
	local ReturnValue
	local CheckInOut = math.huge;
	if game.Players.LocalPlayer.Team then
		for i, v in pairs(game.Workspace._WorldOrigin.PlayerSpawns:FindFirstChild(tostring(game.Players.LocalPlayer.Team)):GetChildren()) do 
			local ReMagnitude = (RealTarget - v:GetModelCFrame().p).Magnitude;
			if ReMagnitude < CheckInOut then
				CheckInOut = ReMagnitude;
				ReturnValue = v.Name
			end
		end
		if ReturnValue then
			return ReturnValue
		end
	end
end
--Get Distance
function GetDistance(q)
	if typeof(q) == "CFrame" then
		return LP:DistanceFromCharacter(q.Position)
	elseif typeof(q) == "Vector3" then
		return LP:DistanceFromCharacter(q)
	end
end
--Get Com
function Com(com, ...)
	local Remote = game:GetService('ReplicatedStorage').Remotes:FindFirstChild("Comm" .. com)
	if Remote:IsA("RemoteEvent") then
		Remote:FireServer(...)
	elseif Remote:IsA("RemoteFunction") then
		Remote:InvokeServer(...)
	end
end
--BTP1
function BTP1(Position)
	game:service('VirtualInputManager'):SendKeyEvent(true, "W", false, game)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Position
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Position
	wait(1)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Position
	game.Players.LocalPlayer.Character.Head:Destroy()
	game:service('VirtualInputManager'):SendKeyEvent(false, "W", false, game)
end
function BTP1(p)
	pcall(function()
		if (p.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude >= 1500 and not getgenv().AutoNextIsland and game.Players.LocalPlayer.Character.Humanoid.Health > 0 then
			repeat
				wait()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
				wait(1)
				game.Players.LocalPlayer.Character.Head:Destroy()
				game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
			until (p.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 1500 and game.Players.LocalPlayer.Character.Humanoid.Health > 0
		end
	end)
end
--UseTool
function EquipTool(ToolSeo)
	if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSeo) then
		local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSeo)
		wait(0.5)
		game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
	end
end
--AimMas
spawn(function()
	local gg = getrawmetatable(game)
	local old = gg.__namecall
	setreadonly(gg, false)
	gg.__namecall = newcclosure(function(...)
		local method = getnamecallmethod()
		local args = {
			...
		}
		if tostring(method) == "FireServer" then
			if tostring(args[1]) == "RemoteEvent" then
				if tostring(args[2]) ~= "true" and tostring(args[2]) ~= "false" then
					if getgenv().UseSkill then
						if type(args[2]) == "vector" then
							args[2] = PositionSkillMasteryDevilFruit
						else
							args[2] = CFrame.new(PositionSkillMasteryDevilFruit)
						end
						return old(unpack(args))
					end
				end
			end
		end
		return old(...)
	end)
end)
--Body
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().TweenToGear or getgenv().AutoRengoku or getgenv().AutoBartiloQuest or getgenv().GetPoleV1 or getgenv().GetSaber or getgenv().AutoEvoRace or getgenv().CastleRaid or getgenv().CollectAzure or getgenv().TweenToKitsune or getgenv().AutoCandy or getgenv().GhostShip or getgenv().Ship or getgenv().SailBoat or getgenv().Auto_Holy_Torch or getgenv().Tweenfruit or getgenv().FindMirageIsland or getgenv().TeleportPly or getgenv().AutoFishCrew or getgenv().AutoShark or getgenv().AutoMysticIsland or getgenv().AutoCakeV2 or getgenv().AutoQuestRace or getgenv().AutoBuyBoat or getgenv().dao or getgenv().AutoFarmAcient or getgenv().AutoMirage or getgenv().Auto_Law or getgenv().AutoQuestRace or getgenv().AutoAllBoss or getgenv().AutoHolyTorch or getgenv().GetTushita or getgenv().farmpiranya or getgenv().AutoTerrorshark or getgenv().AutoNear or getgenv().AutoCakeV2V2 or getgenv().AutoSeaBeast or getgenv().DriveMytic or getgenv().BossRaid or getgenv().GrabChest or getgenv().Ectoplasm or AutoEvoRace or AutoBartilo or AutoFactory or BringChestz or BringFruitz or getgenv().AutoLevel or getgenv().Clip2 or AutoFarmNoQuest or getgenv().AutoBone or AutoFarmSelectMonsterQuest or AutoFarmSelectMonsterNoQuest or getgenv().AutoBoss or getgenv().AutoMasFruit or getgenv().AutoHallowSycthe or AutoCavander or getgenv().GetTushita or AutoDarkDagger or getgenv().CakePrince or getgenv().AutoElite or AutoRainbowHaki or AutoSaber or AutoFarmKen or AutoKenHop or AutoKenV2 or getgenv().AutoKillPlayerMelee or getgenv().AutoKillPlayerGun or getgenv().AutoKillPlayerFruit or getgenv().AutoNextIsland or getgenv().AutoMaterial or getgenv().Factory or getgenv().SwanGlasses or getgenv().Ectoplasm then
				if not game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
					local Noclip = Instance.new("BodyVelocity")
					Noclip.Name = "BodyClip"
					Noclip.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
					Noclip.MaxForce = Vector3.new(100000, 100000, 100000)
					Noclip.Velocity = Vector3.new(0, 0, 0)
				end
			else
				game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
			end
		end)
	end
end)
--NoClipFarm
spawn(function()
	pcall(function()
		game:GetService("RunService").Stepped:Connect(function()
			if getgenv().TweenToGear or getgenv().AutoRengoku or getgenv().AutoBartiloQuest or getgenv().GetPoleV1 or getgenv().GetSaber or getgenv().AutoEvoRace or getgenv().CastleRaid or getgenv().CollectAzure or getgenv().TweenToKitsune or getgenv().AutoCandy or getgenv().GhostShip or getgenv().Ship or getgenv().SailBoat or getgenv().Auto_Holy_Torch or getgenv().Tweenfruit or getgenv().FindMirageIsland or getgenv().TeleportPly or getgenv().AutoFishCrew or getgenv().AutoShark or getgenv().AutoMysticIsland or getgenv().AutoCakeV2 or getgenv().AutoQuestRace or getgenv().AutoBuyBoat or getgenv().dao or getgenv().AutoFarmAcient or getgenv().AutoMirage or getgenv().Auto_Law or getgenv().AutoQuestRace or getgenv().AutoAllBoss or getgenv().AutoHolyTorch or getgenv().GetTushita or getgenv().farmpiranya or getgenv().AutoTerrorshark or getgenv().AutoNear or getgenv().AutoCakeV2V2 or PirateShip or getgenv().AutoSeaBeast or getgenv().DriveMytic or getgenv().BossRaid or getgenv().GrabChest or AutoCitizen or getgenv().Ectoplasm or AutoEvoRace or AutoBartilo or AutoFactory or BringChestz or BringFruitz or getgenv().AutoLevel or getgenv().Clip2 or AutoFarmNoQuest or getgenv().AutoBone or AutoFarmSelectMonsterQuest or AutoFarmSelectMonsterNoQuest or getgenv().AutoBoss or AutoFarmBossQuest or AutoFarmMasGun or getgenv().AutoMasFruit or AutoFarmSelectArea or AutoSecondSea or AutoThirdSea or AutoDeathStep or AutoSuperhuman or AutoSharkman or AutoElectricClaw or AutoDragonTalon or AutoGodhuman or AutoRengoku or AutoBuddySword or AutoPole or getgenv().AutoHallowSycthe or AutoCavander or getgenv().GetTushita or AutoDarkDagger or getgenv().CakePrince or getgenv().AutoElite or AutoRainbowHaki or AutoSaber or AutoFarmKen or AutoKenHop or AutoKenV2 or getgenv().AutoKillPlayerMelee or getgenv().AutoKillPlayerGun or getgenv().AutoKillPlayerFruit or getgenv().AutoNextIsland or getgenv().AutoMaterial or getgenv().Factory or getgenv().SwanGlasses or getgenv().Ectoplasm then
				for i, v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
					if v:IsA("BasePart") then
						v.CanCollide = false
					end
				end
			end
		end)
	end)
end)

NoAttackAnimation = true
local DmgAttack = game:GetService("ReplicatedStorage").Assets.GUI:WaitForChild("DamageCounter")
local PC = require(game.Players.LocalPlayer.PlayerScripts.CombatFramework.Particle)
local RL = require(game:GetService("ReplicatedStorage").CombatFramework.RigLib)
local oldRL = RL.wrapAttackAnimationAsync
RL.wrapAttackAnimationAsync = function(a, b, c, d, func)
	if not NoAttackAnimation then
		return oldRL(a, b, c, 60, func)
	end

	local Hits = {}
	local Client = game.Players.LocalPlayer
	local Characters = game:GetService("Workspace").Characters:GetChildren()
	for i, v in pairs(Characters) do
		local Human = v:FindFirstChildOfClass("Humanoid")
		if v.Name ~= game.Players.LocalPlayer.Name and Human and Human.RootPart and Human.Health > 0 and Client:DistanceFromCharacter(Human.RootPart.Position) < 65 then
			table.insert(Hits, Human.RootPart)
		end
	end
	local Enemies = game:GetService("Workspace").Enemies:GetChildren()
	for i, v in pairs(Enemies) do
		local Human = v:FindFirstChildOfClass("Humanoid")
		if Human and Human.RootPart and Human.Health > 0 and Client:DistanceFromCharacter(Human.RootPart.Position) < 65 then
			table.insert(Hits, Human.RootPart)
		end
	end
	a:Play(0.01, 0.01, 0.01)
	pcall(func, Hits)
end

getAllBladeHits = function(Sizes)
	local Hits = {}
	local Client = game.Players.LocalPlayer
	local Enemies = game:GetService("Workspace").Enemies:GetChildren()
	for i, v in pairs(Enemies) do
		local Human = v:FindFirstChildOfClass("Humanoid")
		if Human and Human.RootPart and Human.Health > 0 and Client:DistanceFromCharacter(Human.RootPart.Position) < Sizes + 5 then
			table.insert(Hits, Human.RootPart)
		end
	end
	return Hits
end

getAllBladeHitsPlayers = function(Sizes)
	local Hits = {}
	local Client = game.Players.LocalPlayer
	local Characters = game:GetService("Workspace").Characters:GetChildren()
	for i, v in pairs(Characters) do
		local Human = v:FindFirstChildOfClass("Humanoid")
		if v.Name ~= game.Players.LocalPlayer.Name and Human and Human.RootPart and Human.Health > 0 and Client:DistanceFromCharacter(Human.RootPart.Position) < Sizes + 5 then
			table.insert(Hits, Human.RootPart)
		end
	end
	return Hits
end

local CombatFramework = require(game:GetService("Players").LocalPlayer.PlayerScripts:WaitForChild("CombatFramework"))
local CombatFrameworkR = getupvalue and getupvalue(CombatFramework, 2) or debug and debug.getupvalue and debug.getupvalue(CombatFramework, 2) or getupvalues and getupvalues(CombatFramework)[2] or debug.getupvalues and debug.getupvalues(CombatFramework)[2]
local RigEven = game:GetService("ReplicatedStorage").RigControllerEvent
local AttackAnim = Instance.new("Animation")
local AttackCoolDown = 0
local cooldowntickFire = 0
local MaxFire = 10000
local FireCooldown = 0.06
local FireL = 0
local bladehit = {}

CancelCoolDown = function()
	local ac = CombatFrameworkR.activeController
	if ac and ac.equipped then
		AttackCoolDown = tick() + (FireCooldown or 0.01) + ((FireL / MaxFire) * 0.3)
		RigEven.FireServer(RigEven, "weaponChange", ac.currentWeaponModel.Name)
		FireL = FireL + 1
		fask.delay((FireCooldown or 0.01) + ((FireL + 0.3 / MaxFire) * 0.3), function()
			FireL = FireL - 1
		end)
	end
end

AttackFunction = function(typef)
	local ac = CombatFrameworkR.activeController
	if ac and ac.equipped then
		local bladehit = {}
		if typef == 1 then
			bladehit = getAllBladeHits(60)
		elseif typef == 2 then
			bladehit = getAllBladeHitsPlayers(65)
		else
			for i2, v2 in pairs(getAllBladeHits(55)) do
				table.insert(bladehit, v2)
			end
			for i3, v3 in pairs(getAllBladeHitsPlayers(55)) do
				table.insert(bladehit, v3)
			end
		end
		if #bladehit > 0 then
			pcall(fask.spawn, ac.attack, ac)
			if tick() > AttackCoolDown then
				CancelCoolDown()
			end
			if tick() - cooldowntickFire > 0.3 then
				ac.timeToNextAttack = 0
				ac.hitboxMagnitude = 60
				pcall(fask.spawn, ac.attack, ac)
				cooldowntickFire = tick()
			end
			local AMI3 = ac.anims.basic[3]
			local AMI2 = ac.anims.basic[2]
			local REALID = AMI3 or AMI2
			AttackAnim.AnimationId = REALID
			local StartP = ac.humanoid:LoadAnimation(AttackAnim)
			StartP:Play(0.01, 0.01, 0.01)
			RigEven.FireServer(RigEven, "hit", bladehit, AMI3 and 3 or 2, "")
			fask.delay(0.01, function()
				StartP:Stop()
			end)
		end
	end
end

function CheckStun()
	if game:GetService('Players').LocalPlayer.Character:FindFirstChild("Stun") then
		return game:GetService('Players').LocalPlayer.Character.Stun.Value ~= 0
	end
	return false
end

function TryAttack()
    if getgenv().DameAura then
        fask.spawn(function()
            pcall(fask.spawn, AttackFunction, 3)
        end)
    elseif getgenv().UseFastAttackPlr then
        fask.spawn(function()
            pcall(fask.spawn, AttackFunction, 2)
        end)
    else
        fask.spawn(function()
            pcall(fask.spawn, AttackFunction, 1)
        end)
    end
end
--Attack for Mastery
function NormalAttack()
	pcall(function()
        if not getgenv().NormalAttack then
            local CamShake = require(game.ReplicatedStorage.Util.CameraShaker)
            CamShake:Stop()
            CombatFrameworkR.activeController.attacking = false
            CombatFrameworkR.activeController.timeToNextAttack = 0
            CombatFrameworkR.activeController.hitboxMagnitude = 180
        end
    end)
    game:GetService'VirtualUser':CaptureController()
    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
end
--Auto Haki
function AutoHaki()
	if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("HasBuso") then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
	end
end
--Remove Effect
if game:GetService("ReplicatedStorage").Effect.Container:FindFirstChild("Death") then
	game:GetService("ReplicatedStorage").Effect.Container.Death:Destroy()
end
if game:GetService("ReplicatedStorage").Effect.Container:FindFirstChild("Respawn") then
	game:GetService("ReplicatedStorage").Effect.Container.Respawn:Destroy()
end
--Toggle Close - Open
local Ui = game.CoreGui:WaitForChild("RobloxGui"):WaitForChild("Modules"):FindFirstChild("dsfwefwfwdfsfasdadaxczcw")
if Ui then
	Ui:Destroy()
end
local UserInputService = game:GetService("UserInputService")
local VirtualInputManager = game:GetService("VirtualInputManager")
local TweenService = game:GetService("TweenService")
local tween = game:service"TweenService"
local RunService = game:GetService("RunService")
local LocalPlayer = game:GetService("Players").LocalPlayer
local Mouse = LocalPlayer:GetMouse()
local GuiService = game:GetService("GuiService")
local SoundClick2 = Instance.new("Sound")
SoundClick2.Name = "Sound Effect"
SoundClick2.SoundId = ""
SoundClick2.Volume = 1
SoundClick2.Parent = game.Workspace
local UIStroke = Instance.new("UIStroke")
local UICorner = Instance.new("UICorner")
local ScreenGui = Instance.new("ScreenGui")
local ImageButton = Instance.new("ImageButton")
local RobloxButton = Enum.ButtonStyle.RobloxButton
ScreenGui.Parent = game.CoreGui:WaitForChild("RobloxGui"):WaitForChild("Modules")
ScreenGui.Name = "dsfwefwfwdfsfasdadaxczcw"
ImageButton.Parent = ScreenGui
ImageButton.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
ImageButton.Size = UDim2.new(0, 45, 0, 45)
ImageButton.Draggable = true
ImageButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ImageButton.BackgroundTransparency = 1
ImageButton.Image = "rbxassetid://17795209303"
function LoadFunction()
	ImageButton.MouseEnter:Connect(function()
		TweenService:Create(
            ImageButton,
            TweenInfo.new(.2, Enum.EasingStyle.Back, Enum.EasingDirection.InOut),
            {
			Size = UDim2.new(0, 80, 0, 80)
		}
        ):Play()
	end)
	ImageButton.MouseLeave:Connect(function()
		TweenService:Create(
            ImageButton,
            TweenInfo.new(.2, Enum.EasingStyle.Back, Enum.EasingDirection.InOut),
            {
			Size = UDim2.new(0, 50, 0, 50)
		}
        ):Play()
	end)
	local LoadFocus = false
	ImageButton.MouseButton1Down:Connect(function()
		if LoadFocus == false then
			LoadFocus = false
			TweenService:Create(
                ImageButton,
                TweenInfo.new(.2, Enum.EasingStyle.Back, Enum.EasingDirection.InOut),
                {
				Rotation = 180
			}
            ):Play()
			SoundClick2:Play()
			TweenService:Create(
                ImageButton,
                TweenInfo.new(.4, Enum.EasingStyle.Quart, Enum.EasingDirection.In),
                {
				ImageTransparency = 0
			}
            ):Play()
			wait(.5)
			TweenService:Create(
                ImageButton,
                TweenInfo.new(.2, Enum.EasingStyle.Back, Enum.EasingDirection.InOut),
                {
				Rotation = 0
			}
            ):Play()
			TweenService:Create(
                ImageButton,
                TweenInfo.new(.4, Enum.EasingStyle.Quart, Enum.EasingDirection.In),
                {
				ImageTransparency = 0
			}
            ):Play()
			wait(.5)
		end
	end)
end
LoadFunction()
ImageButton.MouseButton1Down:connect(function()
	game:GetService("VirtualInputManager"):SendKeyEvent(true, Enum.KeyCode.RightControl, false, game)
	game:GetService("VirtualInputManager"):SendKeyEvent(false, Enum.KeyCode.RightControl, false, game)
end)
-------------------------------------------------------------------------------------------------------------------------------------------
--BossList
if First_Sea then
	tableBoss = {
		"The Gorilla King",
		"Bobby",
		"Yeti",
		"Mob Leader",
		"Vice Admiral",
		"Warden",
		"Chief Warden",
		"Swan",
		"Magma Admiral",
		"Fishman Lord",
		"Wysper",
		"Thunder God",
		"Cyborg",
		"Saber Expert"
	}
elseif Second_Sea then
	tableBoss = {
		"Diamond",
		"Jeremy",
		"Fajita",
		"Don Swan",
		"Smoke Admiral",
		"Cursed Captain",
		"Darkbeard",
		"Order",
		"Awakened Ice Admiral",
		"Tide Keeper"
	}
elseif Third_Sea then
	tableBoss = {
		"Stone",
		"Island Empress",
		"Kilo Admiral",
		"Captain Elephant",
		"Beautiful Pirate",
		"rip_indra True Form",
		"Longma",
		"Soul Reaper",
		"Cake Queen"
	}
end
--FarmBoss
spawn(function()
	while wait() do
		if getgenv().AutoBoss then
			pcall(function()
				if game:GetService("Workspace").Enemies:FindFirstChild(getgenv().SelectBoss) then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == getgenv().SelectBoss then
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(80, 80, 80)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
								until not getgenv().AutoBoss or not v.Parent or v.Humanoid.Health <= 0
							end
						end
					end
				else
					if game:GetService("ReplicatedStorage"):FindFirstChild(getgenv().SelectBoss) then
						toTarget(game:GetService("ReplicatedStorage"):FindFirstChild(getgenv().SelectBoss).HumanoidRootPart.CFrame * CFrame.new(5, 10, 7))
					end
				end
			end)
		end
	end
end)
--FarmLevel
spawn(function()
	while wait() do
		if getgenv().AutoLevel then
			pcall(function()
				CheckLevel()
				if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
					toTarget(CFrameQ)
					wait(1)
					if (CFrameQ.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuest, QuestLv)
					end
				elseif string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
							if v.Name == Ms then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									bringmob = true
									AutoHaki()
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.Transparency = 1
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
								until not getgenv().AutoLevel or not v.Parent or v.Humanoid.Health <= 0 or not game:GetService("Workspace").Enemies:FindFirstChild(v.Name) or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false
								bringmob = false
							end
						end
					end
				end
			end)
		end
	end
end)
--FarmMobAura
spawn(function()
	while wait(.1) do
		if getgenv().AutoNear then
			pcall(function()
				for i, v in pairs (game.Workspace.Enemies:GetChildren()) do
					if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
						if v.Name then
							if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v:FindFirstChild("HumanoidRootPart").Position).Magnitude <= 5000 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									bringmob = true
									AutoHaki()
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.Transparency = 1
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
      --Click
								until not getgenv().AutoNear or not v.Parent or v.Humanoid.Health <= 0 or not game.Workspace.Enemies:FindFirstChild(v.Name)
								bringmob = false
							end
						end
					end
				end
			end)
		end
	end
end)

--CastleRaid
spawn(function()
	while wait() do
		if getgenv().CastleRaid then
			pcall(function()
				toTarget(CFrameCastleRaid)
				local CFrameCastleRaid = CFrame.new(-5496.17432, 313.768921, -2841.53027, 0.924894512, 7.37058015e-09, 0.380223751, 3.5881019e-08, 1, -1.06665446e-07, -0.380223751, 1.12297109e-07, 0.924894512)
				if (CFrame.new(-5539.3115234375, 313.800537109375, -2972.372314453125).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 500 then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if getgenv().CastleRaid and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
							if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 2000 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until v.Humanoid.Health <= 0 or not v.Parent or not getgenv().CastleRaid
							end
						end
					end
				else
				end
			end)
		end
	end
end)
--FarmBones
spawn(function()
	while wait() do
		if getgenv().ClaimQuestBone and getgenv().AutoBone then
			pcall(function()
				local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
				if not string.find(QuestTitle, "Demonic Soul") then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
				end
				if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
					local BoneCFrame = CFrame.new(-9509.3359375, 179.22584533691406, 6078.62646484375)
					toTarget(BoneCFrame)
					wait(1)
					if (BoneCFrame.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", "HauntedQuest2", 1)
					end
				elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
					if game:GetService("Workspace").Enemies:FindFirstChild("Reborn Skeleton") or game:GetService("Workspace").Enemies:FindFirstChild("Living Zombie") or game:GetService("Workspace").Enemies:FindFirstChild("Demonic Soul") or game:GetService("Workspace").Enemies:FindFirstChild("Posessed Mummy") then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
								if v.Name == "Reborn Skeleton" or v.Name == "Living Zombie" or v.Name == "Demonic Soul" or v.Name == "Posessed Mummy" then
									if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Demonic Soul") then
										repeat
											wait(getgenv().Fast_Delay)
											TryAttack()
											AutoHaki()
											bringmob = true
											EquipTool(SelectWeapon)
											topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
											v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
											v.HumanoidRootPart.Transparency = 1
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.CanCollide = false
											FarmPos = v.HumanoidRootPart.CFrame
											MonFarm = v.Name
										until not getgenv().AutoBone or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
									else
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
										bringmob = false
									end
								end
							end
						end
					end
				end
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if not getgenv().ClaimQuestBone and getgenv().AutoBone then
			pcall(function()
				toTarget(BoneCFrame)
				for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
					if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
						if v.Name == "Reborn Skeleton" or v.Name == "Living Zombie" or v.Name == "Demonic Soul" or v.Name == "Posessed Mummy" then
							repeat
								wait(getgenv().Fast_Delay)
								TryAttack()
								AutoHaki()
								bringmob = true
								EquipTool(SelectWeapon)
								topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
								v.HumanoidRootPart.Transparency = 1
								v.Humanoid.JumpPower = 0
								v.Humanoid.WalkSpeed = 0
								v.HumanoidRootPart.CanCollide = false
								FarmPos = v.HumanoidRootPart.CFrame
								MonFarm = v.Name
							until not getgenv().AutoBone or not v.Parent or v.Humanoid.Health <= 0
							bringmob = false
						end
					end
				end
				for i, v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
					if v.Name == "Reborn Skeleton" then
						topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
					elseif v.Name == "Living Zombie" then
						topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
					elseif v.Name == "Demonic Soul" then
						topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
					elseif v.Name == "Posessed Mummy" then
						topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
					end
				end
			end)
		end
	end
end)
--RandomBone
spawn(function()
	while wait(0.00001) do
		if getgenv().AutoRandomBone then
			local args = {
				[1] = "Bones",
				[2] = "Buy",
				[3] = 1,
				[4] = 1
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end
	end
end)
--FarmCakePrince
spawn(function()
	while wait() do
		if getgenv().CakePrince then
			pcall(function()
				local CakeCFrame = CFrame.new(-2325.01708984375, 228.95822143554688, -12366.138671875)
				toTarget(CakeCFrame)
				if game.ReplicatedStorage:FindFirstChild("Cake Prince") or game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince") then
					if game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince") then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v.Name == "Cake Prince" then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.CanCollide = false
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until getgenv().CakePrince == false or not v.Parent or v.Humanoid.Health <= 0
								bringmob = false
							end
						end
					else
						topos(CFrame.new(-2009.2802734375, 4532.97216796875, -14937.3076171875))
					end
				else
					if game.Workspace.Enemies:FindFirstChild("Baking Staff") or game.Workspace.Enemies:FindFirstChild("Head Baker") or game.Workspace.Enemies:FindFirstChild("Cake Guard") or game.Workspace.Enemies:FindFirstChild("Cookie Crafter")  then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if (v.Name == "Baking Staff" or v.Name == "Head Baker" or v.Name == "Cake Guard" or v.Name == "Cookie Crafter") and v.Humanoid.Health > 0 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									bringmob = true
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until getgenv().CakePrince == false or game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince") or not v.Parent or v.Humanoid.Health <= 0
								bringmob = false
							end
						end
					else
					end
				end
			end)
		end
	end
end)
--SpawnBossCake
spawn(function()
	while wait() do
		if getgenv().SpawnCakePrince then
			local args = {
				[1] = "CakePrinceSpawner",
				[2] = true
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			local args = {
				[1] = "CakePrinceSpawner"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end
	end
end)
--FarmEctoplasms
spawn(function()
	while wait(.1) do
		pcall(function()
			if getgenv().Ectoplasm then
				if game:GetService("Workspace").Enemies:FindFirstChild("Ship Deckhand") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Engineer") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Steward") or game:GetService("Workspace").Enemies:FindFirstChild("Ship Officer") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Ship Steward" or v.Name == "Ship Engineer" or v.Name == "Ship Deckhand" or v.Name == "Ship Officer" and v:FindFirstChild("Humanoid") then
							if v.Humanoid.Health > 0 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									bringmob = true
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.Transparency = 1
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
								until getgenv().Ectoplasm == false or not v.Parent or v.Humanoid.Health == 0 or not game:GetService("Workspace").Enemies:FindFirstChild(v.Name)
								bringmob = false
							end
						end
					end
				else
					local Distance = (Vector3.new(904.4072265625, 181.05767822266, 33341.38671875) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
					if Distance > 20000 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
					end
					topos(CFrame.new(904.4072265625, 181.05767822266, 33341.38671875))
				end
			end
		end)
	end
end)
--FarmMaterials
spawn(function()
	while wait() do
		if getgenv().AutoMaterial then
			pcall(function()
				MaterialMon(getgenv().SelectMaterial)
				toTarget(MPos)
				if game:GetService("Workspace").Enemies:FindFirstChild(MMon) then
					for i, v in pairs (game.Workspace.Enemies:GetChildren()) do
						if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
							if v.Name == MMon then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									bringmob = true
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.Transparency = 1
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
								until not getgenv().AutoMaterial or not v.Parent or v.Humanoid.Health <= 0
								bringmob = false
							end
						end
					end
				else
					for i, v in pairs(game:GetService("Workspace")["_WorldOrigin"].EnemySpawns:GetChildren()) do
						if string.find(v.Name, Mon) then
							if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.Position).Magnitude >= 10 then
								topos(v.CFrame * CFrame.new(posX, posY, posZ))
							end
						end
					end
				end
			end)
		end
	end
end)
--FarmElite
spawn(function()
	while wait() do
		if getgenv().AutoElite then
			pcall(function()
				if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
					if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Diablo") or string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Deandre") or string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Urban") then
						if game:GetService("Workspace").Enemies:FindFirstChild("Diablo") or game:GetService("Workspace").Enemies:FindFirstChild("Deandre") or game:GetService("Workspace").Enemies:FindFirstChild("Urban") then
							for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
									if v.Name == "Diablo" or v.Name == "Deandre" or v.Name == "Urban" then
										repeat
											wait(getgenv().Fast_Delay)
											TryAttack()
											EquipTool(SelectWeapon)
											AutoHaki()
											topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
											MonsterPosition = v.HumanoidRootPart.CFrame
											v.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
											v.Humanoid.JumpPower = 0
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.CanCollide = false
											v.HumanoidRootPart.Size = Vector3.new(1, 1, 1)
										until getgenv().AutoElite == false or v.Humanoid.Health <= 0 or not v.Parent
									end
								end
							end
						else
							if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo") then
								toTarget(game:GetService("ReplicatedStorage"):FindFirstChild("Diablo").HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
							elseif game:GetService("ReplicatedStorage"):FindFirstChild("Deandre") then
								toTarget(game:GetService("ReplicatedStorage"):FindFirstChild("Deandre").HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
							elseif game:GetService("ReplicatedStorage"):FindFirstChild("Urban") then
								toTarget(game:GetService("ReplicatedStorage"):FindFirstChild("Urban").HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
							end
						end
					end
				else
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
				end
			end)
		end
	end
end)
--BringMobs
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().BringMob and bringmob then
				for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
					if v.Name == MonFarm and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 300 then
						v.HumanoidRootPart.CFrame = FarmPos
						v.Humanoid:ChangeState(11)
						v.Humanoid:ChangeState(14)
						v.HumanoidRootPart.Size = Vector3.new(1, 1, 1)
						v.HumanoidRootPart.Transparency = 1
						for al, f in pairs(v:GetChildren()) do
							if v:IsA("BasePart") then
								v.Velocity = Vector3.new(0, 0, 0)
								v.CanCollide = 0
								v.Anchored = true
							end
						end
						v.HumanoidRootPart.CanCollide = false
						v.Head.CanCollide = false
						if v:FindFirstChild("Humanoid") then
							v.Humanoid.WalkSpeed = 0
							v.Humanoid.JumpPower = 0
						else
							return
						end
						v.Humanoid:ChangeState(11)
						v.Humanoid:ChangeState(14)
					end
					if v.Humanoid:FindFirstChild("Animator") then
						v.Humanoid.Animator:Destroy()
					end
					sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius",  math.huge)
				end
			end
		end)
	end
end)
--AutoHakiBuso
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoHakiBuso then
				if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
				end
			end
		end)
	end
end)
--FastAttackSida
spawn(function()
	while wait() do
		if getgenv().FastAttackSida then
			pcall(function()
				repeat
					wait(getgenv().Fast_Delay)
					TryAttack()
				until not getgenv().FastAttackSida
			end)
		end
	end
end)
--AutoRejoin
spawn(function()
	while wait() do
		if getgenv().AutoRejoin then
			getgenv().rejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
				if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
					game:GetService("TeleportService"):Teleport(game.PlaceId)
				end
			end)
		end
	end
end)
--RemoveDamageTexts
spawn(function()
	while wait() do
		if getgenv().RemoveDameText then
			game:GetService("ReplicatedStorage").Assets.GUI.DamageCounter.Enabled = false
		else
			game:GetService("ReplicatedStorage").Assets.GUI.DamageCounter.Enabled = true
		end
	end
end)
--RemoveNotify
spawn(function()
	while wait() do
		if getgenv().RemoveNotify then
			game.Players.LocalPlayer.PlayerGui.Notifications.Enabled = false
		else
			game.Players.LocalPlayer.PlayerGui.Notifications.Enabled = true
		end
	end
end)
--SelectWeapons
task.spawn(function()
	while wait() do
		pcall(function()
			if getgenv().ChooseWeapon == "Melee" then
				for i , v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
					if v.ToolTip == "Melee" then
						if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
							SelectWeapon = v.Name
						end
					end
				end
			elseif getgenv().ChooseWeapon == "Sword" then
				for i , v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
					if v.ToolTip == "Sword" then
						if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
							SelectWeapon = v.Name
						end
					end
				end
			elseif getgenv().ChooseWeapon == "Fruit" then
				for i , v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
					if v.ToolTip == "Blox Fruit" then
						if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
							SelectWeapon = v.Name
						end
					end
				end
			else
				for i , v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
					if v.ToolTip == "Melee" then
						if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
							SelectWeapon = v.Name
						end
					end
				end
			end
		end)
	end
end)
--SelectFastAttack
getgenv().Fast_Delay = 0.15
spawn(function()
	while wait() do
		if getgenv().SelectFastAttack then
			pcall(function()
				if getgenv().SelectFastAttack == "Normal Fast" then
					getgenv().Fast_Delay = 0.175
				elseif getgenv().SelectFastAttack == "Fast Attack" then
					getgenv().Fast_Delay = 0.15
				elseif getgenv().SelectFastAttack == "Super Fast Attack" then
					getgenv().Fast_Delay = 0.02
				end
			end)
		end
	end
end)
--Distance
posX = 0
posY = 35.5
posZ = 0
--RedeemCodes
function RedeemCode(Code)
	game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Code)
end
--Boost FPS
function FPSBooster()
	local decalsyeeted = true
	local g = game
	local w = g.Workspace
	local l = g.Lighting
	local t = w.Terrain
	sethiddenproperty(l, "Technology", 2)
	sethiddenproperty(t, "Decoration", false)
	t.WaterWaveSize = 0
	t.WaterWaveSpeed = 0
	t.WaterReflectance = 0
	t.WaterTransparency = 0
	l.GlobalShadows = false
	l.FogEnd = 9e9
	l.Brightness = 0
	settings().Rendering.QualityLevel = "Level01"
	for i, v in pairs(g:GetDescendants()) do
		if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
			v.Material = "Plastic"
			v.Reflectance = 0
		elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
			v.Transparency = 1
		elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
			v.Lifetime = NumberRange.new(0)
		elseif v:IsA("Explosion") then
			v.BlastPressure = 1
			v.BlastRadius = 1
		elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
			v.Enabled = false
		elseif v:IsA("MeshPart") then
			v.Material = "Plastic"
			v.Reflectance = 0
			v.TextureID = 10385902758728957
		end
	end
	for i, e in pairs(l:GetChildren()) do
		if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
			e.Enabled = false
		end
	end
end
--FarmFruitMastery
spawn(function()
	while wait(1) do
		if getgenv().UseSkill then
			pcall(function()
				if getgenv().UseSkill then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == MonFarm and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health <= v.Humanoid.MaxHealth * getgenv().HealthMob / 100 then
							repeat
								game:GetService("RunService").Heartbeat:wait()
								EquipTool(game.Players.LocalPlayer.Data.DevilFruit.Value)
								topos(v.HumanoidRootPart.CFrame * CFrame.new(0, 15.5, 0))
								PositionSkillMasteryDevilFruit = v.HumanoidRootPart.Position
								if game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value) then
									game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value).MousePos.Value = PositionSkillMasteryDevilFruit
									local DevilFruitMastery = game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Data.DevilFruit.Value).Level.Value
									if getgenv().Z and DevilFruitMastery >= 1 then
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "Z", false, game)
										game:GetService("VirtualInputManager"):SendKeyEvent(false, "Z", false, game)
									end
									if getgenv().X and DevilFruitMastery >= 1 then
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "X", false, game)
										game:GetService("VirtualInputManager"):SendKeyEvent(false, "X", false, game)
									end
									if getgenv().C and DevilFruitMastery >= 1 then
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "C", false, game)
										game:GetService("VirtualInputManager"):SendKeyEvent(false, "C", false, game)
									end
									if getgenv().V and DevilFruitMastery >= 1 then
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "V", false, game)
										game:GetService("VirtualInputManager"):SendKeyEvent(false, "V", false, game)
									end
									if getgenv().F and DevilFruitMastery >= 1 then
										game:GetService("VirtualInputManager"):SendKeyEvent(true, "F", false, game)
										game:GetService("VirtualInputManager"):SendKeyEvent(false, "F", false, game)
									end
								end
							until not getgenv().AutoMasFruit or not getgenv().UseSkill or v.Humanoid.Health == 0
						end
					end
				end
			end)
		end
	end
end)
spawn(function()
	while wait(.1) do
		if getgenv().AutoMasFruit and getgenv().TypeMastery == 'Level' then
			pcall(function()
				if getgenv().AutoMasFruit == true then
					getgenv().FastAttackSida = false
				else
					getgenv().FastAttackSida = true
				end
				CheckLevel(SelectMonster)
				if not string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
					toTarget(CFrameQ)
					if (CFrameQ.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuest, QuestLv)
					end
				elseif string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
							if v.Name == Ms then
								repeat
									wait(.1)
									if v.Humanoid.Health <= v.Humanoid.MaxHealth * getgenv().HealthMob / 100 then
										getgenv().UseSkill = true
									else
										getgenv().UseSkill = false
										AutoHaki()
										bringmob = true
										EquipTool(SelectWeapon)
										topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, 45.5, posZ))
										v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
										v.HumanoidRootPart.Transparency = 1
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.CanCollide = false
										FarmPos = v.HumanoidRootPart.CFrame
										MonFarm = v.Name
        --getgenv().FastAttackSida = false
										NormalAttack()
									end
								until not getgenv().AutoMasFruit or not v.Parent or v.Humanoid.Health == 0 or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false or not game:GetService("Workspace").Enemies:FindFirstChild(v.Name) or not getgenv().TypeMastery == 'Level'
								bringmob = false
        --getgenv().FastAttackSida = true
								getgenv().UseSkill = false
							end
						end
					end
				end
			end)
		elseif getgenv().AutoMasFruit and getgenv().TypeMastery == 'Mob Aura' then
			pcall(function()
				for i, v in pairs (game.Workspace.Enemies:GetChildren()) do
					if v.Name and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
						if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v:FindFirstChild("HumanoidRootPart").Position).Magnitude <= 5000 then
							repeat
								wait(.1)
								if v.Humanoid.Health <= v.Humanoid.MaxHealth * getgenv().HealthMob / 100 then
									getgenv().UseSkill = true
								else
									getgenv().UseSkill = false
									AutoHaki()
									bringmob = true
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, 45.5, posZ))
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									v.HumanoidRootPart.Transparency = 1
									v.Humanoid.JumpPower = 0
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
      --getgenv().FastAttackSida = false
									NormalAttack()
								end
							until not getgenv().AutoMasFruit or not MasteryType == 'Mob Aura' or not v.Parent or v.Humanoid.Health == 0 or not getgenv().TypeMastery == 'Mob Aura'
							bringmob = false
      --getgenv().FastAttackSida = true
							getgenv().UseSkill = false
						end
					end
				end
			end)
		end
	end
end)
--SelectMaterials
if First_Sea then
	MaterialList = {
		"Scrap Metal",
		"Leather",
		"Angel Wings",
		"Magma Ore",
		"Fish Tail"
	}
elseif Second_Sea then
	MaterialList = {
		"Scrap Metal",
		"Leather",
		"Radioactive Material",
		"Mystic Droplet",
		"Magma Ore",
		"Vampire Fang"
	}
elseif Third_Sea then
	MaterialList = {
		"Scrap Metal",
		"Leather",
		"Demonic Wisp",
		"Conjured Cocoa",
		"Dragon Scale",
		"Gunpowder",
		"Fish Tail",
		"Mini Tusk"
	}
end
--AutoEvoRace
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoEvoRace then
				local Back = game.Players.LocalPlayer.Backpack
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist", "1")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist", "2")
				if Back:FindFirstChild("Flower 2") then
					if Back:FindFirstChild("Flower 1") then
						topos(CFrame.new(-5497.06152, 47.5923004, -795.237061))
						for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
							if v.Name == "Zombie" then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until Back:FindFirstChild("Flower 3")
							end
						end
					else
						topos(game.Workspace["Flower1"].CFrame)
					end
				else
					topos(game.Workspace["Flower2"].CFrame)
				end
				if Back:FindFirstChild("Flower 1") and Back:FindFirstChild("Flower 2") and Back:FindFirstChild("Flower 3") then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist", "1")
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist", "3")
				end
				for i, v in pairs(game.Workspace:GetChildren()) do
					if v.Name == "Flower1" or v.Name == "Flower2" then
						v.Size = Vector3.new(20, 20, 20)
					end
				end
			end
		end)
	end
end)
--FarmFactory
spawn(function()
	while wait() do
		if getgenv().Factory then
			if game.Workspace.Enemies:FindFirstChild("Core") then
				for i, v in pairs(game.Workspace.Enemies:GetChildren()) do
					if v.Name == "Core" and v.Humanoid.Health > 0 then
						repeat
							wait(getgenv().Fast_Delay)
							TryAttack()
							EquipTool(SelectWeapon)
							AutoHaki()
							topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							v.HumanoidRootPart.Transparency = 1
							v.Humanoid.JumpPower = 0
							v.Humanoid.WalkSpeed = 0
							v.HumanoidRootPart.CanCollide = false
							FarmPos = v.HumanoidRootPart.CFrame
							MonFarm = v.Name
						until not v.Parent or v.Humanoid.Health <= 0  or getgenv().Factory == false
					end
				end
			elseif game.ReplicatedStorage:FindFirstChild("Core") then
				repeat
					topos(CFrame.new(448.46756, 199.356781, -441.389252))
					wait()
				until not getgenv().Factory or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(448.46756, 199.356781, -441.389252)).Magnitude <= 10
			end
		end
	end
end)
--AutoStats
spawn(function()
	while wait() do
		if getgenv().AutoAddStats then
			if getgenv().SelectAddStats == "Demon Fruit" then
				local args = {
					[1] = "AddPoint",
					[2] = "Demon Fruit",
					[3] = 10
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			elseif getgenv().SelectAddStats == "Gun" then
				local args = {
					[1] = "AddPoint",
					[2] = "Gun",
					[3] = 10
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			elseif getgenv().SelectAddStats == "Sword" then
				local args = {
					[1] = "AddPoint",
					[2] = "Sword",
					[3] = 10
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			elseif getgenv().SelectAddStats == "Defense" then
				local args = {
					[1] = "AddPoint",
					[2] = "Defense",
					[3] = 10
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			elseif getgenv().SelectAddStats == "Melee" then
				local args = {
					[1] = "AddPoint",
					[2] = "Melee",
					[3] = 10
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
	end
end)
--AutoSaber
spawn(function()
	while wait() do
		if getgenv().GetSaber and game.Players.LocalPlayer.Data.Level.Value >= 200 then
			pcall(function()
				if game:GetService("Workspace").Map.Jungle.Final.Part.Transparency == 0 then
					if game:GetService("Workspace").Map.Jungle.QuestPlates.Door.Transparency == 0 then
						if (CFrame.new(-1612.55884, 36.9774132, 148.719543, 0.37091279, 3.0717151e-09, -0.928667724, 3.97099491e-08, 1, 1.91679348e-08, 0.928667724, -4.39869794e-08, 0.37091279).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 100 then
							topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
							wait(1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate1.Button.CFrame
							wait(1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate2.Button.CFrame
							wait(1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate3.Button.CFrame
							wait(1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate4.Button.CFrame
							wait(1)
							game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate5.Button.CFrame
							wait(1)
						else
							topos(CFrame.new(-1612.55884, 36.9774132, 148.719543, 0.37091279, 3.0717151e-09, -0.928667724, 3.97099491e-08, 1, 1.91679348e-08, 0.928667724, -4.39869794e-08, 0.37091279))
						end
					else
						if game:GetService("Workspace").Map.Desert.Burn.Part.Transparency == 0 then
							if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Torch") or game.Players.LocalPlayer.Character:FindFirstChild("Torch") then
								EqiupTool("Torch")
								topos(CFrame.new(1114.61475, 5.04679728, 4350.22803, -0.648466587, -1.28799094e-09, 0.761243105, -5.70652914e-10, 1, 1.20584542e-09, -0.761243105, 3.47544882e-10, -0.648466587))
							else
								topos(CFrame.new(-1610.00757, 11.5049858, 164.001587, 0.984807551, -0.167722285, -0.0449818149, 0.17364943, 0.951244235, 0.254912198, 3.42372805e-05, -0.258850515, 0.965917408))
							end
						else
							if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "SickMan") ~= 0 then
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "GetCup")
								wait(0.5)
								EqiupTool("Cup")
								wait(0.5)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "FillCup", game:GetService("Players").LocalPlayer.Character.Cup)
								wait(0)
								game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "SickMan")
							else
								if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "RichSon") == nil then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "RichSon")
								elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "RichSon") == 0 then
									if game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader") or game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader") then
										topos(CFrame.new(-2967.59521, -4.91089821, 5328.70703, 0.342208564, -0.0227849055, 0.939347804, 0.0251603816, 0.999569714, 0.0150796166, -0.939287126, 0.0184739735, 0.342634559)) 
										for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
											if v.Name == "Mob Leader" then
												if game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader") then
													if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
														repeat
															wait(getgenv().Fast_Delay)
															TryAttack()()
															AutoHaki()
															EqiupTool(SelectWeapon)
															v.HumanoidRootPart.CanCollide = false
															v.Humanoid.WalkSpeed = 0
															v.HumanoidRootPart.Size = Vector3.new(80, 80, 80)
															topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
															sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
														until v.Humanoid.Health <= 0 or not getgenv().GetSaber
													end
												end
												if game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader") then
													topos(game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader").HumanoidRootPart.CFrame * Farm_Mode)
												end
											end
										end
									end
								elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "RichSon") == 1 then
									game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "RichSon")
									wait(0.5)
									EqiupTool("Relic")
									wait(0.5)
									topos(CFrame.new(-1404.91504, 29.9773273, 3.80598116, 0.876514494, 5.66906877e-09, 0.481375456, 2.53851997e-08, 1, -5.79995607e-08, -0.481375456, 6.30572643e-08, 0.876514494))
								end
							end
						end
					end
				else
					if game:GetService("Workspace").Enemies:FindFirstChild("Saber Expert") or game:GetService("ReplicatedStorage"):FindFirstChild("Saber Expert") then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								if v.Name == "Saber Expert" then
									repeat
										wait(getgenv().Fast_Delay)
										TryAttack()
										EqiupTool(SelectWeapon)
										topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
										v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
										v.HumanoidRootPart.Transparency = 1
										v.Humanoid.JumpPower = 0
										v.Humanoid.WalkSpeed = 0
										v.HumanoidRootPart.CanCollide = false
									until v.Humanoid.Health <= 0 or not getgenv().GetSaber
									if v.Humanoid.Health <= 0 then
										game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress", "PlaceRelic")
									end
								end
							end
						end
					end
				end
			end)
		end
	end
end)
--AutoPole
local PolePos = CFrame.new(-7748.0185546875, 5606.80615234375, -2305.898681640625)
spawn(function()
	while wait() do
		if  getgenv().GetPoleV1 then
			pcall(function()
				if game:GetService("Workspace").Enemies:FindFirstChild("Thunder God") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Thunder God" then
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								until not  getgenv().GetPoleV1 or not v.Parent or v.Humanoid.Health <= 0
							end
						end
					end
				else
					toTarget(PolePos)
					topos(CFrame.new(-7748.0185546875, 5606.80615234375, -2305.898681640625))
					if game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God") then
						topos(game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God").HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
					else
					end
				end
			end)
		end
	end
end)
--AutoRengoku
spawn(function()
	while wait() do
		if getgenv().AutoRengoku then
			pcall(function()
				if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hidden Key") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Hidden Key") then
					EqiupTool("Hidden Key")
					topos(CFrame.new(6571.1201171875, 299.23028564453, -6967.841796875))
				elseif game:GetService("Workspace").Enemies:FindFirstChild("Snow Lurker") or game:GetService("Workspace").Enemies:FindFirstChild("Arctic Warrior") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if (v.Name == "Snow Lurker" or v.Name == "Arctic Warrior") and v.Humanoid.Health > 0 then
							repeat
								wait(getgenv().Fast_Delay)
								TryAttack()
								AutoHaki()
								EquipTool(SelectWeapon)
								v.HumanoidRootPart.CanCollide = false
								v.Humanoid.WalkSpeed = 0
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								FarmPos = v.HumanoidRootPart.CFrame
								MonFarm = v.Name
								topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hidden Key") or getgenv().AutoRengoku == false or not v.Parent or v.Humanoid.Health <= 0
						end
					end
				else
					local PosRengouku = CFrame.new(5439.716796875, 84.420944213867, -6715.1635742188)
					toTarget(PosRengouku)
				end
			end)
		end
	end
end)
--AutoBartiloQuest
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().AutoBartiloQuest then
				if game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress", "Bartilo") == 0 then
					if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Swan Pirates") and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
						if game:GetService("Workspace").Enemies:FindFirstChild("Swan Pirate") then
							for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
								if v.Name == "Swan Pirate" then
									pcall(function()
										repeat
											wait(getgenv().Fast_Delay)
											TryAttack()
											AutoHaki()
											EquipTool(SelectWeapon)
											v.HumanoidRootPart.CanCollide = false
											v.Humanoid.WalkSpeed = 0
											v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
											FarmPos = v.HumanoidRootPart.CFrame
											MonFarm = v.Name
											topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
										until not v.Parent or v.Humanoid.Health <= 0 or getgenv().AutoBartiloQuest == false or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
									end)
								end
							end
						else
							repeat
								topos(CFrame.new(932.624451, 156.106079, 1180.27466, -0.973085582, 4.55137119e-08, -0.230443969, 2.67024713e-08, 1, 8.47491108e-08, 0.230443969, 7.63147128e-08, -0.973085582))
								wait()
							until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(932.624451, 156.106079, 1180.27466, -0.973085582, 4.55137119e-08, -0.230443969, 2.67024713e-08, 1, 8.47491108e-08, 0.230443969, 7.63147128e-08, -0.973085582)).Magnitude <= 10
						end
					else
						repeat
							topos(CFrame.new(-456.28952, 73.0200958, 299.895966))
							wait()
						until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-456.28952, 73.0200958, 299.895966)).Magnitude <= 10
						wait(1.1)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", "BartiloQuest", 1)
					end
				elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress", "Bartilo") == 1 then
					if game:GetService("Workspace").Enemies:FindFirstChild("Jeremy") then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v.Name == "Jeremy" then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								until not v.Parent or v.Humanoid.Health <= 0 or getgenv().AutoBartiloQuest == false
							end
						end
					elseif game:GetService("ReplicatedStorage"):FindFirstChild("Jeremy") then
						repeat
							topos(CFrame.new(-456.28952, 73.0200958, 299.895966))
							wait()
						until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-456.28952, 73.0200958, 299.895966)).Magnitude <= 10
						wait(1.1)
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress", "Bartilo")
						wait(1)
						repeat
							topos(CFrame.new(2099.88159, 448.931, 648.997375))
							wait()
						until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(2099.88159, 448.931, 648.997375)).Magnitude <= 10
						wait(2)
					else
						repeat
							topos(CFrame.new(2099.88159, 448.931, 648.997375))
							wait()
						until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(2099.88159, 448.931, 648.997375)).Magnitude <= 10
					end
				elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BartiloQuestProgress", "Bartilo") == 2 then
					repeat
						topos(CFrame.new(-1850.49329, 13.1789551, 1750.89685))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1850.49329, 13.1789551, 1750.89685)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1858.87305, 19.3777466, 1712.01807))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1858.87305, 19.3777466, 1712.01807)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1803.94324, 16.5789185, 1750.89685))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1803.94324, 16.5789185, 1750.89685)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1858.55835, 16.8604317, 1724.79541))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1858.55835, 16.8604317, 1724.79541)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1869.54224, 15.987854, 1681.00659))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1869.54224, 15.987854, 1681.00659)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1800.0979, 16.4978027, 1684.52368))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1800.0979, 16.4978027, 1684.52368)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1819.26343, 14.795166, 1717.90625))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1819.26343, 14.795166, 1717.90625)).Magnitude <= 10
					wait(1)
					repeat
						topos(CFrame.new(-1813.51843, 14.8604736, 1724.79541))
						wait()
					until not getgenv().AutoBartiloQuest or (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-1813.51843, 14.8604736, 1724.79541)).Magnitude <= 10
				end
			end
		end
	end)
end)
--AutoHallowScythe
spawn(function()
	while wait() do
		if getgenv().AutoHallowSycthe then
			pcall(function()
				if game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if string.find(v.Name , "Soul Reaper") then
							repeat
								wait(getgenv().Fast_Delay)
								TryAttack()
								AutoHaki()
								EquipTool(SelectWeapon)
								v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
								topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								v.HumanoidRootPart.Transparency = 1
								sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
							until v.Humanoid.Health <= 0 or getgenv().AutoHallowSycthe == false
						end
					end
				elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hallow Essence") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Hallow Essence") then
					wait(0.5)
					EquipTool("Hallow Essence")
					wait(1)
					repeat
						topos(CFrame.new(-8932.322265625, 146.83154296875, 6062.55078125))
						wait()
					until (CFrame.new(-8932.322265625, 146.83154296875, 6062.55078125).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 8
				else
					if game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper") then
						toTarget(game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper").HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
					else
					end
				end
			end)
		end
	end
end)
spawn(function()
	while wait(0.1) do
		if getgenv().AutoHallowSycthe then
			local args = {
				[1] = "Bones",
				[2] = "Buy",
				[3] = 1,
				[4] = 1
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end
	end
end)
--GetYama
spawn(function()
	while wait() do
		if getgenv().AutoYama then
			if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter", "Progress") >= 30 then
				repeat
					wait(.1)
					fireclickdetector(game:GetService("Workspace").Map.Waterfall.SealedKatana.Handle.ClickDetector)
				until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Yama") or not getgenv().AutoYama
			end
		end
	end
end)
--HolyTorch
spawn(function()
	while wait() do
		if getgenv().Auto_Holy_Torch then
			pcall(function()
				wait(1)
				repeat
					topos(CFrame.new(-10752, 417, -9366))
					wait()
				until not getgenv().Auto_Holy_Torch or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-10752, 417, -9366)).Magnitude <= 10
				wait(1)
				repeat
					topos(CFrame.new(-11672, 334, -9474))
					wait()
				until not getgenv().Auto_Holy_Torch or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-11672, 334, -9474)).Magnitude <= 10
				wait(1)
				repeat
					topos(CFrame.new(-12132, 521, -10655))
					wait()
				until not getgenv().Auto_Holy_Torch or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-12132, 521, -10655)).Magnitude <= 10
				wait(1)
				repeat
					topos(CFrame.new(-13336, 486, -6985))
					wait()
				until not getgenv().Auto_Holy_Torch or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-13336, 486, -6985)).Magnitude <= 10
				wait(1)
				repeat
					topos(CFrame.new(-13489, 332, -7925))
					wait()
				until not getgenv().Auto_Holy_Torch or (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Vector3.new(-13489, 332, -7925)).Magnitude <= 10
			end)
		end
	end
end)
--FarmLongma
spawn(function()
	while wait() do
		if getgenv().GetTushita then
			if game:GetService("Workspace").Enemies:FindFirstChild("Longma") then
				for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v.Name == ("Longma" or v.Name == "Longma") and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
						repeat
							wait(getgenv().Fast_Delay)
							TryAttack()
							AutoHaki()
							if not game.Players.LocalPlayer.Character:FindFirstChild(SelectWeapon) then
								wait()
								EquipTool(SelectWeapon)
							end
							v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
							v.Humanoid.JumpPower = 0
							v.Humanoid.WalkSpeed = 0
							v.HumanoidRootPart.CanCollide = false
							v.Humanoid:ChangeState(11)
							topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
						until not getgenv().GetTushita or not v.Parent or v.Humanoid.Health <= 0
					end
				end
			else
				topos(CFrame.new(-10238.875976563, 389.7912902832, -9549.7939453125))
			end
		end
	end
end)
--FarmCakeV2
spawn(function()
	while wait() do
		if getgenv().AutoCakeV2 then
			pcall(function()
				if game:GetService("Workspace").Enemies:FindFirstChild("Dough King") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Dough King" then
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.Humanoid.WalkSpeed = 0
									v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until not getgenv().AutoCakeV2 or not v.Parent or v.Humanoid.Health <= 0
							end
						end
					end
				else
					if game:GetService("ReplicatedStorage"):FindFirstChild("Dough King") then
						topos(game:GetService("ReplicatedStorage"):FindFirstChild("Dough King").HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
					else
					end
				end
			end)
		end
	end
end)
--CastleRaid
spawn(function()
	while wait() do
		if getgenv().CastleRaid then
			pcall(function()
				local CFrameCastleRaid = CFrame.new(-5496.17432, 313.768921, -2841.53027, 0.924894512, 7.37058015e-09, 0.380223751, 3.5881019e-08, 1, -1.06665446e-07, -0.380223751, 1.12297109e-07, 0.924894512)
				if (CFrame.new(-5539.3115234375, 313.800537109375, -2972.372314453125).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 500 then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if getgenv().CastleRaid and v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
							if (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 2000 then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until v.Humanoid.Health <= 0 or not v.Parent or not getgenv().CastleRaid
							end
						end
					end
				else
					toTarget(CFrameCastleRaid)
				end
			end)
		end
	end
end)
--BuyTTK
spawn(function()
	while wait(.1) do
		pcall(function()
			if getgenv().BuyLengendSword then
				local args = {
					[1] = "LegendarySwordDealer",
					[2] = "2"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			else
				wait(2)
			end
		end)
	end
end)
--BuyHakiColor
spawn(function()
	while wait() do
		if getgenv().Auto_Buy_Enchancement then
			local args = {
				[1] = "ColorsDealer",
				[2] = "2"
			}
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
		end
	end
end)
--TeleportoPlayer
spawn(function()
	while wait() do
		if getgenv().TeleportPly then
			pcall(function()
				if game.Players:FindFirstChild(getgenv().SelectPly) then
					toTarget(game.Players[getgenv().SelectPly].Character.HumanoidRootPart.CFrame)
				end
			end)
		end
	end
end)
--TurnRaceV3
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().TurnRaceV3 then
				game:GetService("VirtualInputManager"):SendKeyEvent(true, "T", false, game)
				wait(.1)
				game:GetService("VirtualInputManager"):SendKeyEvent(false, "T", false, game)
			end
		end)
	end
end)
--TurnRaceV4
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().TurnRaceV4 then
				game:GetService("VirtualInputManager"):SendKeyEvent(true, "Y", false, game)
				wait(.1)
				game:GetService("VirtualInputManager"):SendKeyEvent(false, "Y", false, game)
			end
		end)
	end
end)
--NoClip
spawn(function()
	pcall(function()
		game:GetService("RunService").Stepped:Connect(function()
			if getgenv().LOf then
				for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
					if v:IsA("BasePart") then
						v.CanCollide = false
					end
				end
			end
		end)
	end)
end)
--SuperSpeed
spawn(function()
	while wait() do
		if getgenv().RunSpeed then
			InfAb()
		end
	end
end)
function InfAb()
	if getgenv().RunSpeed then
		if not game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
			local inf = Instance.new("ParticleEmitter")
			inf.Acceleration = Vector3.new(0, 0, 0)
			inf.Archivable = true
			inf.Drag = 20
			inf.EmissionDirection = Enum.NormalId.Top
			inf.Enabled = true
			inf.Lifetime = NumberRange.new(0, 0)
			inf.LightInfluence = 0
			inf.LockedToPart = true
			inf.Name = "Agility"
			inf.Rate = 500
			local numberKeypoints2 = {
				NumberSequenceKeypoint.new(0, 0);
				NumberSequenceKeypoint.new(1, 4);
			}
			inf.Size = NumberSequence.new(numberKeypoints2)
			inf.RotSpeed = NumberRange.new(9999, 99999)
			inf.Rotation = NumberRange.new(0, 0)
			inf.Speed = NumberRange.new(30, 30)
			inf.SpreadAngle = Vector2.new(0, 0, 0, 0)
			inf.Texture = ""
			inf.VelocityInheritance = 0
			inf.ZOffset = 2
			inf.Transparency = NumberSequence.new(0)
			inf.Color = ColorSequence.new(Color3.fromRGB(0, 0, 0), Color3.fromRGB(0, 0, 0))
			inf.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
		end
	else
		if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
			game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
		end
	end
end
--WalkonWater
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().WalkonWater then
				game:GetService("Workspace").Map["WaterBase-Plane"].Size = Vector3.new(1000, 112, 1000)
			else
				game:GetService("Workspace").Map["WaterBase-Plane"].Size = Vector3.new(1000, 80, 1000)
			end
		end)
	end
end)
--AutoTurnPvp
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().EnabledPvP then
				if game:GetService("Players").LocalPlayer.PlayerGui.Main.PvpDisabled.Visible == true then
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EnablePvp")
				end
			end
		end
	end)
end)
--IslandList
if First_Sea then
	IslandList = {
		"WindMill",
		"Marine",
		"Middle Town",
		"Jungle",
		"Pirate Village",
		"Desert",
		"Snow Island",
		"MarineFord",
		"Colosseum",
		"Sky Island 1",
		"Sky Island 2",
		"Sky Island 3",
		"Prison",
		"Magma Village",
		"Under Water Island",
		"Fountain City",
		"Shank Room",
		"Mob Island",
	}
elseif Second_Sea then
	IslandList = {
		"The Cafe",
		"Frist Spot",
		"Dark Area",
		"Flamingo Mansion",
		"Flamingo Room",
		"Green Zone",
		"Factory",
		"Colossuim",
		"Zombie Island",
		"Two Snow Mountain",
		"Punk Hazard",
		"Cursed Ship",
		"Ice Castle",
		"Forgotten Island",
		"Ussop Island",
		"Mini Sky Island",
	}
elseif Third_Sea then
	IslandList = {
		"Mansion",
		"Port Town",
		"Great Tree",
		"Castle On The Sea",
		"MiniSky",
		"Hydra Island",
		"Floating Turtle",
		"Haunted Castle",
		"Ice Cream Island",
		"Peanut Island",
		"Cake Island",
		"Cocoa Island",
		"Candy Island",
		"Tiki Outpost",
	}
end
--Local
local Discovery = CFrame.new(posX, posY, posZ)
local P = game:GetService("Players")
local LP = P.LocalPlayer
local PG = LP.PlayerGui
local RS = game:GetService("ReplicatedStorage")
local Remotes = RS:WaitForChild("Remotes")
local Remote = Remotes:WaitForChild("CommF_")
local RunS = game:GetService("RunService")
local Loop = RunS.RenderStepped
local Data = LP.Data
local WS = game:GetService("Workspace")
local WO = WS["_WorldOrigin"]
local VU = game:GetService("VirtualUser")
local EnemySpawns = WO.EnemySpawns
local Enemies = WS.Enemies
local CameraShaker = require(RS.Util.CameraShaker)
local GuideModule = require(RS.GuideModule)
local Quests = require(RS.Quests)
local VIM = game:service("VirtualInputManager")
local Remote_GetFruits = game.ReplicatedStorage:FindFirstChild("Remotes").CommF_:InvokeServer("GetFruits");
--FruitsList
Table_DevilFruitSniper = {}
ShopDevilSell = {}
for i, v in next, Remote_GetFruits do
	table.insert(Table_DevilFruitSniper, v.Name)
	if v.OnSale then
		table.insert(ShopDevilSell, v.Name)
	end
end
--BuyFruit
spawn(function()
	pcall(function()
		while wait(.1) do
			if getgenv().AutoBuyFruitSniper then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PurchaseRawFruit", getgenv().SelectFruit, false)
			end
		end
	end)
end)
--RandomFruit
spawn(function()
	pcall(function()
		while wait(.1) do
			if getgenv().RandomFruits then
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin", "Buy")
			end
		end
	end)
end)
--StoreFruit
function StoreFruit()
	for i, v in pairs(LP.Backpack:GetChildren()) do
		if v:IsA("Tool") and string.find(v.Name, "Fruit") then
			RS.Remotes.CommF_:InvokeServer("StoreFruit", v:GetAttribute("OriginalName"), v)
		end
	end
end
--CollectFruit
spawn(function()
	while wait(.1) do
		if getgenv().CollectFruitTP then
			for i, v in pairs(WS:GetChildren()) do
				if string.find(v.Name, "Fruit") then
					game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame
				end
			end
		end
		if getgenv().StoreFruit then
			StoreFruit()
		end
	end
end)
--FunctionEsp
function UpdateIslandESP()
	for i, v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
		pcall(function()
			if IslandESP then
				if v.Name ~= "Sea" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "GothamBold"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(8, 0, 0)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function isnil(thing)
	return (thing == nil)
end
local function round(n)
	return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
	for i, v in pairs(game:GetService'Players':GetChildren()) do
		pcall(function()
			if not isnil(v.Character) then
				if ESPPlayer then
					if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v.Character.Head)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v.Character.Head
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size10"
						name.TextWrapped = true
						name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude / 3) .. ' Distance')
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						if v.Team == game.Players.LocalPlayer.Team then
							name.TextColor3 = Color3.new(0, 0, 254)
						else
							name.TextColor3 = Color3.new(255, 0, 0)
						end
					else
						v.Character.Head['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' | ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude / 3) .. ' Distance\nHealth : ' .. round(v.Character.Humanoid.Health * 100 / v.Character.Humanoid.MaxHealth) .. '%')
					end
				else
					if v.Character.Head:FindFirstChild('NameEsp' .. Number) then
						v.Character.Head:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateChestChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if string.find(v.Name, "Chest") then
				if ChestESP then
					if string.find(v.Name, "Chest") then
						if not v:FindFirstChild('NameEsp' .. Number) then
							local bill = Instance.new('BillboardGui', v)
							bill.Name = 'NameEsp' .. Number
							bill.ExtentsOffset = Vector3.new(0, 1, 0)
							bill.Size = UDim2.new(1, 200, 1, 30)
							bill.Adornee = v
							bill.AlwaysOnTop = true
							local name = Instance.new('TextLabel', bill)
							name.Font = Enum.Font.GothamSemibold
							name.FontSize = "Size14"
							name.TextWrapped = true
							name.Size = UDim2.new(1, 0, 1, 0)
							name.TextYAlignment = 'Top'
							name.BackgroundTransparency = 1
							name.TextStrokeTransparency = 0.5
							if v.Name == "Chest1" then
								name.TextColor3 = Color3.fromRGB(109, 109, 109)
								name.Text = ("Chest 1" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
							if v.Name == "Chest2" then
								name.TextColor3 = Color3.fromRGB(173, 158, 21)
								name.Text = ("Chest 2" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
							if v.Name == "Chest3" then
								name.TextColor3 = Color3.fromRGB(85, 255, 255)
								name.Text = ("Chest 3" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
						else
							v['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
						end
					end
				else
					if v:FindFirstChild('NameEsp' .. Number) then
						v:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateDevilChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if DevilFruitESP then
				if string.find(v.Name, "Fruit") then
					if not v.Handle:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v.Handle)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v.Handle
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(255, 255, 255)
						name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
					else
						v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
					end
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end)
	end
end
function UpdateFlowerChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if v.Name == "Flower2" or v.Name == "Flower1" then
				if FlowerESP then
					if not v:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(255, 0, 0)
						if v.Name == "Flower1" then
							name.Text = ("Blue Flower" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							name.TextColor3 = Color3.fromRGB(0, 0, 255)
						end
						if v.Name == "Flower2" then
							name.Text = ("Red Flower" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							name.TextColor3 = Color3.fromRGB(255, 0, 0)
						end
					else
						v['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
					end
				else
					if v:FindFirstChild('NameEsp' .. Number) then
						v:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateRealFruitChams()
	for i, v in pairs(game.Workspace.AppleSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(255, 0, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
	for i, v in pairs(game.Workspace.PineappleSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(255, 174, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
	for i, v in pairs(game.Workspace.BananaSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(251, 255, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
end

function UpdateIslandESP()
	for i, v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
		pcall(function()
			if IslandESP then
				if v.Name ~= "Sea" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "GothamBold"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(7, 236, 240)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function isnil(thing)
	return (thing == nil)
end
local function round(n)
	return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
	for i, v in pairs(game:GetService'Players':GetChildren()) do
		pcall(function()
			if not isnil(v.Character) then
				if ESPPlayer then
					if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v.Character.Head)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v.Character.Head
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude / 3) .. ' Distance')
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						if v.Team == game.Players.LocalPlayer.Team then
							name.TextColor3 = Color3.new(0, 255, 0)
						else
							name.TextColor3 = Color3.new(255, 0, 0)
						end
					else
						v.Character.Head['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' | ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude / 3) .. ' Distance\nHealth : ' .. round(v.Character.Humanoid.Health * 100 / v.Character.Humanoid.MaxHealth) .. '%')
					end
				else
					if v.Character.Head:FindFirstChild('NameEsp' .. Number) then
						v.Character.Head:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateChestChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if string.find(v.Name, "Chest") then
				if ChestESP then
					if string.find(v.Name, "Chest") then
						if not v:FindFirstChild('NameEsp' .. Number) then
							local bill = Instance.new('BillboardGui', v)
							bill.Name = 'NameEsp' .. Number
							bill.ExtentsOffset = Vector3.new(0, 1, 0)
							bill.Size = UDim2.new(1, 200, 1, 30)
							bill.Adornee = v
							bill.AlwaysOnTop = true
							local name = Instance.new('TextLabel', bill)
							name.Font = Enum.Font.GothamSemibold
							name.FontSize = "Size14"
							name.TextWrapped = true
							name.Size = UDim2.new(1, 0, 1, 0)
							name.TextYAlignment = 'Top'
							name.BackgroundTransparency = 1
							name.TextStrokeTransparency = 0.5
							if v.Name == "Chest1" then
								name.TextColor3 = Color3.fromRGB(109, 109, 109)
								name.Text = ("Chest 1" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
							if v.Name == "Chest2" then
								name.TextColor3 = Color3.fromRGB(173, 158, 21)
								name.Text = ("Chest 2" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
							if v.Name == "Chest3" then
								name.TextColor3 = Color3.fromRGB(85, 255, 255)
								name.Text = ("Chest 3" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							end
						else
							v['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
						end
					end
				else
					if v:FindFirstChild('NameEsp' .. Number) then
						v:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateDevilChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if DevilFruitESP then
				if string.find(v.Name, "Fruit") then
					if not v.Handle:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v.Handle)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v.Handle
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(255, 255, 255)
						name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
					else
						v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
					end
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end)
	end
end
function UpdateFlowerChams()
	for i, v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if v.Name == "Flower2" or v.Name == "Flower1" then
				if FlowerESP then
					if not v:FindFirstChild('NameEsp' .. Number) then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp' .. Number
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = Enum.Font.GothamSemibold
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(255, 0, 0)
						if v.Name == "Flower1" then
							name.Text = ("Blue Flower" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							name.TextColor3 = Color3.fromRGB(0, 0, 255)
						end
						if v.Name == "Flower2" then
							name.Text = ("Red Flower" .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
							name.TextColor3 = Color3.fromRGB(255, 0, 0)
						end
					else
						v['NameEsp' .. Number].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' Distance')
					end
				else
					if v:FindFirstChild('NameEsp' .. Number) then
						v:FindFirstChild('NameEsp' .. Number):Destroy()
					end
				end
			end
		end)
	end
end
function UpdateRealFruitChams()
	for i, v in pairs(game.Workspace.AppleSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(255, 0, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
	for i, v in pairs(game.Workspace.PineappleSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(255, 174, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
	for i, v in pairs(game.Workspace.BananaSpawner:GetChildren()) do
		if v:IsA("Tool") then
			if RealFruitESP then
				if not v.Handle:FindFirstChild('NameEsp' .. Number) then
					local bill = Instance.new('BillboardGui', v.Handle)
					bill.Name = 'NameEsp' .. Number
					bill.ExtentsOffset = Vector3.new(0, 1, 0)
					bill.Size = UDim2.new(1, 200, 1, 30)
					bill.Adornee = v.Handle
					bill.AlwaysOnTop = true
					local name = Instance.new('TextLabel', bill)
					name.Font = Enum.Font.GothamSemibold
					name.FontSize = "Size14"
					name.TextWrapped = true
					name.Size = UDim2.new(1, 0, 1, 0)
					name.TextYAlignment = 'Top'
					name.BackgroundTransparency = 1
					name.TextStrokeTransparency = 0.5
					name.TextColor3 = Color3.fromRGB(251, 255, 0)
					name.Text = (v.Name .. ' \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				else
					v.Handle['NameEsp' .. Number].TextLabel.Text = (v.Name .. ' ' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude / 3) .. ' Distance')
				end
			else
				if v.Handle:FindFirstChild('NameEsp' .. Number) then
					v.Handle:FindFirstChild('NameEsp' .. Number):Destroy()
				end
			end
		end
	end
end

spawn(function()
	while wait() do
		pcall(function()
			if MobESP then
				for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v:FindFirstChild('HumanoidRootPart') then
						if not v:FindFirstChild("MobEap") then
							local BillboardGui = Instance.new("BillboardGui")
							local TextLabel = Instance.new("TextLabel")
							BillboardGui.Parent = v
							BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
							BillboardGui.Active = true
							BillboardGui.Name = "MobEap"
							BillboardGui.AlwaysOnTop = true
							BillboardGui.LightInfluence = 1.000
							BillboardGui.Size = UDim2.new(0, 200, 0, 50)
							BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)
							TextLabel.Parent = BillboardGui
							TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.BackgroundTransparency = 1.000
							TextLabel.Size = UDim2.new(0, 200, 0, 50)
							TextLabel.Font = Enum.Font.GothamBold
							TextLabel.TextColor3 = Color3.fromRGB(7, 236, 240)
							TextLabel.Text.Size = 35
						end
						local Dis = math.floor((game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude)
						v.MobEap.TextLabel.Text = v.Name .. " - " .. Dis .. " Distance"
					end
				end
			else
				for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
					if v:FindFirstChild("MobEap") then
						v.MobEap:Destroy()
					end
				end
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if SeaESP then
				for i, v in pairs(game:GetService("Workspace").SeaBeasts:GetChildren()) do
					if v:FindFirstChild('HumanoidRootPart') then
						if not v:FindFirstChild("Seaesps") then
							local BillboardGui = Instance.new("BillboardGui")
							local TextLabel = Instance.new("TextLabel")
							BillboardGui.Parent = v
							BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
							BillboardGui.Active = true
							BillboardGui.Name = "Seaesps"
							BillboardGui.AlwaysOnTop = true
							BillboardGui.LightInfluence = 1.000
							BillboardGui.Size = UDim2.new(0, 200, 0, 50)
							BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)
							TextLabel.Parent = BillboardGui
							TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.BackgroundTransparency = 1.000
							TextLabel.Size = UDim2.new(0, 200, 0, 50)
							TextLabel.Font = Enum.Font.GothamBold
							TextLabel.TextColor3 = Color3.fromRGB(7, 236, 240)
							TextLabel.Text.Size = 35
						end
						local Dis = math.floor((game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude)
						v.Seaesps.TextLabel.Text = v.Name .. " - " .. Dis .. " Distance"
					end
				end
			else
				for i, v in pairs (game:GetService("Workspace").SeaBeasts:GetChildren()) do
					if v:FindFirstChild("Seaesps") then
						v.Seaesps:Destroy()
					end
				end
			end
		end)
	end
end)

spawn(function()
	while wait() do
		pcall(function()
			if NpcESP then
				for i, v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
					if v:FindFirstChild('HumanoidRootPart') then
						if not v:FindFirstChild("NpcEspes") then
							local BillboardGui = Instance.new("BillboardGui")
							local TextLabel = Instance.new("TextLabel")
							BillboardGui.Parent = v
							BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
							BillboardGui.Active = true
							BillboardGui.Name = "NpcEspes"
							BillboardGui.AlwaysOnTop = true
							BillboardGui.LightInfluence = 1.000
							BillboardGui.Size = UDim2.new(0, 200, 0, 50)
							BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)
							TextLabel.Parent = BillboardGui
							TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
							TextLabel.BackgroundTransparency = 1.000
							TextLabel.Size = UDim2.new(0, 200, 0, 50)
							TextLabel.Font = Enum.Font.GothamBold
							TextLabel.TextColor3 = Color3.fromRGB(7, 236, 240)
							TextLabel.Text.Size = 35
						end
						local Dis = math.floor((game.Players.LocalPlayer.Character.HumanoidRootPart.Position - v.HumanoidRootPart.Position).Magnitude)
						v.NpcEspes.TextLabel.Text = v.Name .. " - " .. Dis .. " Distance"
					end
				end
			else
				for i, v in pairs (game:GetService("Workspace").NPCs:GetChildren()) do
					if v:FindFirstChild("NpcEspes") then
						v.NpcEspes:Destroy()
					end
				end
			end
		end)
	end
end)
function isnil(thing)
	return (thing == nil)
end
local function round(n)
	return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)

function UpdateIslandMirageESP()
	for i, v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
		pcall(function()
			if MirageIslandESP then
				if v.Name == "Mirage Island" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function isnil(thing)
	return (thing == nil)
end
local function round(n)
	return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)

function UpdateAfdESP()
	for i, v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
		pcall(function()
			if AfdESP then
				if v.Name == "Advanced Fruit Dealer" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function UpdateAuraESP()
	for i, v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
		pcall(function()
			if AuraESP then
				if v.Name == "Master of Enhancement" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function UpdateLSDESP()
	for i, v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
		pcall(function()
			if LADESP then
				if v.Name == "Legendary Sword Dealer" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end

function UpdateGeaESP()
	for i, v in pairs(game:GetService("Workspace").Map.MysticIsland:GetChildren()) do
		pcall(function()
			if GearESP then
				if v.Name == "MeshPart" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end
--ChipsList
SelectRaid = {}
RaidsModule = require(game.ReplicatedStorage.Raids)
for i, v in pairs(RaidsModule.raids) do
	table.insert(SelectRaid, v)
end
for i, v in pairs(RaidsModule.advancedRaids) do
	table.insert(SelectRaid, v)
end
--BuyChip
spawn(function()
	while wait() do
		if getgenv().Auto_Buy_Chips_Dungeon then
			pcall(function()
				local args = {
					[1] = "RaidsNpc",
					[2] = "Select",
					[3] = getgenv().SelectChip
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end)
		end
	end
end)
--StartRaid
spawn(function()
	while wait(.1) do
		pcall(function()
			if getgenv().Auto_StartRaid then
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
					if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
						if Second_Sea then
							fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
						elseif Third_Sea then
							fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
						end
					end
				end
			end
		end)
	end
end)
--KillAura
spawn(function()
	while wait() do
		if getgenv().KillAura then
			pcall(function()
				for i, v in pairs(game.Workspace.Enemies:GetDescendants()) do
					if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
						repeat
							wait()
							sethiddenproperty(game:GetService('Players').LocalPlayer, "SimulationRadius", math.huge)
							v.Humanoid.Health = 0
							v.HumanoidRootPart.CanCollide = false
						until not getgenv().KillAura or not v.Parent or v.Humanoid.Health <= 0
					end
				end
			end)
		end
	end
end)
--NextIsland
spawn(function()
	while wait() do
		if getgenv().AutoNextIsland then
			pcall(function()
				if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
					if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
						topos(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame * CFrame.new(0, 70, 100))
					elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
						topos(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame * CFrame.new(0, 70, 100))
					elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
						topos(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame * CFrame.new(0, 70, 100))
					elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
						topos(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame * CFrame.new(0, 70, 100))
					elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
						topos(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame * CFrame.new(0, 70, 100))
					end
				end
			end)
		end
	end
end)
--AutoAwake
spawn(function()
	while wait() do
		if getgenv().AutoAwakenAbilities then
			pcall(function()
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener", "Awaken")
			end)
		end
	end
end)
--LawRaid
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().Auto_Law then
				if not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Microchip") and not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Microchip") and not game:GetService("Workspace").Enemies:FindFirstChild("Order") and not game:GetService("ReplicatedStorage"):FindFirstChild("Order") then
					wait(0.3)
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Microchip", "1")
					game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Microchip", "2")
				end
			end
		end
	end)
end)
spawn(function()
	pcall(function()
		while wait(0.4) do
			if getgenv().Auto_Law then
				if not game:GetService("Workspace").Enemies:FindFirstChild("Order") and not game:GetService("ReplicatedStorage"):FindFirstChild("Order") then
					if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Microchip") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Microchip") then
						fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon.Button.Main.ClickDetector)
					end
				end
				if game:GetService("ReplicatedStorage"):FindFirstChild("Order") or game:GetService("Workspace").Enemies:FindFirstChild("Order") then
					if game:GetService("Workspace").Enemies:FindFirstChild("Order") then
						for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
							if v.Name == "Order" then
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
									v.HumanoidRootPart.CanCollide = false
									v.HumanoidRootPart.Size = Vector3.new(120, 120, 120)
                                    --Click
								until not v.Parent or v.Humanoid.Health <= 0 or getgenv().Auto_Law == false
							end
						end
					elseif game:GetService("ReplicatedStorage"):FindFirstChild("Order") then
						topos(CFrame.new(-6217.2021484375, 28.047645568848, -5053.1357421875))
					end
				end
			end
		end
	end)
end)
--AutoTrials
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().AutoQuestRace then
				if game:GetService("Players").LocalPlayer.Data.Race.Value == "Human" then
					for i, v in pairs(game.Workspace.Enemies:GetDescendants()) do
						if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
							pcall(function()
								repeat
									wait(.1)
									v.Humanoid.Health = 0
									v.HumanoidRootPart.CanCollide = false
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								until not getgenv().AutoQuestRace or not v.Parent or v.Humanoid.Health <= 0
							end)
						end
					end
				elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Skypiea" then
					for i, v in pairs(game:GetService("Workspace").Map.SkyTrial.Model:GetDescendants()) do
						if v.Name ==  "snowisland_Cylinder.081" then
							BTPZ(v.CFrame * CFrame.new(0, 0, 0))
						end
					end
				elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Fishman" then
					for i, v in pairs(game:GetService("Workspace").SeaBeasts.SeaBeast1:GetDescendants()) do
						if v.Name ==  "HumanoidRootPart" then
							topos(v.CFrame * Random)
							for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
								if v:IsA("Tool") then
									if v.ToolTip == "Melee" then
										game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
									end
								end
							end
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
								if v:IsA("Tool") then
									if v.ToolTip == "Blox Fruit" then
										game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
									end
								end
							end
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
					
							wait(0.5)
							for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
								if v:IsA("Tool") then
									if v.ToolTip == "Sword" then
										game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
									end
								end
							end
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(0.5)
							for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
								if v:IsA("Tool") then
									if v.ToolTip == "Gun" then
										game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
									end
								end
							end
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 122, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 120, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							wait(.2)
							game:GetService("VirtualInputManager"):SendKeyEvent(true, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
							game:GetService("VirtualInputManager"):SendKeyEvent(false, 99, false, game.Players.LocalPlayer.Character.HumanoidRootPart)
						end
					end
				elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Cyborg" then
					topos(CFrame.new(28654, 14898.7832, -30, 1, 0, 0, 0, 1, 0, 0, 0, 1))
				elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Ghoul" then
					for i, v in pairs(game.Workspace.Enemies:GetDescendants()) do
						if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
							pcall(function()
								repeat
									wait(.1)
									v.Humanoid.Health = 0
									v.HumanoidRootPart.CanCollide = false
									sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
								until not getgenv().AutoQuestRace or not v.Parent or v.Humanoid.Health <= 0
							end)
						end
					end
				elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Mink" then
					for i, v in pairs(game:GetService("Workspace"):GetDescendants()) do
						if v.Name == "StartPoint" then
							topos(v.CFrame * CFrame.new(0, 10, 0))
						end
					end
				end
			end
		end
	end)
end)
--AutoTrains
local AcientCframe = CFrame.new(216.211181640625, 126.9352035522461, -12599.0732421875)
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().AutoFarmAcient then
				if game.Players.LocalPlayer.Character.RaceTransformed.Value == true then
					getgenv().AutoFarmAcient = false
					topos(CFrame.new(216.211181640625, 126.9352035522461, -12599.0732421875))
				end
			end
		end
	end)
end)
spawn(function()
	while wait() do
		if getgenv().AutoFarmAcient then
			pcall(function()
				if game:GetService("Workspace").Enemies:FindFirstChild("Cocoa Warrior") or game:GetService("Workspace").Enemies:FindFirstChild("Chocolate Bar Battler") or game:GetService("Workspace").Enemies:FindFirstChild("Sweet Thief") or game:GetService("Workspace").Enemies:FindFirstChild("Candy Rebel") then
					for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
						if v.Name == "Cocoa Warrior" or v.Name == "Chocolate Bar Battler" or v.Name == "Sweet Thief" or v.Name == "Candy Rebel" then
							if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
								bringmob = true
								repeat
									wait(getgenv().Fast_Delay)
									TryAttack()
									AutoHaki()
									EquipTool(SelectWeapon)
									v.HumanoidRootPart.CanCollide = false
									v.Humanoid.WalkSpeed = 0
									v.Head.CanCollide = false
									FarmPos = v.HumanoidRootPart.CFrame
									MonFarm = v.Name
									topos(v.HumanoidRootPart.CFrame * CFrame.new(posX, posY, posZ))
								until not getgenv().AutoFarmAcient or not v.Parent or v.Humanoid.Health <= 0
								bringmob = false
							end
						end
					end
				else
					toTarget(AcientCframe)
				end
			end)
		end
	end
end)
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().AutoFarmAcient then
				if game.Players.LocalPlayer.Character.RaceTransformed.Value == false then
					getgenv().AutoFarmAcient = true
				end
			end
		end
	end)
end)
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoFarmAcient then
				game:GetService("VirtualInputManager"):SendKeyEvent(true, "Y", false, game)
				wait(0.1)
				game:GetService("VirtualInputManager"):SendKeyEvent(false, "Y", false, game)
			end
		end)
	end
end)
--AutoBuyGears
spawn(function()
	pcall(function()
		while wait(.1) do
			if getgenv().AutoBuyGears then
				local args = {
					[1] = true
				}
				local args = {
					[1] = "UpgradeRace",
					[2] = "Buy"
				}
				game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("CommF_"):InvokeServer(unpack(args))
			end
		end
	end)  
end)
--EspKitsune
function UpdateIslandKisuneESP()
	for i, v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
		pcall(function()
			if KitsuneIslandEsp then
				if v.Name == "Kitsune Island" then
					if not v:FindFirstChild('NameEsp') then
						local bill = Instance.new('BillboardGui', v)
						bill.Name = 'NameEsp'
						bill.ExtentsOffset = Vector3.new(0, 1, 0)
						bill.Size = UDim2.new(1, 200, 1, 30)
						bill.Adornee = v
						bill.AlwaysOnTop = true
						local name = Instance.new('TextLabel', bill)
						name.Font = "Code"
						name.FontSize = "Size14"
						name.TextWrapped = true
						name.Size = UDim2.new(1, 0, 1, 0)
						name.TextYAlignment = 'Top'
						name.BackgroundTransparency = 1
						name.TextStrokeTransparency = 0.5
						name.TextColor3 = Color3.fromRGB(80, 245, 245)
					else
						v['NameEsp'].TextLabel.Text = (v.Name .. '   \n' .. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude / 3) .. ' M')
					end
				end
			else
				if v:FindFirstChild('NameEsp') then
					v:FindFirstChild('NameEsp'):Destroy()
				end
			end
		end)
	end
end
--TweentoKitsune
spawn(function()
	local kitsuneIsland
	while not kitsuneIsland do
		kitsuneIsland = game:GetService("Workspace").Map:FindFirstChild("KitsuneIsland")
		wait(1)
	end
	while wait() do
		if getgenv().TweenToKitsune then
			local shrineActive = kitsuneIsland:FindFirstChild("ShrineActive")
			if shrineActive then
				for _, v in pairs(shrineActive:GetDescendants()) do
					if v:IsA("BasePart") and v.Name:find("NeonShrinePart") then
						topos(v.CFrame)
					end
				end
			end
		end
	end
end)
--AutoAzureAmbers
spawn(function()
	while wait() do
		if getgenv().CollectAzure then
			pcall(function()
				if game:GetService("Workspace"):FindFirstChild("AttachedAzureEmber") then
					topos(game:GetService("Workspace"):WaitForChild("EmberTemplate"):FindFirstChild("Part").CFrame)
					print("Azure")
				end
			end)
		end
	end
end)
--TweenToMystic
function TweenMirage()
	repeat
		wait()
	until game:GetService("Workspace").Map:FindFirstChild("MysticIsland")
	if game:GetService("Workspace").Map:FindFirstChild("MysticIsland") then
		AllNPCS = getnilinstances()
		for r, v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
			table.insert(AllNPCS, v)
		end
		for r, v in pairs(AllNPCS) do
			if v.Name == "Advanced Fruit Dealer" then
				topos(v.HumanoidRootPart.CFrame)
			end
		end
	end
end
--TweentoGear
spawn(function()
	pcall(function()
		while wait() do
			if getgenv().TweenToGear then
				if game:GetService("Workspace").Map:FindFirstChild("MysticIsland") then
					for i, v in pairs(game:GetService("Workspace").Map.MysticIsland:GetChildren()) do 
						if v:IsA("MeshPart") then
							if v.Material ==  Enum.Material.Neon then
								topos(v.CFrame)
							end
						end
					end
				end
			end
		end
	end)
end)
--TweentoHighestPoint
function TwenetoHighestPoint()
	HighestPoint = getHighestPoint()
	if HighestPoint then
		topos(HighestPoint.CFrame * CFrame.new(0, 211.88, 0))
	end
end
function getHighestPoint()
	if not game.workspace.Map:FindFirstChild("MysticIsland") then
		return nil
	end
	for r, v in pairs(game:GetService("Workspace").Map.MysticIsland:GetDescendants()) do
		if v:IsA("MeshPart") then
			if v.MeshId == "rbxassetid://6745037796" then
				return v
			end
		end
	end
end
--LockMoonAndUseRaceSkill
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoLockMoon then
				local moonDir = game.Lighting:GetMoonDirection()
				local lookAtPos = game.Workspace.CurrentCamera.CFrame.p + moonDir * 100
				game.Workspace.CurrentCamera.CFrame = CFrame.lookAt(game.Workspace.CurrentCamera.CFrame.p, lookAtPos)
			end
		end)
	end
end)
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoLockMoon then
				wait(1.5)
				game:GetService("VirtualInputManager"):SendKeyEvent(true, "T", false, game)
				wait(.1)
				game:GetService("VirtualInputManager"):SendKeyEvent(false, "T", false, game)
			end
		end)
	end
end)
--RemoveFog
function NoFog()
	local c = game.Lighting
	c.FogEnd = 100000
	for r, v in pairs(c:GetDescendants()) do
		if v:IsA("Atmosphere") then
			v:Destroy()
		end
	end
end
--IncreaseSpeedBoats
game:GetService("RunService").RenderStepped:Connect(function()
	if getgenv().SpeedBoat then
		for i, v in pairs(game:GetService("Workspace").Boats:GetChildren()) do
			if game:GetService("Players").LocalPlayer.Character.Humanoid.Sit then
				v:FindFirstChild("VehicleSeat").MaxSpeed = 300
			end
		end
	end
end)
--CanCollideBoats(no clip boats)
spawn(function()
	while wait() do
		if getgenv().Nocliprock then
			if game.Players.LocalPlayer.Character.Humanoid.Sit == true then
				for _, v in pairs(game.Workspace.Boats:GetDescendants()) do
					if v:IsA("BasePart") and v.CanCollide == true then
						v.CanCollide = false
					end
				end
				for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
					if v:IsA("BasePart") and v.CanCollide == true then
						v.CanCollide = false
					end
				end
			elseif game.Players.LocalPlayer.Character.Humanoid.Sit == false then
				for _, v in pairs(game.Workspace.Boats:GetDescendants()) do
					if v:IsA("BasePart") and v.CanCollide == false then
						v.CanCollide = true
					end
				end
				for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
					if v:IsA("BasePart") and v.CanCollide == false then
						v.CanCollide = true
					end
				end
			end
		end
	end
end)
--PressW
spawn(function()
	while wait() do
		pcall(function()
			if getgenv().AutoW then
				game:GetService("VirtualInputManager"):SendKeyEvent(true, "W", false, game)
			end
		end)
	end
end)
--MeleeList
WeaponsList = {
	"Dark Step",
	"Electro",
	"Fishman Karate",
	"Dragon Claw",
	"SuperHuman",
	"Death Step",
	"Electric Claw",
	"SharkMan Karate",
	"Dragon Talon",
	"God Human",
	"Sanguine Art"
}
--SkillsList
SkillsList = {
	"Geppo",
	"Soru",
	"Ken Haki",
	"Buso Haki"
}
--ShopsList
ShopsList = {
	"Katana [1,000]",
	"Cutlass [1,000]",
	"Duel Katana [12,000]",
	"Iron Mace [25,000]",
	"Pipe [100,000]",
	"Triple Katana [60,000]",
	"Dual-Headed Blade [400,000]",
	"Bisento [1,000,000]",
	"Soul Cane [750,000]",
	"Slingshot [5,000]",
	"Musket [8,000]",
	"Flintlock [10,500]",
	"Refined Flintlock [65,000]",
	"Cannon [100,000]",
	"Kabucha [1500F]",
	"Black Cape [50,000]",
	"Toemo Ring [500,000]",
	"Swordsman Hat [150,000]"
}
--OhersLits
OthersList = {
	"Refund Stats",
	"Reroll Race",
	"Race Ghoul",
	"Race Cyborg"
}
--MusicsList
ListMusics = {
	'Quốc Ca Việt Nam',
	'I Love (slow+reverb version)',
	'Sad',
	'MisChief',
	'Squid Game',
	'SOS',
	'2 Guns',
	'Stay',
	'Fatal Breath',
	'Reason to Stay',
	'Only You',
	'Diss na Hagi Lagi (Nightcore)',
	'Dream Girl (sped up)',
	'Ocean Eyes',
	'Broken Glass',
	'Same Mistake',
	'Alone',
	'Thinking About You',
	'Hold On',
	'New World',
	'Rest For Life',
	'Vip Me',
	'Color',
	'Night Out (feat. Esther Dee)',
	'Crab Rave',
	'Unbreakable',
	'Can You ?',
	'White Tee',
	'WRLD Hang Up',
	'Free Fire',
	'Chipi Chipi Speed',
	'Blod Blod',
	'Play It Cool',
	'No Sleep',
	'Shine',
	'Gojo',
	'Gambare Senpai',
	'Din1c-DOWN2KILL',
	'Waka Waka',
	'Rickroll',
	'Preytty Girl',
	'Không Nên Tò Mò',
	'Phonk #1',
	'Phonk #2',
	'Phonk #3',
	'Phonk #4',
	'Phonk #5'
}
----------------------------------------------------------------------------------------------------------------------------------------
--Settings
Setting:Seperator("Settings")
Setting:Dropdown("Select Fast Attacks", {
	"Normal Fast",
	"Fast Attack",
	"Super Fast Attack"
}, "Smooth", function(Value)
	getgenv().SelectFastAttack = Value
end)
Setting:Dropdown("Select Weapons", {
	"Fruit",
	"Sword",
	"Melee"
}, "Melee", function(Value)
	getgenv().ChooseWeapon = Value
end)
Setting:Toggle("Enabled Fast Attack", true, function(Value)
	getgenv().FastAttackSida = Value
end)

Setting:Toggle("Enabled DamageAura (maybe get ban)", false, function(Value)
	getgenv().DamageAura = Value
end)

Setting:Toggle("Enabled Bring Mobs", true, function(Value)
	getgenv().BringMob = Value
end)
Setting:Toggle("Enabled Bypass TP", false, function(Value)
	getgenv().BypassTp = Value
end)
Setting:Toggle("Enabled Auto Buso Haki", false, function(Value)
	getgenv().AutoHakiBuso = Value
end)
Setting:Toggle("Enabled Remove Damage Texts", true, function(Value)
	getgenv().RemoveDameText = Value
end)
Setting:Toggle("Enabled Remove Notify", false, function(Value)
	getgenv().RemoveNotify = Value
end)
Setting:Toggle("Enabled White Screen", false, function(Value)
	if Value then
		game.RunService:Set3dRenderingEnabled(false)
		game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(500, 0, 500, 500)
	else
		game.RunService:Set3dRenderingEnabled(true)
		game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(1, 0, 500, 500)
	end
end)
Setting:Toggle("Enabled Anti AFK", true, function()
	local vu = game:GetService("VirtualUser")
	repeat
		wait()
	until game:IsLoaded()
	game:GetService("Players").LocalPlayer.Idled:connect(function()
		game:GetService("VirtualUser"):ClickButton2(Vector2.new())
		vu:Button2Down(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
		wait(1)
		vu:Button2Up(Vector2.new(0, 0), workspace.CurrentCamera.CFrame)
	end)
end)
Setting:Toggle("Enabled Auto Rejoin", true, function(Value)
	getgenv().AutoRejoin = Value
end)
Setting:Seperator("Setting Skills")
Setting:Toggle("Enabled Skill Z", true, function(Value)
	getgenv().Z = Value
end)
Setting:Toggle("Enabled Skill X", true, function(Value)
	getgenv().X = Value
end)
Setting:Toggle("Enabled Skill C", false, function(Value)
	getgenv().C = Value
end)
Setting:Toggle("Enabled Skill V", false, function(Value)
	getgenv().V = Value
end)
Setting:Toggle("Enabled Skill F", false, function(Value)
	getgenv().F = Value
end)
----------------------------------------------------------------------------------------------------------------------------------------
--Farming
Main:Seperator("Miscs Farm")
Main:Button("Redeem All Codes", function()
	RedeemCode()
end)
Main:Button("Boost FPS", function()
	FPSBooster()
end)

Main:Seperator("Main Farm")
Main:Toggle("Farm Level", false, function(Value)
	getgenv().AutoLevel = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Toggle("Farm Mobs Aura", false, function(Value)
	getgenv().AutoNear = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)

Main:Seperator("Bones Farm")
Main:Toggle("Farm Bones", false, function(Value)
	getgenv().AutoBone = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Toggle("Get Quest", true, function(Value)
	getgenv().ClaimQuestBone = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Toggle("Random Bones", false, function(Value)
	getgenv().AutoRandomBone = Value
end)
Main:Seperator("Katakuri Farm")
Main:Toggle("Farm Cake Prince", false, function(Value)
	getgenv().CakePrince = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Toggle("Spawn Boss", true, function(Value)
	getgenv().SpawnCakePrince = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Seperator("Ectoplasms Farm")
Main:Toggle("Farm Ectoplasms", false, function(Value)
	getgenv().Ectoplasm = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Seperator("Mastery Farm")
getgenv().TypeMastery = "Level"
Main:Dropdown("Select Mode Farm", {
	"Level",
	"Mob Aura"
}, "Level", function(Value)
	getgenv().TypeMastery = Value
end)
getgenv().HealthMob = 25
Main:Dropdown("Select Health Mobs", {
	'20',
	'25',
	'30',
	'35',
	'40',
	'45',
	'50'
}, "25", function(Value)
	getgenv().HealthMob = Value
end)
Main:Toggle("Farm Fruit Mastery", false, function(Value)
	getgenv().AutoMasFruit = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Seperator("Materials Farm")
Main:Dropdown("Select Materials", MaterialList, "", function(Value)
	getgenv().SelectMaterial = Value
end)
Main:Toggle("Farm Selected Material", false, function(Value)
	getgenv().AutoMaterial = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Seperator("Bosses Farm")
local StatusBoss = Main:Label("Status Boss: N/A")
spawn(function()
	while wait() do
		pcall(function()
			if game:GetService("ReplicatedStorage"):FindFirstChild(getgenv().SelectBoss) or game:GetService("Workspace").Enemies:FindFirstChild(getgenv().SelectBoss) then
				StatusBoss:Set("Status Boss: 🟢")
			else
				StatusBoss:Set("Status Boss: 🔴")
			end
		end)
	end
end)
Main:Dropdown("Select Boss", tableBoss, "", function(Value)
	getgenv().SelectBoss = Value
end)
Main:Toggle("Farm Selected Boss", false, function(Value)
	getgenv().AutoBoss = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Main:Seperator("Elite Farm")
Main:Toggle("Farm Elite Hunter", false, function(Value)
	getgenv().AutoElite = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
----------------------------------------------------------------------------------------------------------------------------------------
--Others Farm
Farm:Seperator("Stats")
Farm:Dropdown("Select Add Stats", {
	'Demon Fruit',
	'Gun',
	'Sword',
	'Defense',
	'Melee'
}, "", function(Value)
	getgenv().SelectAddStats = Value
end)
Farm:Toggle("Auto Add Stats", false, function(Value)
	getgenv().AutoAddStats = Value
end)
Farm:Seperator("First Sea Items")
Farm:Toggle("Auto Saber", false, function(Value)
	getgenv().GetSaber = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Auto Pole V1", false, function(Value)
	getgenv().GetPoleV1 = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Seperator("Second Sea Items")
Farm:Toggle("Auto Bartilo Quest", false, function(Value)
	getgenv().AutoBartiloQuest = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Auto Evo Race", false, function(Value)
	getgenv().AutoEvoRace = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Farm Factory", false, function(Value)
	getgenv().Factory = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Auto Rengoku", false, function(Value)
	getgenv().AutoRengoku = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Seperator("Third Sea Items")
Farm:Toggle("Auto Hallow Scythe", false, function(Value)
	getgenv().AutoHallowSycthe = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Claim Yama", false, function(Value)
	getgenv().AutoYama = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Holy Torch ", false, function(Value)
	getgenv().Auto_Holy_Torch = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Kill Longma Boss", false, function(Value)
	getgenv().GetTushita = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Farm Dought King (killing boss)", false, function(Value)
	getgenv().AutoCakeV2 = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Farm Castle Raids", false, function(Value)
	getgenv().CastleRaid = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Seperator("Others Items")
Farm:Toggle("Buy Swords Lengendary", false, function(Value)
	getgenv().BuyLengendSword = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm:Toggle("Buy Haki Colors", false, function(Value)
	getgenv().Auto_Buy_Enchancement = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm2:Seperator("Fighting Styles")
Farm2:Toggle("Auto Death Step", false, function(Value)
	getgenv().AutoDeathStep = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm2:Toggle("Auto Sharkman Karate", false, function(Value)
	getgenv().AutoSharkmanKarate = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm2:Toggle("Auto Electric Claw", false, function(Value)
	getgenv().AutoElectricClaw = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm2:Toggle("Auto Dragon Talon", false, function(Value)
	getgenv().AutoDragonTalon = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Farm2:Toggle("Auto God Human", false, function(Value)
	getgenv().AutoGodHuman = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
-------------------------------------------------------------------------------------------------------------------------------------------
--Players - Teleports
Player:Seperator("Players")
local Playerslist = {}
for i, v in pairs(game:GetService("Players"):GetChildren()) do
	table.insert(Playerslist, v.Name)
end
local PlayersDropdown = Player:Dropdown("Select Players", Playerslist, "", function(Value)
	getgenv().SelectPly = Value
end)
Player:Button("Refresh Players Dropdown", function()
	Playerslist = {}
	PlayersDropdown:Clear()
	for i, v in pairs(game:GetService("Players"):GetChildren()) do
		PlayersDropdown:Add(v.Name)
	end
end)
Player:Toggle("Teleport to Selected Player", false, function(Value)
	getgenv().TeleportPly = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("Spectate Selected Player", false, function(Value)
	getgenv().SpectatePlys = Value
	local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
	local plr2 = game:GetService("Players"):FindFirstChild(getgenv().SelectPly)
	repeat
		wait(.1)
		game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(getgenv().SelectPly).Character.Humanoid
	until getgenv().SpectatePlys == false
	game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Seperator("Others")
Player:Toggle("Turn Race V3", false, function(Value)
	getgenv().TurnRaceV3 = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("Turn Race V4", false, function(Value)
	getgenv().TurnRaceV4 = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("No Clip", false, function(Value)
	getgenv().LOf = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("Super Speed", true, function(Value)
	getgenv().RunSpeed = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("Walk on Water", true, function(Value)
	getgenv().WalkonWater = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Player:Toggle("Auto Turn PVP", false, function(Value)
	getgenv().EnabledPvP = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Teleport:Seperator("Teleports")
Teleport:Dropdown("Select Islands", IslandList, "", function(Value)
	getgenv().SelectIsland = Value
end)
Teleport:Button("Tween", function()
	if getgenv().SelectIsland == "WindMill" then
		topos(CFrame.new(979.79895019531, 16.516613006592, 1429.0466308594))
	elseif getgenv().SelectIsland == "Marine" then
		topos(CFrame.new(-2566.4296875, 6.8556680679321, 2045.2561035156))
	elseif getgenv().SelectIsland == "Middle Town" then
		topos(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
	elseif getgenv().SelectIsland == "Jungle" then
		topos(CFrame.new(-1612.7957763672, 36.852081298828, 149.12843322754))
	elseif getgenv().SelectIsland == "Pirate Village" then
		topos(CFrame.new(-1181.3093261719, 4.7514905929565, 3803.5456542969))
	elseif getgenv().SelectIsland == "Desert" then
		topos(CFrame.new(944.15789794922, 20.919729232788, 4373.3002929688))
	elseif getgenv().SelectIsland == "Snow Island" then
		topos(CFrame.new(1347.8067626953, 104.66806030273, -1319.7370605469))
	elseif getgenv().SelectIsland == "MarineFord" then
		topos(CFrame.new(-4914.8212890625, 50.963626861572, 4281.0278320313))
	elseif getgenv().SelectIsland == "Colosseum" then
		topos( CFrame.new(-1427.6203613281, 7.2881078720093, -2792.7722167969))
	elseif getgenv().SelectIsland == "Sky Island 1" then
		topos(CFrame.new(-4869.1025390625, 733.46051025391, -2667.0180664063))
	elseif getgenv().SelectIsland == "Sky Island 2" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.82275, 872.54248, -1667.55688))
	elseif getgenv().SelectIsland == "Sky Island 3" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
	elseif getgenv().SelectIsland == "Prison" then
		topos( CFrame.new(4875.330078125, 5.6519818305969, 734.85021972656))
	elseif getgenv().SelectIsland == "Magma Village" then
		topos(CFrame.new(-5247.7163085938, 12.883934020996, 8504.96875))
	elseif getgenv().SelectIsland == "Under Water Island" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
	elseif getgenv().SelectIsland == "Fountain City" then
		topos(CFrame.new(5127.1284179688, 59.501365661621, 4105.4458007813))
	elseif getgenv().SelectIsland == "Shank Room" then
		topos(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
	elseif getgenv().SelectIsland == "Mob Island" then
		topos(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
	elseif getgenv().SelectIsland == "The Cafe" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-281.93707275390625, 306.130615234375, 609.280029296875))
		topos(CFrame.new(-380.47927856445, 77.220390319824, 255.82550048828))
	elseif getgenv().SelectIsland == "Frist Spot" then
		topos(CFrame.new(-11.311455726624, 29.276733398438, 2771.5224609375))
	elseif getgenv().SelectIsland == "Dark Area" then
		topos(CFrame.new(3780.0302734375, 22.652164459229, -3498.5859375))
	elseif getgenv().SelectIsland == "Flamingo Mansion" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-281.93707275390625, 306.130615234375, 609.280029296875))
	elseif getgenv().SelectIsland == "Flamingo Room" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(2284.912109375, 15.152034759521484, 905.48291015625))
	elseif getgenv().SelectIsland == "Green Zone" then
		topos( CFrame.new(-2448.5300292969, 73.016105651855, -3210.6306152344))
	elseif getgenv().SelectIsland == "Factory" then
		topos(CFrame.new(424.12698364258, 211.16171264648, -427.54049682617))
	elseif getgenv().SelectIsland == "Colossuim" then
		topos( CFrame.new(-1503.6224365234, 219.7956237793, 1369.3101806641))
	elseif getgenv().SelectIsland == "Zombie Island" then
		topos(CFrame.new(-5622.033203125, 492.19604492188, -781.78552246094))
	elseif getgenv().SelectIsland == "Two Snow Mountain" then
		topos(CFrame.new(753.14288330078, 408.23559570313, -5274.6147460938))
	elseif getgenv().SelectIsland == "Punk Hazard" then
		topos(CFrame.new(-6127.654296875, 15.951762199402, -5040.2861328125))
	elseif getgenv().SelectIsland == "Cursed Ship" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.40197753906, 125.05712890625, 32885.875))
	elseif getgenv().SelectIsland == "Ice Castle" then
		topos(CFrame.new(6148.4116210938, 294.38687133789, -6741.1166992188))
	elseif getgenv().SelectIsland == "Forgotten Island" then
		topos(CFrame.new(-3032.7641601563, 317.89672851563, -10075.373046875))
	elseif getgenv().SelectIsland == "Ussop Island" then
		topos(CFrame.new(4816.8618164063, 8.4599885940552, 2863.8195800781))
	elseif getgenv().SelectIsland == "Mini Sky Island" then
		topos(CFrame.new(-288.74060058594, 49326.31640625, -35248.59375))
	elseif getgenv().SelectIsland == "Great Tree" then
		topos(CFrame.new(2681.2736816406, 1682.8092041016, -7190.9853515625))
	elseif getgenv().SelectIsland == "Castle On The Sea" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-5075.50927734375, 314.5155029296875, -3150.0224609375))
	elseif getgenv().SelectIsland == "MiniSky" then
		topos(CFrame.new(-260.65557861328, 49325.8046875, -35253.5703125))
	elseif getgenv().SelectIsland == "Port Town" then
		topos(CFrame.new(-290.7376708984375, 6.729952812194824, 5343.5537109375))
	elseif getgenv().SelectIsland == "Hydra Island" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(5753.5478515625, 610.7880859375, -282.33172607421875))
	elseif getgenv().SelectIsland == "Floating Turtle" then
		topos(CFrame.new(-13274.528320313, 531.82073974609, -7579.22265625))
	elseif getgenv().SelectIsland == "Mansion" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-12468.5380859375, 375.0094299316406, -7554.62548828125))
	elseif getgenv().SelectIsland == "Haunted Castle" then
		topos(CFrame.new(-9515.3720703125, 164.00624084473, 5786.0610351562))
	elseif getgenv().SelectIsland == "Ice Cream Island" then
		topos(CFrame.new(-902.56817626953, 79.93204498291, -10988.84765625))
	elseif getgenv().SelectIsland == "Peanut Island" then
		topos(CFrame.new(-2062.7475585938, 50.473892211914, -10232.568359375))
	elseif getgenv().SelectIsland == "Cake Island" then
		topos(CFrame.new(-1884.7747802734375, 19.327526092529297, -11666.8974609375))
	elseif getgenv().SelectIsland == "Cocoa Island" then
		topos(CFrame.new(87.94276428222656, 73.55451202392578, -12319.46484375))
	elseif getgenv().SelectIsland == "Candy Island" then
		topos(CFrame.new(-1014.4241943359375, 149.11068725585938, -14555.962890625))
	elseif getgenv().SelectIsland == "Tiki Outpost" then
		topos(CFrame.new(-16217.7568359375, 15.757582664489746, 480.287109375))
	end
end)
Teleport:Button("BypassTP", function()
	if getgenv().SelectIsland == "WindMill" then
		BTP1(CFrame.new(979.79895019531, 16.516613006592, 1429.0466308594))
	elseif getgenv().SelectIsland == "Marine" then
		BTP1(CFrame.new(-2566.4296875, 6.8556680679321, 2045.2561035156))
	elseif getgenv().SelectIsland == "Middle Town" then
		BTP1(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
	elseif getgenv().SelectIsland == "Jungle" then
		BTP1(CFrame.new(-1612.7957763672, 36.852081298828, 149.12843322754))
	elseif getgenv().SelectIsland == "Pirate Village" then
		BTP1(CFrame.new(-1181.3093261719, 4.7514905929565, 3803.5456542969))
	elseif getgenv().SelectIsland == "Desert" then
		BTP1(CFrame.new(944.15789794922, 20.919729232788, 4373.3002929688))
	elseif getgenv().SelectIsland == "Snow Island" then
		BTP1(CFrame.new(1347.8067626953, 104.66806030273, -1319.7370605469))
	elseif getgenv().SelectIsland == "MarineFord" then
		BTP1(CFrame.new(-4914.8212890625, 50.963626861572, 4281.0278320313))
	elseif getgenv().SelectIsland == "Colosseum" then
		BTP1( CFrame.new(-1427.6203613281, 7.2881078720093, -2792.7722167969))
	elseif getgenv().SelectIsland == "Sky Island 1" then
		BTP1(CFrame.new(-4869.1025390625, 733.46051025391, -2667.0180664063))
	elseif getgenv().SelectIsland == "Sky Island 2" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-4607.82275, 872.54248, -1667.55688))
	elseif getgenv().SelectIsland == "Sky Island 3" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
	elseif getgenv().SelectIsland == "Prison" then
		BTP1( CFrame.new(4875.330078125, 5.6519818305969, 734.85021972656))
	elseif getgenv().SelectIsland == "Magma Village" then
		BTP1(CFrame.new(-5247.7163085938, 12.883934020996, 8504.96875))
	elseif getgenv().SelectIsland == "Under Water Island" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
	elseif getgenv().SelectIsland == "Fountain City" then
		BTP1(CFrame.new(5127.1284179688, 59.501365661621, 4105.4458007813))
	elseif getgenv().SelectIsland == "Shank Room" then
		BTP1(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
	elseif getgenv().SelectIsland == "Mob Island" then
		BTP1(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
	elseif getgenv().SelectIsland == "The Cafe" then
		BTP1(CFrame.new(-380.47927856445, 77.220390319824, 255.82550048828))
	elseif getgenv().SelectIsland == "Frist Spot" then
		BTP1(CFrame.new(-11.311455726624, 29.276733398438, 2771.5224609375))
	elseif getgenv().SelectIsland == "Dark Area" then
		BTP1(CFrame.new(3780.0302734375, 22.652164459229, -3498.5859375))
	elseif getgenv().SelectIsland == "Flamingo Mansion" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-281.93707275390625, 306.130615234375, 609.280029296875))
	elseif getgenv().SelectIsland == "Flamingo Room" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(2284.912109375, 15.152034759521484, 905.48291015625))
	elseif getgenv().SelectIsland == "Green Zone" then
		BTP1( CFrame.new(-2448.5300292969, 73.016105651855, -3210.6306152344))
	elseif getgenv().SelectIsland == "Factory" then
		BTP1(CFrame.new(424.12698364258, 211.16171264648, -427.54049682617))
	elseif getgenv().SelectIsland == "Colossuim" then
		BTP1( CFrame.new(-1503.6224365234, 219.7956237793, 1369.3101806641))
	elseif getgenv().SelectIsland == "Zombie Island" then
		BTP1(CFrame.new(-5622.033203125, 492.19604492188, -781.78552246094))
	elseif getgenv().SelectIsland == "Two Snow Mountain" then
		BTP1(CFrame.new(753.14288330078, 408.23559570313, -5274.6147460938))
	elseif getgenv().SelectIsland == "Punk Hazard" then
		BTP1(CFrame.new(-6127.654296875, 15.951762199402, -5040.2861328125))
	elseif getgenv().SelectIsland == "Cursed Ship" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(923.40197753906, 125.05712890625, 32885.875))
	elseif getgenv().SelectIsland == "Ice Castle" then
		BTP1(CFrame.new(6148.4116210938, 294.38687133789, -6741.1166992188))
	elseif getgenv().SelectIsland == "Forgotten Island" then
		BTP1(CFrame.new(-3032.7641601563, 317.89672851563, -10075.373046875))
	elseif getgenv().SelectIsland == "Ussop Island" then
		BTP1(CFrame.new(4816.8618164063, 8.4599885940552, 2863.8195800781))
	elseif getgenv().SelectIsland == "Mini Sky Island" then
		BTP1(CFrame.new(-288.74060058594, 49326.31640625, -35248.59375))
	elseif getgenv().SelectIsland == "Great Tree" then
		BTP1(CFrame.new(2681.2736816406, 1682.8092041016, -7190.9853515625))
	elseif getgenv().SelectIsland == "Castle On The Sea" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-5075.50927734375, 314.5155029296875, -3150.0224609375))
	elseif getgenv().SelectIsland == "MiniSky" then
		BTP1(CFrame.new(-260.65557861328, 49325.8046875, -35253.5703125))
	elseif getgenv().SelectIsland == "Port Town" then
		BTP1(CFrame.new(-290.7376708984375, 6.729952812194824, 5343.5537109375))
	elseif getgenv().SelectIsland == "Hydra Island" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(5753.5478515625, 610.7880859375, -282.33172607421875))
	elseif getgenv().SelectIsland == "Floating Turtle" then
		BTP1(CFrame.new(-13274.528320313, 531.82073974609, -7579.22265625))
	elseif getgenv().SelectIsland == "Mansion" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-12468.5380859375, 375.0094299316406, -7554.62548828125))
	elseif getgenv().SelectIsland == "Haunted Castle" then
		BTP1(CFrame.new(-9515.3720703125, 164.00624084473, 5786.0610351562))
	elseif getgenv().SelectIsland == "Ice Cream Island" then
		BTP1(CFrame.new(-902.56817626953, 79.93204498291, -10988.84765625))
	elseif getgenv().SelectIsland == "Peanut Island" then
		BTP1(CFrame.new(-2062.7475585938, 50.473892211914, -10232.568359375))
	elseif getgenv().SelectIsland == "Cake Island" then
		BTP1(CFrame.new(-1884.7747802734375, 19.327526092529297, -11666.8974609375))
	elseif getgenv().SelectIsland == "Cocoa Island" then
		BTP1(CFrame.new(87.94276428222656, 73.55451202392578, -12319.46484375))
	elseif getgenv().SelectIsland == "Candy Island" then
		BTP1(CFrame.new(-1014.4241943359375, 149.11068725585938, -14555.962890625))
	elseif getgenv().SelectIsland == "Tiki Outpost" then
		BTP1(CFrame.new(-16217.7568359375, 15.757582664489746, 480.287109375))
	end
end)
Teleport:Button("Stop Tween", function()
	topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
end)
Teleport:Seperator("Worlds")
Teleport:Button("Teleport to Old World", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelMain")
end)
Teleport:Button("Teleport to Second World", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
end)
Teleport:Button("Teleport to Third World", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
end)
-------------------------------------------------------------------------------------------------------------------------------------------
--Fruits - Raids
Fruit:Seperator("Fruits")
getgenv().SelectFruit = "Kitsune-Kitsune"
Fruit:Dropdown("Select Fruits", Table_DevilFruitSniper, "Kitsune-Kitsune", function(Value)
	getgenv().SelectFruit = Value
end)
Fruit:Toggle("Buy Selected Fruits", false, function(Value)
	getgenv().AutoBuyFruitSniper = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Fruit:Toggle("Auto Random Fruits", false, function(Value)
	getgenv().RandomFruits = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Fruit:Toggle("Auto Store Fruits", false, function(Value)
	getgenv().StoreFruit = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Fruit:Toggle("Auto Collect Fruits (risk)", false, function(Value)
	getgenv().CollectFruitTP = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Fruit:Seperator("Esp")
Fruit:Toggle("Esp Players", false, function(Value)
	ESPPlayer = Value
	UpdatePlayerChams()
end)
Fruit:Toggle("Esp Fruits", false, function(Value)
	DevilFruitESP = Value
	while DevilFruitESP do
		wait()
		UpdateDevilChams()
	end
end)
Fruit:Toggle("Esp Islands", false, function(Value)
	IslandESP = Value
	while IslandESP do
		wait()
		UpdateIslandESP()
	end
end)
Fruit:Toggle("Esp Flowers", false, function(Value)
	FlowerESP = Value
	UpdateFlowerChams()
end)
spawn(function()
	while wait(2) do
		if FlowerESP then
			UpdateFlowerChams()
		end
		if DevilFruitESP then
			UpdateDevilChams()
		end
		if ChestESP then
			UpdateChestChams()
		end
		if ESPPlayer then
			UpdatePlayerChams()
		end
		if RealFruitESP then
			UpdateRealFruitChams()
		end
	end
end)
Raid:Seperator("Raids")
getgenv().SelectChip = "Dough"
Raid:Dropdown("Select Chips", SelectRaid, "", function(Value)
	getgenv().SelectChip = Value
end)
Raid:Toggle("Auto Buy Selected Chip", false, function(Value)
	getgenv().Auto_Buy_Chips_Dungeon = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Raid:Toggle("Auto Start Raid", false, function(Value)
	getgenv().Auto_StartRaid = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Raid:Toggle("Auto Kill Aura", false, function(Value)
	getgenv().KillAura = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Raid:Toggle("Auto Next Island", false, function(Value)
	getgenv().AutoNextIsland = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Raid:Toggle("Auto Awake", false, function(Value)
	getgenv().AutoAwakenAbilities = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Raid:Seperator("Others")
if Second_Sea then
	Raid:Button("Tween to Raid Lab (Second Sea)", function()
		topos(CFrame.new(-6438.73535, 250.645355, -4501.50684))
	end)
elseif Third_Sea then
	Raid:Button("Tween to Raid Lab (Third Sea)", function()
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(-5075.50927734375, 314.5155029296875, -3150.0224609375))
		topos(CFrame.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818))
	end)
end
Raid:Seperator("Law Raid")
Raid:Toggle("Auto Law Raid (fully)", false, function(Value)
	getgenv().Auto_Law = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
----------------------------------------------------------------------------------------------------------------------------------------
--Race1
Race:Seperator("Tween")
Race:Button("Tween to Timple of Time", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(28286.35546875, 14895.3017578125, 102.62469482421875))
end)
Race:Button("Tween to Lever", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(28286.35546875, 14895.3017578125, 102.62469482421875))
	topos(CFrame.new(28575.181640625, 14936.6279296875, 72.31636810302734))
end)
Race:Button("Tween to Ancient One", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(28286.35546875, 14895.3017578125, 102.62469482421875))
	topos(CFrame.new(28981.552734375, 14888.4267578125, -120.245849609375))
end)
Race:Seperator("Doors")
Race:Button("Tween to Your Race", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance", Vector3.new(28286.35546875, 14895.3017578125, 102.62469482421875))
	if game:GetService("Players").LocalPlayer.Data.Race.Value == "Human" then
		topos(CFrame.new(29221.822265625, 14890.9755859375, -205.99114990234375))
	elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Skypiea" then
		topos(CFrame.new(28960.158203125, 14919.6240234375, 235.03948974609375))
	elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Fishman" then
		topos(CFrame.new(28231.17578125, 14890.9755859375, -211.64173889160156))
	elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Cyborg" then
		topos(CFrame.new(28502.681640625, 14895.9755859375, -423.7279357910156))
	elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Ghoul" then
		topos(CFrame.new(28674.244140625, 14890.6767578125, 445.4310607910156))
	elseif game:GetService("Players").LocalPlayer.Data.Race.Value == "Mink" then
		topos(CFrame.new(29012.341796875, 14890.9755859375, -380.1492614746094))
	end
end)
Race2:Seperator("Auto Trials")
Race2:Toggle("Auto Human + Ghoul Trials", false, function(Value)
	getgenv().KillAura = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Race2:Toggle("Auto Trials", false, function(Value)
	getgenv().AutoQuestRace = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Race2:Seperator("Ancient One Quests")
Race2:Toggle("Auto Train Your Race", false, function(Value)
	getgenv().AutoFarmAcient = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Race2:Toggle("Auto Buy Gears", false, function(Value)
	getgenv().AutoBuyGears = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
-------------------------------------------------------------------------------------------------------------------------------------------
--Sea Events
Sea:Seperator("Rough Sea(soon)")
Sea:Seperator("Kitsune Island")
Sea:Toggle("Esp Kitsune Island", false, function(Value)
	KitsuneIslandEsp = Value
	while KitsuneIslandEsp do
		wait()
		UpdateIslandKisuneESP()
	end
end)
Sea:Toggle("Tween to Kitsune Island", false, function(Value)
	getgenv().TweenToKitsune = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea:Toggle("Auto Collect Azure Ambers", false, function(Value)
	getgenv().CollectAzure = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea:Seperator("Mystic Island")
Sea:Button("Tween to Mystic Island", function()
	TweenMirage()
end)
Sea:Button("Tween to Highest Point", function()
	TwenetoHighestPoint()
end)
Sea:Button("Tween to Advanced Fruit Dealer", function()
	FindAdvancedDealer()
end)
Sea:Toggle("Tween to Blue Gear", false, function(Value)
	getgenv().TweenToGear = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea:Toggle("Lock Moon and Use Race Skill", false, function(Value)
	getgenv().AutoLockMoon = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea2:Seperator("Others")
Sea2:Button("Remove Fog", function()
	NoFog()
end)
Sea2:Seperator("Boats")
BoatsName = {}
for i, v in pairs(game:GetService("Workspace").Boats:GetChildren()) do
	table.insert(BoatsName , v.Name)
end
local Boats = Sea2:Dropdown("Select Boats", BoatsName, "", function(Value)
	getgenv().SelectBoatsBring = Value
end)
Sea2:Button("Refresh Boats Dropdown", function()
	BoatsName = {}
	Boats:Clear()
	for i, v in pairs(game:GetService("Workspace").Boats:GetChildren()) do
		Boats:Add(v.Name)
	end
end)
Sea2:Button("Bring Selected Boat", function()
	game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Boats[getgenv().SelectBoatsBring].VehicleSeat.CFrame
end)
Sea2:Button("Tween to Selected Boat", function()
	if game:GetService("Workspace").Boats:FindFirstChild(getgenv().SelectBoatsBring) then
		topos(game:GetService("Workspace").Boats[getgenv().SelectBoatsBring].VehicleSeat.CFrame)
	end
end)
Sea2:Seperator("Others")
Sea2:Toggle("Increase Speed Boats", false, function(Value)
	getgenv().SpeedBoat = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea2:Toggle("CanCollide Boats (no clip)", false, function(Value)
	getgenv().Nocliprock = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
Sea2:Toggle("Press W", false, function(Value)
	getgenv().AutoW = Value
	if Value == false then
		wait()
		topos(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
		wait()
	end
end)
----------------------------------------------------------------------------------------------------------------------------------------
--Status Server
Sta:Seperator("Infomations Servers")
local Time = Sta:Label("")
function UpdateTime()
	local GameTime = math.floor(workspace.DistributedGameTime + 0.5)
	local Hour = math.floor(GameTime / (60 ^ 2)) % 24
	local Minute = math.floor(GameTime / (60 ^ 1)) % 60
	local Second = math.floor(GameTime / (60 ^ 0)) % 60
	Time:Set("< Game Time > : Hours : " .. Hour .. " Minutes : " .. Minute .. " Seconds : " .. Second)
end
spawn(function()
	while wait() do
		pcall(function()
			UpdateTime()
		end)
	end
end)
local StatusElite = Sta:Label("")
spawn(function()
	while wait() do
		pcall(function()
			if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo") or game:GetService("ReplicatedStorage"):FindFirstChild("Deandre") or game:GetService("ReplicatedStorage"):FindFirstChild("Urban") or game:GetService("Workspace").Enemies:FindFirstChild("Diablo") or game:GetService("Workspace").Enemies:FindFirstChild("Deandre") or game:GetService("Workspace").Enemies:FindFirstChild("Urban") then
				StatusElite:Set("Status Elite Hunter : 🟢 | Totals:  " .. game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter", "Progress"))
			else
				StatusElite:Set("Status Elite Hunter : 🔴 | Totals: " .. game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter", "Progress"))
			end
		end)
	end
end)
local Mob_Kill_Cake_Prince = Sta:Label("")
spawn(function()
	while wait() do
		pcall(function()
			if string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 88 then
				Mob_Kill_Cake_Prince:Set("Status Cake Mobs : " .. string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"), 39, 41) .. "/500")
			elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 87 then
				Mob_Kill_Cake_Prince:Set("Status Cake Mobs : " .. string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"), 39, 40) .. "/500")
			elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 86 then
				Mob_Kill_Cake_Prince:Set("Status Cake Mobs : " .. string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"), 39, 39) .. "/500")
			else
				Mob_Kill_Cake_Prince:Set("Status Cake Boss : 🟢")
			end
		end)
	end
end)
local StatusKitsune = Sta:Label("")
function UpdateKitsune()
	if game.Workspace._WorldOrigin.Locations:FindFirstChild('Kitsune Island') then
		StatusKitsune:Set("Status Kitsune Island : 🟢")
	else
		StatusKitsune:Set("Status Kitsune Island : 🔴")
	end
end
spawn(function()
	pcall(function()
		while wait() do
			UpdateKitsune()
		end
	end)
end)
local StatusMirage = Sta:Label("")
task.spawn(function()
	while wait() do
		pcall(function()
			if game:GetService("Lighting").Sky.MoonTextureId == "http://www.roblox.com/asset/?id=9709149431" then
				FullMoonStatus = "100%"
			elseif game:GetService("Lighting").Sky.MoonTextureId == "http://www.roblox.com/asset/?id=9709149052" then
				FullMoonStatus = "75%"
			elseif game:GetService("Lighting").Sky.MoonTextureId == "http://www.roblox.com/asset/?id=9709143733" then
				FullMoonStatus = "50%"
			elseif game:GetService("Lighting").Sky.MoonTextureId == "http://www.roblox.com/asset/?id=9709150401" then
				FullMoonStatus = "25%"
			elseif game:GetService("Lighting").Sky.MoonTextureId == "http://www.roblox.com/asset/?id=9709149680" then
				FullMoonStatus = "15%"
			else
				FullMoonStatus = "0%"
			end
		end)
	end
end)
task.spawn(function()
	while wait() do
		pcall(function()
			if game.Workspace._WorldOrigin.Locations:FindFirstChild('Mirage Island') then
				MirageStatus = "🟢"
			else
				MirageStatus = '🔴'
			end
		end)
	end
end)
spawn(function()
	pcall(function()
		while wait() do
			StatusMirage:Set("Status Mirage Island: " .. MirageStatus .. " | Status Full Moon: " .. FullMoonStatus)
		end
	end)
end)
Sta2:Seperator("Info")
Sta2:Label("Script by: piamla")
Sta2:Label("Discord link: https://discord.com/invite/3kux4YeHmP")
Sta2:Button("Copy link", function()
end)
----------------------------------------------------------------------------------------------------------------------------------------
--Shops - Miscs
S:Seperator("Shops")
S:Dropdown("Select Melee", WeaponsList, "", function(Value)
	getgenv().SelectMelee = Value
end)
S:Button("Buy Selected Melee", function()
	if getgenv().SelectMelee == "Dark Step" then
		RS.Remotes.CommF_:InvokeServer("BuyBlackLeg")
	elseif getgenv().SelectMelee == "Electro" then
		RS.Remotes.CommF_:InvokeServer("BuyElectro")
	elseif getgenv().SelectMelee == "Fishman Karate" then
		RS.Remotes.CommF_:InvokeServer("BuyFishmanKarate")
	elseif getgenv().SelectMelee == "Dragon Claw" then
		RS.CommF_:InvokeServer("BlackbeardReward", "DragonClaw", "1")
		RS.Remotes.CommF_:InvokeServer("BlackbeardReward", "DragonClaw", "2")
	elseif getgenv().SelectMelee == "SuperHuman" then
		RS.Remotes.CommF_:InvokeServer("BuySuperhuman")
	elseif getgenv().SelectMelee == "Death Step" then
		RS.Remotes.CommF_:InvokeServer("BuyDeathStep")
	elseif getgenv().SelectMelee == "Electric Claw" then
		RS.Remotes.CommF_:InvokeServer("BuyElectricClaw")
	elseif getgenv().SelectMelee == "SharkMan Karate" then
		RS.Remotes.CommF_:InvokeServer("BuySharkmanKarate", true)
		RS.Remotes.CommF_:InvokeServer("BuySharkmanKarate")
	elseif getgenv().SelectMelee == "Dragon Talon" then
		RS.Remotes.CommF_:InvokeServer("BuyDragonTalon")
	elseif getgenv().SelectMelee == "God Human" then
		RS.Remotes.CommF_:InvokeServer("BuyGodhuman")
	elseif getgenv().SelectMelee == "Sanguine Art" then
		RS.Remotes.CommF_:InvokeServer("BuySanguineArt")
	end
end)
S:Dropdown("Select Skills", SkillsList, "", function(Value)
	getgenv().SelectSkills = Value
end)
S:Button("Buy Selected Skills", function()
	if getgenv().SelectSkills == "Geppo" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki", "Geppo")
	elseif getgenv().SelectSkills == "Soru" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki", "Soru")
	elseif getgenv().SelectSkills == "Ken Haki" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk", "Buy")
	elseif getgenv().SelectSkills == "Buso Haki" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki", "Buso")
	end
end)
S:Dropdown("Select Items", ShopsList, "", function(Value)
	getgenv().SelectItems = Value
end)
S:Button("Buy Selected Items", function()
	if getgenv().SelectItems == "Katana [1,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Katana")
	elseif getgenv().SelectItems == "Cutlass [1,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Cutlass")
	elseif getgenv().SelectItems == "Duel Katana [12,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Duel Katana")
	elseif getgenv().SelectItems == "Iron Mace [25,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Iron Mace")
	elseif getgenv().SelectItems == "Pipe [100,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Pipe")
	elseif getgenv().SelectItems == "Triple Katana [60,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Triple Katana")
	elseif getgenv().SelectItems == "Dual-Headed Blade [400,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Dual-Headed Blade")
	elseif getgenv().SelectItems == "Bisento [1,000,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Bisento")
	elseif getgenv().SelectItems == "Soul Cane [750,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Soul Cane")
	elseif getgenv().SelectItems == "Slingshot [5,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Slingshot")
	elseif getgenv().SelectItems == "Musket [8,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Musket")
	elseif getgenv().SelectItems == "Flintlock [10,500]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Flintlock")
	elseif getgenv().SelectItems == "Refined Flintlock [65,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Refined Flintlock")
	elseif getgenv().SelectItems == "Cannon [100,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Cannon")
	elseif getgenv().SelectItems == "Kabucha [1500F]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Slingshot", "1")
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Slingshot", "2")
	elseif getgenv().SelectItems == "Black Cape [50,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Black Cape")
	elseif getgenv().SelectItems == "Toemo Ring [500,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Tomoe Ring")
	elseif getgenv().SelectItems == "Swordsman Hat [150,000]" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem", "Swordsman Hat")
	end
end)
S:Dropdown("Select Others", OthersList, "", function(Value)
	getgenv().SelectOthers = Value
end)
S:Button("Buy Selected Items", function()
	if getgenv().SelectOthers == "Refund Stats" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Refund", "1")
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Refund", "2")
	elseif getgenv().SelectOthers == "Reroll Race" then
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Reroll", "1")
		game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward", "Reroll", "2")
	elseif getgenv().SelectOthers == "Race Ghoul" then
		local args = {
			[1] = "Ectoplasm",
			[2] = "BuyCheck",
			[3] = 4
		}
		RS.Remotes.CommF_:InvokeServer(unpack(args))
		local args = {
			[1] = "Ectoplasm",
			[2] = "Change",
			[3] = 4
		}
		RS.Remotes.CommF_:InvokeServer(unpack(args))
	elseif getgenv().SelectOthers == "Race Cyborg" then
		local args = {
			[1] = "CyborgTrainer",
			[2] = "Buy"
		}
		RS.Remotes.CommF_:InvokeServer(unpack(args))
	end
end)
M:Seperator("Servers")
M:Button("Rejoin Server", function()
	game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
end)
M:Button("Hop Servers", function()
	Hop()
end)
M:Seperator("Ui Open")
M:Button("Open Devil Fruit Shop", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
	game:GetService("Players").LocalPlayer.PlayerGui.Main.FruitShop.Visible = true
end)
M:Button("Open Haki Color", function()
	game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end)
M:Button("Open Title Name", function()
	local args = {
		[1] = "getTitles"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end)
M:Button("Open Awakening", function()
	game:GetService("Players").LocalPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
end)
M:Seperator("Teams")
M:Button("Join Pirates Team", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam", "Pirates")
end)
M:Button("Join Marines Team", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam", "Marines")
end)
M:Seperator("Others")
M:Button("Rain Fruit", function()
	for i, v in pairs(game:GetObjects("rbxassetid://14759368201")[1]:GetChildren()) do
		v.Parent = game.Workspace.Map
		v:MoveTo(game.Players.LocalPlayer.Character.PrimaryPart.Position + Vector3.new(math.random(-50, 50), 100, math.random(-50, 50)))
		if v.Fruit:FindFirstChild("AnimationController") then
			v.Fruit:FindFirstChild("AnimationController"):LoadAnimation(v.Fruit:FindFirstChild("Idle")):Play()
		end
		v.Handle.Touched:Connect(function(otherPart)
			if otherPart.Parent == game.Players.LocalPlayer.Character then
				v.Parent = game.Players.LocalPlayer.Backpack
				game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
			end
		end)
	end
end)
M:Button("Show Items", function()
	do
		local ui = game:GetService("CoreGui").RobloxGui.Modules.Profile:FindFirstChild("UILibrary")
		if ui then
			ui:Destroy()
		end
	end
	local UserInputService = game:GetService("UserInputService")
	local TweenService = game:GetService("TweenService")
	local RunService = game:GetService("RunService")
	local LocalPlayer = game:GetService("Players").LocalPlayer
	local Mouse = LocalPlayer:GetMouse()
	do
		local ui = game:GetService("Lighting"):FindFirstChild("Blur")
		if ui then
			ui:Destroy()
		end
	end
	local Blur = Instance.new("BlurEffect")
	TweenService:Create(
                    Blur,
                    TweenInfo.new(.4, Enum.EasingStyle.Back, Enum.EasingDirection.InOut),
                    {
		Size = 50
	}
                ):Play()
	Blur.Parent = game.Lighting
	local UIStroke = Instance.new("UIStroke")
	local UICorner = Instance.new("UICorner")
	local ScreenGui = Instance.new("ScreenGui")
	local ImageButton = Instance.new("ImageButton")
	local RobloxButton = Enum.ButtonStyle.RobloxButton
	ScreenGui.Parent = game.CoreGui
	ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	local cac = require(game:GetService("Players").LocalPlayer.PlayerGui.Main.UIController.Inventory)
	local Inventory = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventory")
	local Items = {}
	local RaityLevel = {
		"Mythical",
		"Legendary",
		"Rare",
		"Uncommon",
		"Common"
	}
	local RaityColor = {
		["Common"] = Color3.fromRGB(179, 179, 179),
		["Uncommon"] = Color3.fromRGB(92, 140, 211),
		["Rare"] = Color3.fromRGB(140, 82, 255),
		["Legendary"] = Color3.fromRGB(213, 43, 228),
		["Mythical"] = Color3.fromRGB(238, 47, 50)
	}
	function GetRaity(color)
		for k, v in pairs(RaityColor) do
			if v == color then
				return k
			end
		end
	end
	for k, v in pairs(Inventory) do
		Items[v.Name] = v
	end
    local total = getupvalue and #getupvalue(cac.UpdateRender, 4) or debug and debug.getupvalue and #debug.getupvalue(cac.UpdateRender, 4) or getupvalues and #getupvalues(cac.UpdateRender)[4] or debug.getupvalues and #debug.getupvalues(cac.UpdateRender)[4]
	local rac = {}
	local allitem = {}
	local total2 = 0
	while total2 < total do
		local i = 0
		while i < 25000 and total2 < total do
			game:GetService("Players").LocalPlayer.PlayerGui.Main.InventoryContainer.Right.Content.ScrollingFrame.CanvasPosition =
                            Vector2.new(0, i)
			for k, v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Main.InventoryContainer.Right.Content.ScrollingFrame.Frame:GetChildren()) do
				if v:IsA("Frame") and not rac[v.ItemName.Text] and v.ItemName.Visible == true then
					local vaihuhu = GetRaity(v.Background.BackgroundColor3)
					if vaihuhu then
						if not allitem[vaihuhu] then
							allitem[vaihuhu] = {}
						end
						table.insert(allitem[vaihuhu], v:Clone())
					end
					total2 = total2 + 1
					rac[v.ItemName.Text] = true
				end
			end
			i = i + 20
		end
		wait()
	end
	function GetXY(vec)
		return vec * 100
	end
	local tvk = Instance.new("UIListLayout")
	tvk.FillDirection = Enum.FillDirection.Vertical
	tvk.SortOrder = 2
	tvk.Padding = UDim.new(0, 10)
	local Left = Instance.new("Frame", game.Players.LocalPlayer.PlayerGui.BubbleChat)
	Left.BackgroundTransparency = 1
	Left.Size = UDim2.new(.5, 0, 1, 0)
	tvk.Parent = Left
	local Right = Instance.new("Frame", game.Players.LocalPlayer.PlayerGui.BubbleChat)
	Right.BackgroundTransparency = 1
	Right.Size = UDim2.new(.5, 0, 1, 0)
	Right.Position = UDim2.new(.6, 0, 0, 0)
	tvk:Clone().Parent = Right
	for k, v in pairs(allitem) do
		local cac = Instance.new("Frame", Left)
		cac.BackgroundTransparency = 1
		cac.Size = UDim2.new(1, 0, 0, 0)
		cac.LayoutOrder = table.find(RaityLevel, k)
		local cac2 = Instance.new("Frame", Right)
		cac2.BackgroundTransparency = 1
		cac2.Size = UDim2.new(1, 0, 0, 0)
		cac2.LayoutOrder = table.find(RaityLevel, k)
		local tvk = Instance.new("UIGridLayout", cac)
		tvk.CellPadding = UDim2.new(.005, 0, .005, 0)
		tvk.CellSize = UDim2.new(0, 70, 0, 70)
		tvk.FillDirectionMaxCells = 100
		tvk.FillDirection = Enum.FillDirection.Horizontal
		local ccc = tvk:Clone()
		ccc.Parent = cac2
		for k, v in pairs(v) do
			if Items[v.ItemName.Text] and Items[v.ItemName.Text].Mastery then
				if v.ItemLine2.Text ~= "Accessory" then
					local bucac                  = v.ItemName:Clone()
					bucac.BackgroundTransparency = 1
					bucac.TextSize               = 10
					bucac.TextXAlignment         = 2
					bucac.TextYAlignment         = 2
					bucac.ZIndex                 = 5
					bucac.Text                   = Items[v.ItemName.Text].Mastery
					bucac.Size                   = UDim2.new(.5, 0, .5, 0)
					bucac.Position               = UDim2.new(.5, 0, .5, 0)
					bucac.Parent                 = v
				end
				v.Parent = cac
			elseif v.ItemLine2.Text == "Blox Fruit" then
				v.Parent = cac2
			end
		end
		cac.AutomaticSize = 2
		cac2.AutomaticSize = 2
	end
	local ListHuhu = {
		["Superhuman"] = Vector2.new(3, 2),
		["DeathStep"] = Vector2.new(4, 3),
		["ElectricClaw"] = Vector2.new(2, 0),
		["SharkmanKarate"] = Vector2.new(0, 0),
		["DragonTalon"] = Vector2.new(1, 5)
	}
	local MeleeG = Instance.new("Frame", Left)
	MeleeG.BackgroundTransparency = 1
	MeleeG.Size = UDim2.new(1, 0, 0, 0)
	MeleeG.LayoutOrder = table.find(RaityLevel, k)
	MeleeG.AutomaticSize = 2
	MeleeG.LayoutOrder = 100
	local tvk = Instance.new("UIGridLayout", MeleeG)
	tvk.CellPadding = UDim2.new(.005, 0, .005, 0)
	tvk.CellSize = UDim2.new(0, 70, 0, 70)
	tvk.FillDirectionMaxCells = 100
	tvk.FillDirection = Enum.FillDirection.Horizontal
	local cac = {
		"Superhuman",
		"ElectricClaw",
		"DragonTalon",
		"SharkmanKarate",
		"DeathStep",
		"GodHuman"
	}
	for k, v in pairs(cac) do
		if ListHuhu[v] and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buy" .. v, true) == 1 then
			local huhu = Instance.new("ImageLabel", MeleeG)
			huhu.Image = "rbxassetid://9945562382"
			huhu.ImageRectSize = Vector2.new(100, 100)
			huhu.ImageRectOffset = ListHuhu[v] * 100
		end
	end
	function formatNumber(v)
		return tostring(v):reverse():gsub("%d%d%d", "%1,"):reverse():gsub("^,", "")
	end
	game:GetService("Players").LocalPlayer.PlayerGui.Main.Beli.AnchorPoint = Vector2.new(0.5, 0.5)
	game:GetService("Players").LocalPlayer.PlayerGui.Main.Beli.Position = UDim2.new(0, 1120, 0, 700)
	game:GetService("Players").LocalPlayer.PlayerGui.Main.Level.AnchorPoint = Vector2.new(0.5, 0.5)
	game:GetService("Players").LocalPlayer.PlayerGui.Main.Level.Position = UDim2.new(0, 1150, 0, 750)
	local Name = game:GetService("Players").LocalPlayer.PlayerGui.Main.Fragments:Clone()
	Name.Name = "Name"
	Name.Parent = game:GetService("Players").LocalPlayer.PlayerGui.Main.Beli
	Name.Position = UDim2.new(0, 0, -1.5, 0)
	Name.Size = UDim2.new(1, 0, 1, 0)
	Name.TextColor3 = Color3.fromRGB(255, 255, 255)
	Name.Text = game.Players.LocalPlayer.Name
	local Fragments = game:GetService("Players").LocalPlayer.PlayerGui.Main.Fragments:Clone()
	Fragments.Name = "FragmentsCheck"
	Fragments.Parent = game:GetService("Players").LocalPlayer.PlayerGui.Main.Beli
	Fragments.Position = UDim2.new(0, 0, -0.75, 0)
	Fragments.Size = UDim2.new(1, 0, 1, 0)
	Fragments.Text = 'ƒ' .. formatNumber(game:GetService("Players").LocalPlayer.Data.Fragments.Value)
	local args = {
		[1] = "getAwakenedAbilities"
	}
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
	game.Players.LocalPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
	game:GetService("Players").LocalPlayer.PlayerGui.Main.AwakeningToggler.Position = UDim2.new(0.48, 10, 0.908, 2)
	game:GetService("Players").LocalPlayer.PlayerGui.Main.AwakeningToggler.Size = UDim2.new(1, 0, 0.22, 0)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.MenuButton.Visible = false
	end)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.RaceEnergy.Visible = false
	end)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.SafeZone.Visible = false
	end)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.HP.Visible = false
	end)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Backpack.Enabled.Visible = false
	end)
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.Energy.Visible = false
	end)
	for k, v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Main:GetChildren()) do
		if v:IsA("ImageButton") then
			v:Destroy()
		end
	end
	pcall(function()
		game:GetService("Players").LocalPlayer.PlayerGui.Main.Compass.Visible = false
	end)
end)
M:Seperator("Musics")
M:Dropdown("Select Musics", ListMusics, "", function(Value)
	getgenv().SelectMusics = Value
end)
M:Toggle("Start Play Music (dont reset or die)", false, function(Value)
	game.Players.LocalPlayer.Character.HumanoidRootPart.Sound.Playing = Value
end)

local songs = {
    ["Quốc Ca Việt Nam"] = "1845922899",
    ["Shine"] = "1842095470",
    ["No Sleep"] = "7029011778",
    ["Night Out (feat. Esther Dee)"] = "1843324953",
    ["2 Guns"] = "17422075096",
    ["I Love (slow+reverb version)"] = "15689455422",
    ["Alone"] = "16190782786",
    ["Diss na Hagi Lagi (Nightcore)"] = "14366983688",
    ["Fatal Breath"] = "15689447272",
    ["Dream Girl (sped up)"] = "15689457918",
    ["Reason to Stay"] = "9038730676",
    ["SOS"] = "6901063458",
    ["Squid Game"] = "7535587224",
    ["Phonk #5"] = "6911766512",
    ["MisChief"] = "1836362602",
    ["WRLD Hang Up"] = "5410084188",
    ["Sad"] = "135308045",
    ["White Tee"] = "9087418452",
    ["Ocean Eyes"] = "5410085296",
    ["Broken Glass"] = "7028799370",
    ["Same Mistake"] = "7024101188",
    ["Thinking About You"] = "7028540590",
    ["Hold On"] = "7029005367",
    ["New World"] = "5410082346",
    ["Rest For Life"] = "9045395415",
    ["Vip Me"] = "1838028467",
    ["Color"] = "7023828725",
    ["Crab Rave"] = "5410086218",
    ["Unbreakable"] = "14145626744",
    ["Can You ?"] = "15689448519",
    ["Only You"] = "7024028859",
    ["Chipi Chipi Speed"] = "16190783444",
    ["Không Nên Tò Mò"] = "7000891754",
    ["Blod Blod"] = "6783714255",
    ["Phonk #4"] = "1842652230",
    ["Phonk #3"] = "13530439660",
    ["Free Fire"] = "7634196777",
    ["Play It Cool"] = "7029017448",
    ["Phonk #2"] = "15689451063",
    ["Stay"] = "9062549544",
    ["Phonk #1"] = "15689443663",
    ["Gambare Senpai"] = "7431081635",
    ["Gojo"] = "7896694622",
    ["Din1c-DOWN2KILL"] = "16190760285",
    ["Waka Waka"] = "5506713323",
    ["Rickroll"] = "7363412529",
    ["Preytty Girl"] = "6574868925",
}
-- chat gpt code for real
spawn(function()
    pcall(function()
        while wait(0.3) do
            local selectedMusic = getgenv().SelectMusics
            local soundId = songs[selectedMusic]
            if soundId then
                game.Players.LocalPlayer.Character.HumanoidRootPart.Sound.SoundId = ContentProvider.BaseUrl .. "asset/?id=" .. soundId
            end
        end
    end)
end)

