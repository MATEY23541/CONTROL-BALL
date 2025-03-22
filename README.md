debounce = false
 
script.Parent.Touched:Connect(function(hit)
    if hit.Parent:FindFirstChild('Humanoid') and debounce == false then
        debounce = true
        game.Players:FindFirstChild(hit.Parent.Name).PlayerGui.Jumpscare.Enabled = true
        script.Parent.Sound:Play()
        wait(1)
        game.Players:FindFirstChild(hit.Parent.Name).PlayerGui.Jumpscare.Enabled = true
    end
end)
 
-- Sound I Used: https://www.roblox.com/library/4750230490/
-- Image I Used: https://www.roblox.com/library/9244881738/
