# Proyect_Haggins

# Documentation Proyect ID => ChickenDrumsticks
First of all let me scream in anger and vent my frustration
FUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUCK

After said venting of frustration ill procced to use this Readme as to keep tabs on documentation about every aspect of the system I am currently trying to put together to make some great procedurally generated dismemberment with the help of a bunch of internet weirdos.

So without further a do lets get this thing rolling cause its 2:27 AM and I tunneled so hard on this Shi I forgot to go go bed.

## First System Template

The first steps where derived from this video: https://youtu.be/Nt7r2OD8pUQ

Its good and allows a basic understanding for hwo the system might look once fully fleshed out, however it has flaws. 
TIME TO NITPICK HEHEHHEE

### Identifiable flaws:
1. The system was built for UE4 taking out of the equation new tech found on UE5 which means it needs updating
2. It relies on decals and legacy cascade particle emitters in order to show the effects of things happening so that could change a bit
3. Dreaded #3 is the fact that if the model you are using does not have a spine_01 that has no weights assigned to it and also splits the model in half, its useless (big yikes!!)
4. Its not scalable because its not allowing for other models with possible different bone structures to be played with
5. It bloats the system with a crawling side system to make enemies crawl towards you which is a good nick but its not really functional and just bloats the scope of usefulness.
6. Parts blow up and they just get ejected full force on random directions, that is not natural at all.

Now after realizing an extensive critique of the material at hand lets set some basic goals that we might want to achieve by tinkering with this.

### Goals for this system:
1. Fully updated towards UE5 dismemberment system (Just use Niagara for everything visual VFX related)
2. Ground down the system to only make sure things get dismembered and user recieves feedback, no extra stuff like crawling and such that might bloat the project
3. Make it model universal, or at the very list implement a Bone structure detector so that we can define how to correctly deattach the bones
4. Alow for a more detailed dismemberment with a bit less erraticness. We want to achieve a somewhat realistic system

That is all of the goals for now as off the creation of a cool and really dope dismemberment system to be built, lots of work needs to be done however lets do some resource gathering really quickly in order to start gathering info to be able to fix this shiiiiii. Tutorial era is over, now lets start with some good and dirty engeniering work :DDDD.

### Maybe Useful Resource
1. Zombie Lite + Dismemberment system -> Its a free Fab asset you can bring in your projects and we can analyze the way they tacled the issue to hopefully learn from them
2. [UE5 Documentation on how decals work ->](https://dev.epicgames.com/documentation/en-us/unreal-engine/decal-materials-in-unreal-engine) It may be usefull to understand if we want to switch from decals to other systems to show the blood spurts on the ground or use some other UE5 new and handy tool.
3. [UE5 Documentation on how niagara works ->](https://dev.epicgames.com/documentation/en-us/unreal-engine/creating-visual-effects-in-niagara-for-unreal-engine) It may proove usefull to understand how the new Niagara system works and how we can use it to replace the old legacy cascade particle emiter
4. [UE5 Documentation on a general overview for Niagara ->](https://dev.epicgames.com/documentation/en-us/unreal-engine/overview-of-niagara-effects-for-unreal-engine) Niagara is way more robust than Cascade so we better spend some good time understanding how it works
5. [UE5 mini course on Niagara control through Blueprints ->](https://dev.epicgames.com/community/learning/tutorials/vaEw/unreal-engine-blueprint-module-controlling-niagara-particles-part-1) It will allow us to understand how to change the system so it takes Niagara systems instead of Cascade.
6. STEVEN KEARNY I SUMMON THE WITH ALL YOUR MIGTHY BLUEPRINTS POWERS IN ORDER TO HELP ME UNDERSTAND HOW TF TO MAKE THIS WORK
7. JEFF PLAMONDON I INVOKE YER ALLMIGTHY 3D POWERS TO HELP ME UNDERSTAND AND DOCUMENT HOW TO MAKE THE BONES AND WEIGHT THINGS WORK
8. GREG WHOSE SECOND NAME I DONT REALLY KNOW BUT I KNOW YOU ARE QUITE THE AMAZING CODER, I ALSO INVOKE YER POWERS TO HELP AN AMBICIOUS MF!!
9. GOD ALMIGHTY GIVE MY BRAIN THE POWER OF THE SPONGE TO ABSORB ALL OF THIS KNOWLEDGE AND SUCCESFULLY OVERCOME THIS DIFICULT TASK FOR IF I AM WITH YOU THERE IS NO WAY ILL LOOSE
    '''
    ISAIAH 41:10 "FEAR NOT, FOR I AM WITH YOU; BE NOT DISMAYED, FOR I AM YOUR GOD; I WILL STRENGTHEN YOU, I WILL HELP YOU, I WILL UPHOLD YOU WITH MY RIGTHEOUS RIGHT HAND!!!"
    '''
    In jesus name I pray for the success of this project.



# Documentation Proyect ID => RandomMathBullshitGo

Le documentation for le system that le fletcher built based on procedural generation, will add more documentation whenever I get to peep them files
