local E = 6.5
local F = CFrame.new(-596.0128173828125, 308.015625, -1143.5589599609375)

A1 = F.x
A2 = F.y
A3 = F.z

function Left(Num)
for g = 1,Num do wait()
A1 = A1 - E
game:GetService("ReplicatedStorage").Events.PlaceStructure:FireServer("Plant Box",CFrame.new(A1, A2, A3),0)
end
end

function UP(Num)
for g = 1,Num do wait()
A3 = A3 - E
game:GetService("ReplicatedStorage").Events.PlaceStructure:FireServer("Plant Box",CFrame.new(A1, A2, A3),0)
end
end

function Right(Num)
for g = 1,Num do wait()
A1 = A1 + E
game:GetService("ReplicatedStorage").Events.PlaceStructure:FireServer("Plant Box",CFrame.new(A1, A2, A3),0)
end
end

function Down(Num)
for g = 1,Num do wait()
A3 = A3 + E
game:GetService("ReplicatedStorage").Events.PlaceStructure:FireServer("Plant Box",CFrame.new(A1, A2, A3),0)
end
end

Right(3)
Left(6)
UP(3)
Right(6)
Down(6)
Left(6)
UP(2)
Right(5)
Down(1)
Left(4)
UP(4)
Right(4)
Down(1)
Left(5)
UP(3)

for g = 1,6 do wait()
Right(6)
UP(1)
Left(6)
UP(1)
end

Right(6)
