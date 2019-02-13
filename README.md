# Simplex-Noise based Map Generator
This is a java port of [Sebastian Lague](https://github.com/SebLague)'s map generetor, Thank you! <3. This version is based on the Simplex-Noise (the simplex noise implementation was written by [Stefan Gustavson](https://github.com/stegu)) algorithm. The map generator class uses the Vector2 LibGdx implementation but you can modify it to use any Pair/Point/Vector class.
## Usage example
The MapGenerator has two static methods to generate the noise map, one generates a map and returns it, the other puts the map values inside a float matrix passed as parameter.
```java
float[][] map = new float[height][width];
MapGenerator.GenerateNoiseMap(map, mapWidth, mapHeight, seed, scale, octaves, persistence, lacunarity, offset);

//Alternatively
float[][] map = MapGenerator.GenerateNoiseMap(mapWidth, mapHeight, seed, scale, octaves, persistence, lacunarity, offset);
```
## Results
Here are some images I created for a game project (I use LibGdx this is why I used the Vector2 class)
![hope](mapgen/map_ex1.png"Hope")
![you](mapgen/map_ex2.png"You")
![enjoy](mapgen/map_ex3.png"Enjoy")
![:)](mapgen/map_ex4.png":)")
