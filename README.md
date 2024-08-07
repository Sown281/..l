# ..l
local Hits = {}  Part.Touched:Connect(function(Hit)  if Hit.Parent:FindFirstChild("Humanoid") then   if Hits[Hit.Parent.Name] then    return   end   Hits[Hit.Parent.Name] = true   Hit.Parent.Humanoid:TakeDamage(5)  end end)
