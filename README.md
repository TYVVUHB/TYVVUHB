tu masz jebany skrypt ok?

**game.StarterGui:SetCore("ChatMakeSystemMessage", {
    Text = "Skrypt stworzony przez dwóch debili TYVVUHB I WojoX";
    Color = Color3.new(255, 0, 72);
    Font = Enum.Font.SourceSansBold;
    FontSize = Enum.FontSize.Size24;
})

game.StarterGui:SetCore("ChatMakeSystemMessage", {
    Text = "UWAGA JESLI dostaniesz bana to masz problem uzyj [alt account] było nie czitować!";
    Color = Color3.new(255, 0, 0);
    Font = Enum.Font.SourceSansBold;
    FontSize = Enum.FontSize.Size24;
})


local SkidParkour = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local Functions = Instance.new("Frame")
local CTP = Instance.new("TextButton")
local NameESP = Instance.new("TextButton")
local TPBACK = Instance.new("TextButton")
local TPORB = Instance.new("TextButton")
local TPPlayer = Instance.new("TextButton")
local InputPlayer = Instance.new("TextBox")
local NoFall = Instance.new("TextButton")
local Walkspeed = Instance.new("TextButton")
local Btools = Instance.new("TextButton")
local Gravity = Instance.new("TextButton")
local Settings = Instance.new("Frame")
local WhiteBackground = Instance.new("Frame")
local FormCheck = Instance.new("Frame")
local Form = Instance.new("TextLabel")
local White = Instance.new("TextLabel")
local del = Instance.new("TextButton")
local Credits = Instance.new("Frame")
local Outer = Instance.new("ImageLabel")
local Discord = Instance.new("TextLabel")
local Alone = Instance.new("ImageLabel")
local Discord_2 = Instance.new("TextLabel")
local ROexploits = Instance.new("ImageLabel")
local Discord_3 = Instance.new("TextLabel")
local TextLabel = Instance.new("TextLabel")
local TabList = Instance.new("Frame")
local FunctionsBTN = Instance.new("TextButton")
local SettingsBTN = Instance.new("TextButton")
local CreditsBTN_2 = Instance.new("TextButton")
local Title = Instance.new("TextLabel")
local Close = Instance.new("TextButton")

Main.Name = "Główne"
Main.Parent = SkidParkour
Main.Active = true
Main.Draggable = true
Main.BackgroundColor3 = Color3.new(0.133333, 0.141176, 0.176471)
Main.BackgroundTransparency = 1
Main.BorderSizePixel = 0
Main.Position = UDim2.new(0.26029411, 0, 0.32432431, 0)
Main.Size = UDim2.new(0, 676, 0, 323)

Functions.Name = "Funkcje"
Functions.Parent = Main
Functions.BackgroundColor3 = Color3.new(0.133333, 0.141176, 0.176471)
Functions.BorderSizePixel = 0
Functions.Size = UDim2.new(0, 676, 0, 285)
Functions.Visible = true


CTP.Name = "KTP"
CTP.Parent = Functions
CTP.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
CTP.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
CTP.Position = UDim2.new(0.0695266277, 0, 0.259649128, 0)
CTP.Size = UDim2.new(0, 112, 0, 24)
CTP.Font = Enum.Font.SourceSansLight
CTP.Text = "Aby się tepnąć kliknij [Z]"
CTP.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
CTP.TextSize = 18
CTP.MouseButton1Click:connect(function()
	plr = game.Players.LocalPlayer;
	hum = plr.Character.HumanoidRootPart;
	mouse = plr:GetMouse()
	mouse.KeyDown:connect(function(aa)
		if aa == "z" then
			if mouse.Target then
				hum.CFrame = CFrame.new(mouse.Hit.x, mouse.Hit.y + 5, mouse.Hit.z)
			end
		end
	end)
end)


NameESP.Name = "NameESP"
NameESP.Parent = Functions
NameESP.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
NameESP.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
NameESP.Position = UDim2.new(0.0695266277, 0, 0.3859649, 0)
NameESP.Size = UDim2.new(0, 112, 0, 24)
NameESP.Font = Enum.Font.SourceSansLight
NameESP.Text = "Name ESP"
NameESP.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
NameESP.TextSize = 18
NameESP.MouseButton1Click:connect(function()
    Important = {

        Players = game:GetService("Gracze"),
		Workspace = game:GetService("Workspace"),
		CoreGui = game:WaitForChild("Rdzeń Moda")

	}
	local ai = false;
	function CreateESP(plr)
		if plr ~= nil then
			local aj = plr.Character;
			if not aj then
				return
            end;
			local ak;
			do
                repeat
					wait()
				until aj:FindFirstChild("Head")
			end;
			ak = aj.Head;
			local al = Instance.new("BillboardGui", Important.CoreGui)
			al.Adornee = ak;
			al.ExtentsOffset = Vector3.new(0, 1, 0)
			al.AlwaysOnTop = true;
			al.Size = UDim2.new(0, 5, 0, 5)
			al.StudsOffset = Vector3.new(0, 3, 0)
			al.Name = "ESP_PLAYER_"..plr.Name;
			local am = Instance.new("Frame", al)
			am.ZIndex = 10;
			am.BackgroundTransparency = 1;
			am.Size = UDim2.new(1, 0, 1, 0)
			local an = Instance.new("TextLabel", am)
			an.Name = "Name"
			an.ZIndex = 10;
			an.Text = plr.Name;
			an.Visible = true;
			an.TextColor3 = Color3.new(255, 45, 126)
			an.BackgroundTransparency = 1;
			an.Size = UDim2.new(1, 0, 10, 0)
			an.Font = Enum.Font.SourceSansLight;
			an.TextSize = 20;
			an.TextStrokeTransparency = .5
		end
	end;
	for ag, ah in pairs(Important.Players:GetChildren()) do
		if game.GameId == 445664957 then
			return
		end;  

        CreateESP(ah)
	end
end)
 
TPBACK.Name = "TPBACK"
TPBACK.Parent = Functions
TPBACK.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
TPBACK.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
TPBACK.Position = UDim2.new(0.0695266277, 0, 0.519298255, 0)
TPBACK.Size = UDim2.new(0, 112, 0, 24)
TPBACK.Font = Enum.Font.SourceSansLight
TPBACK.Text = "teleport do skinów"
TPBACK.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
TPBACK.TextSize = 18

TPORB.Name = "TPORB"
TPORB.Parent = Functions
TPORB.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
TPORB.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
TPORB.Position = UDim2.new(0.0695266277, 0, 0.65263164, 0)
TPORB.Size = UDim2.new(0, 112, 0, 24)
TPORB.Font = Enum.Font.SourceSansLight
TPORB.Text = "teleport do jakiś orbów XD"
TPORB.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
TPORB.TextSize = 18

TPPlayer.Name = "TPPlayer"
TPPlayer.Parent = Functions
TPPlayer.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
TPPlayer.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
TPPlayer.Position = UDim2.new(0.334319532, 0, 0.519298255, 0)
TPPlayer.Size = UDim2.new(0, 183, 0, 36)
TPPlayer.Font = Enum.Font.SourceSansLight
TPPlayer.Text = "Teleport do pajaców"
TPPlayer.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
TPPlayer.TextSize = 18
TPPlayer.MouseButton1Down:connect(function()
	local tp_namedplayer = InputPlayer.Text
	local tp_player = game:GetService("Players")[tp_namedplayer]
	local PLR = game:GetService("Players").LocalPlayer
	local p = InputPlayer.Text

    if tp_player then 
        for i = 1,2 do
    wait(.08)
    PLR.Character.HumanoidRootPart.CFrame = tp_player.Character.HumanoidRootPart.CFrame + Vector3.new(0, 3, 0)
    end
end
end)

 
InputPlayer.Name = "połóż greacza ok?"
InputPlayer.Parent = Functions
InputPlayer.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
InputPlayer.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
InputPlayer.Position = UDim2.new(0.334319532, 0, 0.343859643, 0)
InputPlayer.Size = UDim2.new(0, 182, 0, 35)
InputPlayer.Font = Enum.Font.SourceSans
InputPlayer.PlaceholderColor3 = Color3.new(0.780392, 0.780392, 0.780392)
InputPlayer.PlaceholderText = "199, 199, 199"
InputPlayer.Text = "połóż gracza ok?"
InputPlayer.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
InputPlayer.TextSize = 16

Walkspeed.Name = "szybkość[dej na maksa]"
Walkspeed.Parent = Functions
Walkspeed.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
Walkspeed.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
Walkspeed.Position = UDim2.new(0.69970417, 0, 0.259649128, 0)
Walkspeed.Size = UDim2.new(0, 113, 0, 24)
Walkspeed.Font = Enum.Font.SourceSansLight
Walkspeed.Text = "szybkość[X]"
Walkspeed.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
Walkspeed.TextSize = 18
Walkspeed.MouseButton1Down:connect(function()
	local walkspeedplayer = game:GetService("Players").LocalPlayer
	local walkspeedmouse = walkspeedplayer:GetMouse()

    local walkspeedenabled = false
 
	function x_walkspeed(key)
		if (key == "x") then
			if walkspeedenabled == false then
				_G.WS = 125;
				local Humanoid = game:GetService("Players").LocalPlayer.Character.Humanoid;
				Humanoid:GetPropertyChangedSignal("WalkSpeed"):Connect(function()
				Humanoid.WalkSpeed = _G.WS;
				end)
				Humanoid.WalkSpeed = _G.WS;
 
				walkspeedenabled = true
			elseif walkspeedenabled == true then
				_G.WS = 40;
				local Humanoid = game:GetService("Players").LocalPlayer.Character.Humanoid;
				Humanoid:GetPropertyChangedSignal("WalkSpeed"):Connect(function()
				Humanoid.WalkSpeed = _G.WS;
				end)
				Humanoid.WalkSpeed = _G.WS;

                alkspeedenabled = false
			end
		end
	end
 
	walkspeedmouse.KeyDown:connect(x_walkspeed)
 
end)

Btools.Name = "Btoolsy kurwa ok?"
Btools.Parent = Functions
Btools.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
Btools.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
Btools.Position = UDim2.new(0.69970417, 0, 0.3859649, 0)
Btools.Size = UDim2.new(0, 113, 0, 24)
Btools.Font = Enum.Font.SourceSansLight
Btools.Text = "BTOOOLSY"
Btools.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
Btools.TextSize = 18
Btools.MouseButton1Down:connect(function()
	game.StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.Backpack, true)
for index, child in pairs(game:GetService("Workspace"):GetChildren()) do
   if child.ClassName == "Part" then
       child.Locked = false
   end
   if child.ClassName == "MeshPart" then
    child.Locked = false
end
if child.ClassName == "UnionOperation" then
    child.Locked = false
end
if child.ClassName == "Model" then
    for index, chil in pairs(child:GetChildren()) do
        if chil.ClassName == "Part" then
            chil.Locked = false
        end
        if chil.ClassName == "MeshPart" then
            chil.Locked = false
        end
        if chil.ClassName == "UnionOperation" then
            chil.Locked = false
        end
        if chil.ClassName == "Model" then
            for index, childe in pairs(chil:GetChildren()) do
                if childe.ClassName == "Part" then
                    childe.Locked = false
                end
                if childe.ClassName == "MeshPart" then
                    childe.Locked = false
                end
                if childe.ClassName == "UnionOperation" then
                    childe.Locked = false
                end
                if childe.ClassName == "Model" then
                    for index, childeo in pairs(childe:GetChildren()) do
                        if childeo.ClassName == "Part" then
                            childeo.Locked = false
                        end
                        if childeo.ClassName == "MeshPart" then
                            childeo.Locked = false
                        end
                        if childeo.ClassName == "UnionOperation" then
                            childeo.Locked = false
                        end
                        if childeo.ClassName == "Model" then
                        end
                    end
                end
            end
        end
    end
end
end


c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Hammer
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Clone
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Grab
end)

Gravity.Name = "Grawitacja"
Gravity.Parent = Functions
Gravity.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
Gravity.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
Gravity.Position = UDim2.new(0.69970417, 0, 0.519298255, 0)
Gravity.Size = UDim2.new(0, 113, 0, 24)
Gravity.Font = Enum.Font.SourceSansLight
Gravity.Text = "Grawitacja"
Gravity.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
Gravity.TextSize = 18
Gravity.MouseButton1Down:connect(function()
if Gravity == true then
Gravity = false
game.workspace.Gravity = 90
else
Gravity = true
game.workspace.Gravity = 45
end
end)
 
Settings.Name = "Ustawienia"
Settings.Parent = Main
Settings.BackgroundColor3 = Color3.new(0.133333, 0.141176, 0.176471)
Settings.BorderSizePixel = 0
Settings.Size = UDim2.new(0, 676, 0, 285)
Settings.Visible = false
 
WhiteBackground.Name = "Biały EKRAN"
WhiteBackground.Parent = Settings
WhiteBackground.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
WhiteBackground.BorderSizePixel = 0
WhiteBackground.Position = UDim2.new(0.0325443782, 0, 0.228070185, 0)
WhiteBackground.Size = UDim2.new(0, 18, 0, 18)

FormCheck.Name = "FormCheck"
FormCheck.Parent = Settings
FormCheck.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
FormCheck.BorderSizePixel = 0
FormCheck.Position = UDim2.new(0.0325443782, 0, 0.105263159, 0)
FormCheck.Size = UDim2.new(0, 18, 0, 18)
 
Form.Name = "Formy"
Form.Parent = Settings
Form.BackgroundColor3 = Color3.new(1, 1, 1)
Form.BackgroundTransparency = 1
Form.Position = UDim2.new(0.0719999969, 0, 0.112999998, 0)
Form.Size = UDim2.new(0, 113, 0, 12)
Form.Font = Enum.Font.SourceSans
Form.Text = "możesz draggklikować"
Form.TextColor3 = Color3.new(0.815686, 0.835294, 0.901961)
Form.TextSize = 15
 
White.Name = "Biały"
White.Parent = Settings
White.BackgroundColor3 = Color3.new(1, 1, 1)
White.BackgroundTransparency = 1
White.Position = UDim2.new(0.0591716208, 0, 0.225999996, 0)
White.Size = UDim2.new(0, 106, 0, 18)
White.Font = Enum.Font.SourceSans
White.Text = "Biały EKRAN"
White.TextColor3 = Color3.new(0.815686, 0.835294, 0.901961)
White.TextSize = 15
 
del.Name = "del"
del.Parent = Settings
del.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
del.BorderColor3 = Color3.new(0.356863, 0.388235, 0.470588)
del.Position = UDim2.new(0.0325443782, 0, 0.824561417, 0)
del.Size = UDim2.new(0, 124, 0, 25)
del.Font = Enum.Font.SourceSansLight
del.Text = "Un-Inject GUI"
del.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
del.TextSize = 20
del.MouseButton1Down:connect(function()
Main:Destroy()
end)
 
 
Credits.Name = "jakieś gówna"
Credits.Parent = Main
Credits.BackgroundColor3 = Color3.new(0.133333, 0.141176, 0.176471)
Credits.BorderSizePixel = 0
Credits.Size = UDim2.new(0, 676, 0, 285)
Credits.Visible = false
 


 
Discord.Name = "Discord"
Discord.Parent = Outer
Discord.BackgroundColor3 = Color3.new(1, 1, 1)
Discord.BackgroundTransparency = 100
Discord.Position = UDim2.new(-0.206349224, 0, 1.07200003, 0)
Discord.Size = UDim2.new(0, 177, 0, 50)
Discord.Font = Enum.Font.SourceSansItalic
Discord.Text = "POMOC TYVVUHB#0407"
Discord.TextColor3 = Color3.new(1, 0.168627, 0.847059)
Discord.TextSize = 19

 
Discord_2.Name = "Discord"
Discord_2.Parent = Alone
Discord_2.BackgroundColor3 = Color3.new(1, 1, 1)
Discord_2.BackgroundTransparency = 100
Discord_2.Position = UDim2.new(-0.0317460299, 0, 1.07200003, 0)
Discord_2.Size = UDim2.new(0, 134, 0, 50)
Discord_2.Font = Enum.Font.SourceSansItalic
Discord_2.Text = "Twórcy:  TYVVUHB i Siemka12345109#6994"
Discord_2.TextColor3 = Color3.new(1, 0.317647, 0)
Discord_2.TextSize = 19
 
 
TabList.Name = "TAB LISTA"
TabList.Parent = Main
TabList.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
TabList.BorderSizePixel = 0
TabList.Position = UDim2.new(0, 0, 0.882352948, 0)
TabList.Size = UDim2.new(0, 676, 0, 38)
 
FunctionsBTN.Name = "FUNKCJE BTN"
FunctionsBTN.Parent = TabList
FunctionsBTN.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
FunctionsBTN.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
FunctionsBTN.Position = UDim2.new(0.289940834, 0, 0.184210539, 0)
FunctionsBTN.Size = UDim2.new(0, 82, 0, 24)
FunctionsBTN.Font = Enum.Font.SourceSansLight
FunctionsBTN.Text = "Funkcje"
FunctionsBTN.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
FunctionsBTN.TextSize = 20
FunctionsBTN.MouseButton1Down:connect(function()
Functions.Visible = true
Settings.Visibe = false
Credits.Visible = false
end)
 
SettingsBTN.Name = "USTAWIENIABTN"
SettingsBTN.Parent = TabList
SettingsBTN.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
SettingsBTN.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
SettingsBTN.Position = UDim2.new(0.437869817, 0, 0.184210539, 0)
SettingsBTN.Size = UDim2.new(0, 82, 0, 24)
SettingsBTN.Font = Enum.Font.SourceSansLight
SettingsBTN.Text = "USTAWIENIA"
SettingsBTN.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
SettingsBTN.TextSize = 20
SettingsBTN.MouseButton1Down:connect(function()
Functions.Visible = false
Settings.Visibe = true
Credits.Visible = false
end)
 
CreditsBTN_2.Name = "INNEBTN"
CreditsBTN_2.Parent = TabList
CreditsBTN_2.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
CreditsBTN_2.BorderColor3 = Color3.new(0.470588, 0.513726, 0.623529)
CreditsBTN_2.Position = UDim2.new(0.587278128, 0, 0.184210539, 0)
CreditsBTN_2.Size = UDim2.new(0, 82, 0, 24)
CreditsBTN_2.Font = Enum.Font.SourceSansLight
CreditsBTN_2.Text = "INNE"
CreditsBTN_2.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
CreditsBTN_2.TextSize = 20
CreditsBTN_2.MouseButton1Down:connect(function()
Functions.Visible = false
Settings.Visibe = false
Credits.Visible = true
end)
 
Title.Name = "Title"
Title.Parent = TabList
Title.BackgroundColor3 = Color3.new(1, 1, 1)
Title.BackgroundTransparency = 1
Title.Position = UDim2.new(0, 0, 0.184210539, 0)
Title.Size = UDim2.new(0, 111, 0, 25)
Title.Font = Enum.Font.SourceSansLight
Title.Text = "SKRYPT OD ZJEBÓW NA PARKOUR"
Title.TextColor3 = Color3.new(0.819608, 0.819608, 0.819608)
Title.TextSize = 14
 
Close.Name = "zamknij"
Close.Parent = Main
Close.BackgroundColor3 = Color3.new(0.0980392, 0.109804, 0.137255)
Close.BorderColor3 = Color3.new(0.215686, 0.231373, 0.286275)
Close.BorderSizePixel = 0
Close.Position = UDim2.new(0.96449703, 0, 0, 0)
Close.Size = UDim2.new(0, 24, 0, 24)
Close.Font = Enum.Font.SourceSansLight
Close.Text = "-"
Close.TextColor3 = Color3.new(0.780392, 0.780392, 0.780392)
Close.TextSize = 24
Close.MouseButton1Down:connect(function()
	Main.Visible = false
	Open.Visible = true
end)

 



