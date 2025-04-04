# Atlas Loader V1 [BETA]
- small update, this will allow you to load any of Atlas Hub scripts!
- developed by arayz✅

# Source:

local Rayfield = loadstring(game:HttpGet('https://raw.githubusercontent.com/UI-Interface/CustomFIeld/main/RayField.lua'))()
local Window = Rayfield:CreateWindow({
   Name = "Atlas Hub Loader V1 [BETA]",
   LoadingTitle = "Atlas Hub Loader: Loading...",
   LoadingSubtitle = "Developed by arayz",
   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "AtlasHub"
   },
   Discord = {
      Enabled = false,
      Invite = "bA3msE2Xcj", -- The Discord invite code, do not include discord.gg/
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = false, -- Disable the key system
})

local Tab = Window:CreateTab("Tab Example", 4483362458) -- Title, Image

-- Add the first button
local Button1 = Tab:CreateButton({
   Name = "Atlas Hub | Rivals V2.1.2",
   Info = "Loads Atlas hub Rivals 2.1.2",
   Interact = "Load Rivals",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/VisioneducationOfLuaCoding/Rivals2.1/refs/heads/main/CmdLoader"))()
      print([[
**Features Added:**

- Silent Aim (Legacy)
- Silent Aim Working on Sniper now.
- Set Target Feature - None/Closest

**Support:**
- will not support Xeno⚠️
- will not support Cloudy⚠️
]])

   end,
})

-- Add the second button
local Button2 = Tab:CreateButton({
   Name = "Atlas Hub | Arsenal V1.1.4",
   Info = "Loads the Arsenal script of Atlas Hub",
   Interact = "Load Arsenal",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/VisioneducationOfLuaCoding/ArsenalV1.1.0/refs/heads/main/1.1.3"))()
   end,
})

