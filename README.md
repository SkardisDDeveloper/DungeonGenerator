![obrazek](https://github.com/user-attachments/assets/fd32ce67-96de-45b1-9801-82bc6e7b4713)
![obrazek](https://github.com/user-attachments/assets/460b114c-123d-42c5-ae55-3a66f9576c0b)
![obrazek](https://github.com/user-attachments/assets/9569ba03-e657-4a5e-a608-8b253d93a066)

Setup:
------------------------
1. Import unity package
2. Make your own prefabs or use the one in the package.
     Prefabs you must have:
       -As many room prefabs as you want
       -11 Path prefabs for each scenario F-Front(Z+), B-Back(Z-), R-Right(X+), L-Left(X-) (HallwayLR, HallwayFB, HallwayFR, HallwayFL, HallwayBR, HallwayBL, HallwayBLR, HallwayFLR, HallwayFBR, HallwayFBL, HallwayFBRL) they must be the size of 1x1x1 cube in unity, otherwise you would need to tweak the settings of the 3D grid.
       -4 Stairs prefabs for each direction X+, X-, Z+, Z- they must be the size of 2x2x1 cube in unity, otherwise you would need to tweak the settings of the 3D grid.
       -Door for each axis (Make them based on prefabs in package, hard to exlain)
   !!! I plan to make it so you can put more variants of each door and stairs and hallways but time is not my friend sry, but it should just be when it chooses the number in the list change it to a list of the thing and choose one random out of it !!!
3. Put Dungeon Generator script on empty object, dungeon will generate based on size you put into positive X and Z axis
4. Put Size and number of rooms you want. It might generate longer the bigger and more rooms you put in. (Room Count is number of tries to spawn room, not final number of rooms created)
5. Put Prefabs correctly:
  Rooms - doesn't matter
  Path in this order - 0 - HallwayLR, 1 - HallwayFB, 2 - HallwayBR, 3 - HallwayBL, 4 - HallwayFR, 5 - HallwayFL, 6 - HallwayBRL, 7 - HallwayFBR, 8 - HallwayFBL, 9 - HallwayFRL, 10 - HallwayFBRL
  Stairs in this order - 0 - StairsXPositive, 1 - StairsXNegative, 2 - StairsZPositive, 3 - StairsZNegative
  Doors in this order - 0 - DoorLeft, 1 - DoorRight, 2 - DoorFront, 3 - DoorBack
6. HOPE AND PRAY!!!
It takes a few seconds to generate.
