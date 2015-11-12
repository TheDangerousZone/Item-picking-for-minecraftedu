ItemPick
CODE
local Item
local Inventory

Item = 1

turtle.select( Item )

for Inventory = 1, 15 do

  if turtle.getItemCount() == 0 then
    Item = Item + 1
    turtle.select( Item )
  end
end
