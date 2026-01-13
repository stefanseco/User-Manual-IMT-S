### General notes for Prefabs of Machines and materials
Both Prefabs should have a box collider when they are being made. Additionally the Machine prefabs should all also have the Machine script which has the logic to make the recipes work.
## Step 1: Making the material

1. Open the unity project
2. In the assets open the Machines document 
3. Right click on the Materials folder and click create > Scriptable Objects > Material data
![[Pasted image 20260113120752.png]]
Doing so will make a object that works with the code of the engineers and is streamlined for designers to put functionality

#### Example of a material object
![[Pasted image 20260113121538.png]]
Inside the designer can attach the materials prefab so it can be produced in game as well as its icon that will appear in the inventory and also set its cost 

## Step 2: Making the recipe

1. While in the Machines folder right click the RecipeSO folder and click Create > Scriptable Object > Machine > Machine Recipe

![[Pasted image 20260113121914.png]]
Following these steps will now create a scriptable object that can hold one recipe

![[Pasted image 20260113123146.png]]
Each recipe only works with the materials that the designer has made. The recipe can be modified so that it can take or make as many different materials as the designer wants.


## Step 3: Making the machine
1. While in the Machines folder right click the MachineSO folder and then click Create > Scriptable Objects > Machine > Machine Data
![[Pasted image 20260113140038.png]]
After doing so the designer will have created a Machine scriptable object.

Within the scriptable object there are a lot of elements that the designer can use.
Machine OS elements:
1. Orientation: Picking which way the machine faces north being the prefabs standard rotation
2. Basic Info: Attaching a prefab to the machine as well as an Icon and name that will appear in the shop
3. Production: is and old version of the Recipes section and can only be use for machines that have one recipe
4. Recipes: Adding the Recipe SO that they have made linking them both 
5. Size: Determining the how much space the machine will take up in the factory
6. Repair minigame: What game will pop up when the player is trying to fix the machine
7. Upgrades: To be developed further
8. Conveyor ports: Choosing how many ports there are and how many of them intake materials and output materials
9. Port indicator: Applying a visual indicator for the player to understand where they can feed and produce materials from
10. Machine Breaking: How often the machine can break and what indicators they give for it
![[Pasted image 20260113140502.png]]
![[Pasted image 20260113141136.png]]
![[Pasted image 20260113141624.png]]
## Step 4: Putting all SO in the games data

Putting objects in the data registry makes it so that they can be saved by the games system, each object not in there will be removed from the game when it is closed.
![[Pasted image 20260113142122.png]]