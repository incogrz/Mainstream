local brick = script.Parent

local function onTouch(part)
    local character = part.Parent
    local humanoid = character:FindFirstChildOfClass("Humanoid")
    if humanoid then
        humanoid.Health = 0
    end
end

brick.Touched:Connect(onTouch)
